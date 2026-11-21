# Mimari Bakış (Architecture Overview)

Teneffüs, birbirinden bağımsız elden ele parti oyunlarını tek bir çatı altında toplayan modüler bir istemci tarafı web uygulamasıdır.

## 1. Hub Registry Mimarisi
- Her oyun kendi modülünde izole edilir ve merkezi bir `HUB_GAMES` oyun kayıt listesi (registry) üzerinden Hub'a bağlanır.
- Hub (`/`), paylaşılan oyuncu ekibini, tüm oyunlar için devam eden oturum kartlarını, sürüm etiketlerini ve oyun rotalarını (`/oyun/:slug`) yönetir.

## 2. Paylaşılan Pass-and-Play Bileşenleri & Mobil Korumalar
- **Gizlilik Kalkanları (`PassPhoneShield`, `HoldToReveal`):** Elden ele telefon devrinde ekranın kazara görülmesini önleyen onay ve basılı tutarak açma bileşenleri.
- **Dokunmatik Korumalar:** Çoklu dokunma (pinch-zoom) hareketlerini, uzun basma bağlam menüsünü ve oyun içi metin seçimini engelleyen mobil koruma katmanı (`mobileGuards`), form girişleri (`input`/`textarea`) hariç tüm ekranda aktif tutulur.
- **Otomatik Konum & Sayaç Yönetimi:** Her faz/oyuncu geçişinde sayfa en üste hizalanır; tartışma sayaçları tur bazlı yenilenir.

## 3. İzole Oyun Motorları (`Vampir-Köylü` & `Kelime Sahtekarı`)
- **Vampir-Köylü:** Takım bazlı rol dağıtımı, rol içi ayarlar, gece takım oyu görünürlük kombinasyonları, çoklu doktor/dedektif/avcı motor desteği, gece çözümleme, koruma/sorgu/avcı zincirleri ve oylama akışı **21 Vitest birim testi** ile doğrulanır.
- **Kelime Sahtekarı:** 10 kategori (450 kelime) + özel liste havuzu, sınırsız özel sahtekar desteği, zorlaştırılmış çağrışım ipuçları, tekrarsız kelime seçimi, Açık Masa / Gizli oylama, Türkçe karakter esnekliğiyle yazarak tahmin ve şıklı/sözlü son şans kuralları **11 Vitest birim testi** ile doğrulanır; tut-sürükle sıralama yardımcısı **3 birim testi** ile kapsanır (toplam **35 birim testi**).

## 4. Çevrimdışı PWA & Edge Dağıtımı
- **Service Worker:** Uygulama kabuğu (`/`), `manifest.webmanifest`, uygulama simgesi ve hash'li Vite JS/CSS paketleri cihazda önbelleğe alınır.
- **Cloudflare Workers Static Assets:** Uygulama sunucusuz statik varlık olarak SPA fallback (`single-page-application`) yapılandırmasıyla Cloudflare edge ağı üzerinden sunulur.
