# Sürüm Geçmişi (Changelog)

## v1.4.3 (Sınırsız Rol & Sahtekar Desteği — 2026-11-21)
- **Vampir-Köylü `v1.4.1`:** *Doktor*, *Dedektif*, *Avcı* ve *Deli* rollerindeki adet sınırı kaldırıldı; çoklu doktor korumaları, bağımsız dedektif sorguları ve her avcının kendi hedefi tam motor/anlatıcı desteğiyle çalışacak şekilde geliştirildi.
- **Kelime Sahtekarı `v1.1.1`:** *Sahtekar* sayısındaki 3/çoğunluk kısıtı kaldırıldı; istenirse oyuncu sayısına kadar (kaotik mod dahil) serbest sahtekar seçimi ve tek dokunuşla *Önerilen* ayarına dönüş eklendi.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.4.3` olarak güncellendi.

## v1.4.2 (Vampir-Köylü v1.4.0 — Takımlı Rol Dağıtımı & Rol İçi Ayarlar — 2026-11-21)
- **3 Kategorili Rol Dağıtımı:** Vampir-Köylü rolleri **Vampir Takımı**, **Köy Halkı (Masum)** ve **Tarafsız** gruplarına ayrıldı.
- **Rol İçi Ayar Çekmeceleri:** *Doktor* ve *Vampir* ile ilgili özel kurallar doğrudan rol kartlarının üzerindeki ayarlar ikonuna taşındı; Genel Kural Ayarları sadeleştirildi.
- **Gece Takım Oyu Görünümü:** Vampirlerin gece diğer vampir oylarını **İsimli**, anonim **Vampir oyu** veya **Gizli** olarak görme seçeneği eklendi; birbirini tanıma ayarıyla uyumlu çalışır.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.4.2` olarak güncellendi.

## v1.4.1 (Sürükle-Bırak Sıralama & 450 Kelime — 2026-11-21)
- **Tut-Sürükle Oyuncu Sıralama:** Hub Oyuncu Ekibi (`RosterSheet`), Vampir-Köylü (`v1.3.1`) ve Kelime Sahtekarı (`v1.1.0`) kurulum ekranlarına dokunmatik ve fare destekli sürükle-bırak sıralama eklendi.
- **Kelime Sahtekarı `v1.1.0`:**
  - Toplam kelime havuzu 10 kategoride **260 → 450** benzersiz Türkçe kelimeye çıkarıldı (`45` kelime/kategori).
  - Sahtekar çağrışım ipuçları cevabı doğrudan ele vermeyecek şekilde daha dengeli ve ince ipuçlarıyla yenilendi.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.4.1` olarak güncellendi.

## v1.4.0 (Kelime Sahtekarı v1.0.0 Lansmanı — 2026-11-21)
- **Yeni Oyun — Kelime Sahtekarı `v1.0.0`:**
  - 10 kategoride 260 kürasyonlu Türkçe kelime ve tek/çoklu kategori seçimi eklendi.
  - Cihazda saklanan **Özel Kelime Ekle** havuzu eklendi.
  - Yakalanan sahtekarın oyunu çalması için **6 Şıklı**, **Yazarak** (büyük/küçük harf ve Türkçe karakter toleranslı), **Sözlü (Masa Onaylı)** ve **Kapalı** modları eklendi.
  - Anti-ipucu sabit yükseklikli kartlar, Açık Masa / Gizli oylama, tekrarsız kelime seçimi ve 10 yeni Vitest motor birim testi eklendi.
- **Hub Güncellemesi:** Oyun kartları kendi tema vurgusunu destekleyecek şekilde güncellendi; Devam Eden Oyun kartı aktif olan tüm oyunları listeler hale getirildi.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.4.0` olarak güncellendi.

## v1.3.1 (Hub Güncellemesi — 2026-11-21)
- **Geri Bildirim & Tanıtım Alt Bölümü:** Hub alt kısmına doğrudan e-posta (`enesso.iletisim@icloud.com`), tek dokunuşla kopyalama butonu ve GitHub tanıtım deposu bağlantısı eklendi.

## v1.3.0 (Vampir-Köylü & Mobil UX — 2026-11-21)
- **Ön-Hedefli Avcı Mekaniği:** Avcı artık ölmeden önce her gece hedefini seçip değiştirebiliyor; elendiğinde seçili hedefi yanında götürüyor.
- **Anti-İpucu Kompakt Rol Kartı:** Tüm roller için eşit yükseklikli gece kartları ve `(i)` rol bilgi penceresi eklendi; hedef seçimi ekranları tek ekranda kaydırmasız hizalandı.

## v1.2.0 (Oyun Akışı & Dokunmatik İyileştirmeler — 2026-11-21)
- **Tek Turda Rol + 1. Gece:** Oyuncular ilk gecede rollerini öğrendikten hemen sonra aynı turda ilk gece eylemini gerçekleştirebiliyor.
- **Açık Masa Oylaması:** Telefon masadayken sırayla tek dokunuşla oy verme ve geri alma seçeneği eklendi.
- **Paravan Eylemi Netliği & Metin Seçimi Koruması:** Köylü ve Deli gece ekranlarında paravan bilgilendirmesi netleştirildi; mobilde basılı tutarken metin kopyalama/seçme menüsü kapatıldı.

## v1.1.0 (Özelleştirilebilir Kurallar & Sürüm Rozetleri — 2026-11-21)
- **Özelleştirilebilir Kurallar:** Elenen kişinin rolünü gösterme, ilk gece vampir öldürme, doktor kuralları ve oylama stili ayarları eklendi.
- **Sürüm Görünürlüğü:** Hub ve oyun kartlarına ayrı sürüm etiketleri eklendi.
- **Mobil Odak & Yakınlaştırma Düzeltmeleri:** Giriş alanlarında otomatik yakınlaştırma engellendi ve faz geçişlerinde sayfa konumu sıfırlandı.

## v1.0.0 (İlk Yayın — 2026-11-21)
- **Teneffüs Hub** ve paylaşılan **Oyuncu Ekibi** yayına alındı.
- **Vampir-Köylü** (4–16 kişi, 6 rol, Moderatörsüz ve Anlatıcı Yardımcılı modlar, oyun günlüğü ve çevrimdışı PWA desteği) yayınlandı.
