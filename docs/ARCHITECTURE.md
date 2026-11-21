# Mimari Bakış (Architecture Overview)

Teneffüs, birbirinden bağımsız elden ele parti oyunlarını tek bir çatı altında toplayan modüler bir istemci tarafı web uygulamasıdır.

## 1. Hub Registry Mimarisi
- Her oyun kendi modülünde izole edilir ve merkezi bir `HUB_GAMES` oyun kayıt listesi (registry) üzerinden Hub'a bağlanır.
- Hub (`/`), paylaşılan oyuncu ekibini, aktif oyun devam bildirimini, sürüm etiketlerini ve oyun rotasını (`/oyun/:slug`) yönetir.

## 2. Paylaşılan Pass-and-Play Bileşenleri & Mobil Korumalar
- **Gizlilik Kalkanları (`PassPhoneShield`, `HoldToReveal`):** Elden ele telefon devrinde ekranın kazara görülmesini önleyen onay ve basılı tutarak açma bileşenleri.
- **Dokunmatik Korumalar:** Çoklu dokunma (pinch-zoom) hareketlerini, uzun basma bağlam menüsünü ve oyun içi metin seçimini engelleyen mobil koruma katmanı (`mobileGuards`), form girişleri (`input`/`textarea`) hariç tüm ekranda aktif tutulur.
- **Otomatik Konum & Sayac Yönetimi:** Her faz/oyuncu geçişinde sayfa en üste hizalanır; gündüz tartışma sayacı oyun turuna göre yönetilir.

## 3. İzole Oyun Motoru (`Vampir-Köylü`)
- Tüm rol dağıtımı, gece çözümleme, koruma/sorgu/avcı zincirleri, oylama ve kazanma kontrolleri React arayüzünden tamamen bağımsız saf TypeScript fonksiyonları olarak uygulanmıştır.
- Bu motor, arayüzden ayrı olarak **19 Vitest birim testi** ile doğrulanmaktadır.

## 4. Çevrimdışı PWA & Edge Dağıtımı
- **Service Worker:** Uygulama kabuğu (`/`), `manifest.webmanifest`, uygulama simgesi ve hash'li Vite JS/CSS paketleri cihazda önbelleğe alınır.
- **Cloudflare Workers Static Assets:** Uygulama sunucusuz statik varlık olarak tek seferlik SPA fallback (`single-page-application`) yapılandırmasıyla Cloudflare edge ağı üzerinden sunulur.
