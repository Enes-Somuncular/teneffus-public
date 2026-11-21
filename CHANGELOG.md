# Sürüm Geçmişi (Changelog)

## v1.6.4 (Daha Sade & Okunaklı 2×2 Oyun Kartları — 2026-11-21)
- **Kart Sadeleştirmesi (`HubHome`):** Tüm kart alanı zaten tıklanabilir olduğu için 2×2 oyun kartlarının altındaki tekrarlayan *Oyna* tuşu kaldırıldı; başlık tipografisi büyütülüp alt meta satırı ince bir ayraç çizgisiyle daha temiz ve ferah hale getirildi.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.6.4` olarak güncellendi.

## v1.6.3 (2×2 Kompakt Oyun Vitrini — 2026-11-21)
- **2×2 Kompakt Hub Oyun Vitrini (`HubHome`):** Ana sayfadaki oyun kartları tek sütundan **2 sütunlu eşit yükseklikte vitrin düzenine** (`grid-cols-2`) geçirildi. Tüm oyunlar tek bakışta kaydırmadan görülebilir hale geldi; kısa rozetler (*6 Rol*, *800 Kelime*, *72 Mekân*, *360 Kart*), iki satırlık vurucu özetler, kişi sayısı/süre bilgisi ve yüksek kontrastlı tam genişlik *Oyna* butonlarıyla sadeleştirildi.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.6.3` olarak güncellendi.

## v1.6.2 (Kompakt & Şık Sayısal Ayar Kartları — 2026-11-21)
- **Kompakt Sayısal Ayar Kartı (`NumericStepperInput`):** Sayısal ayar kartlarındaki gereksiz açıklama satırları kaldırıldı; sayı ve birimin (`180 sn`, `60 sn`, `3 pas`, `-1 puan`) kutu içinde boşluksuz, dengeli ve tek boyutta hizalandığı daha zarif bir tasarım uygulandı.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.6.2` olarak güncellendi.

## v1.6.1 (Tüm Oyunlarda Serbest Sayısal Ayarlar & Yasaklı Kelime v1.1.0 — 2026-11-21)
- **Serbest Sayısal Ayarlar (`NumericStepperInput` — `- / +` + Klavyeden Direkt Giriş + Hızlı Seçenekler):**
  - **Yasaklı Kelime `v1.1.0`:** *Anlatım Süresi* (`10..600 sn`), *Tur Başına Pas Hakkı* (`0..99 pas` + `Sınırsız`), *Yasak (Tabu) Cezası* (`0..-20 puan`), *Tur Sayısı* (`1..25 tur`) ve *Hedef Puan* (`5..500 puan`) ayarlarının tamamı `- / +` tuşları ve klavyeden doğrudan sayı yazma desteğiyle özgürleştirildi.
  - **3+ Kişilik Takımsız (Bireysel) Mod Doğru Düğmesi Düzeltmesi:** 3+ kişilik Bireysel modda hem anlatan hem bilen `+1 puan` aldığı için bilenin seçilmemesine yol açan alttaki genel `"Doğru (+1)"` tuşu kaldırıldı; doğru kart seçimi doğrudan **Doğru Bilen Oyuncuyu Seç** butonlarıyla yapılır ve Tur Özeti ekranından da bilen kişi değiştirilebilir.
  - **Vampir-Köylü `v1.4.3`, Kelime Sahtekarı `v1.2.1` ve Casus Kim? `v1.0.1`:** Sabit 4 seçenekli *Tartışma Süresi* ve *Çapraz Sorgu Süresi* seçicileri `- / +`, klavyeden saniye girişi, hazır dakika kısayolları ve *Süresiz* anahtarı içeren yeni sayısal bileşene geçirildi.
- **Birim Testleri:** Toplam Vitest birim testi sayısı **48/48**'e çıkarıldı.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.6.1` olarak güncellendi.

## v1.6.0 (Yasaklı Kelime v1.0.0 Lansmanı — 2026-11-21)
- **Yeni Oyun — Yasaklı Kelime `v1.0.0` (2–16 Kişi):**
  - **İki Oynanış Modu:** 2–12 kişilik **Takımsız (Bireysel / Küçük Grup)** modu (*hem anlatana hem bilene +1 puan*) ve 4–16 kişilik **Klasik Takım (Tabu)** modu (*A Takımı vs. B Takımı*).
  - **6 Kategori • 360 Kart (2.160 Kelime) + Özel Kart Ekle (`localStorage`):** *Günlük Hayat & Eşyalar*, *Yemek, İçecek & Mutfak*, *Kültür, Sanat & Eğlence*, *Spor, Oyun & Hobi*, *Bilim, Doğa & Teknoloji* ve *Duygular, Deyimler & Kavramlar* paketleri ile özel kart oluşturma desteği eklendi.
  - **Anti-Kopya Duraklatma & Tur Sonu Masa İtirazı Düzeltmesi:** Süre duraklatıldığında kelimeyi gizleyen kalkan ve tur sonunda oynanan kartların durumunu (*Doğru ↔ Yasak ↔ Pas*) tek dokunuşla düzeltme sistemi eklendi.
  - **Birim Testleri:** 5 yeni Vitest motor birim testiyle toplam test sayısı **47/47**'ye ulaştı.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.6.0` olarak güncellendi.

## v1.5.4 (Oyun Kartları & Oyun Başlığı Sürüm Konumlandırması — 2026-11-21)
- **Zarif Oyun Sürüm Etiketleri:** Oyun kartlarındaki ve oyun içi üst başlıktaki büyük sürüm kutucukları başlıkların yanından kaldırılarak kartların alt bilgi satırına ve alt başlık sonuna daha küçük, sade bir tipografiyle taşındı.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.5.4` olarak güncellendi.

## v1.5.3 (Web-App Tek Dokunuşla Yenile / Güncelle Butonu — 2026-11-21)
- **Sağ Üst "Yenile" Butonu:** Web-App (Standalone PWA) modunda uygulamadan çıkıp girmeye gerek kalmadan yeni güncellemeleri anında çekip sayfayı yenileyen (çevrimdışı modda ise yerel önbelleği bozmadan güvenle yenileyen) sağ üst **Yenile** butonu eklendi.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.5.3` olarak güncellendi.

## v1.5.2 (Sadeleştirilmiş Hub Başlığı & Alt Bilgi Sürüm Rozeti — 2026-11-21)
- **Hub Başlığı & Alt Bilgi:** Üst başlıktaki Teneffüs logosu ve başlık alanı sadeleştirilerek site sürüm rozeti (`v1.5.2`) alt bilgi (footer) bölümüne taşındı.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.5.2` olarak güncellendi.

## v1.5.1 (%100 Anonim Canlı Topluluk Nabzı, Yerel Fontlar & KVKK Notu — 2026-11-21)
- **Canlı Topluluk Nabzı (`CommunityStatsCard` & Cloudflare Worker + KV):** Hiçbir IP adresi, cihaz kimliği, çerez veya oyuncu ismi kaydetmeden anlık aktif masa sayısını ve bu hafta oynanan el/oyuncu sayısını gösteren, çevrimdışı modda da sorunsuz çalışan anonim topluluk istatistiği eklendi.
- **Yerel Yazı Tipi (`Plus Jakarta Sans` Self-Hosted `.woff2`):** Google Fonts dış bağlantısı kaldırılarak yazı tipleri doğrudan uygulama paketine ve çevrimdışı PWA önbelleğine dahil edildi (sıfır dış IP aktarımı, birebir aynı görünüm).
- **Site İçi Gizlilik & KVKK Aydınlatma Notu:** Hub alt bölümüne tek dokunuşla açılan şeffaf KVKK ve gizlilik bilgilendirme penceresi eklendi.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.5.1` olarak güncellendi.

## v1.5.0 (Casus Kim? v1.0.0 Lansmanı — 2026-11-21)
- **Yeni Oyun — Casus Kim? `v1.0.0`:**
  - **6 Tema Paketi, 72 Mekân ve 720 Rol Kimliği:** *Türkiye & Bizden*, *Seyahat & Ulaşım*, *Eğlence & Etkinlik*, *Kurumlar & Mekânlar*, *Macera & Fantastik* ve *Sosyal Hayat & Buluşma* paketleri ile her mekâna özel 10 rol eklendi.
  - **Özel Mekân Ekle (`localStorage`):** Arkadaş grubunuza özel mekânlar ekleyip kaydetme desteği eklendi.
  - **Birebir Çapraz Sorgu & İnteraktif Masa Panosu:** İlk soru eşleşmesi, tek dokunuşla rastgele sorgu sorusu önerici, üzeri çizilebilir 16'lı *Olası Mekânlar Panosu* ve **“Casusum — Mekânı Buldum!”** anında baskın mekaniği eklendi.
  - **Oylama, Son Şans & Esnek Casus Sayısı:** Açık Masa / Gizli oylama, 6 Şıklı / Yazarak / Sözlü / Kapalı mekân tahmin modları, sınırsız/önerilen casus sayısı ve 7 yeni Vitest motor birim testi (toplam 42 test) eklendi.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.5.0` olarak güncellendi.

## v1.4.6 (iOS Web-App Güvenli Alan & Yeni İkon Tasarımı — 2026-11-21)
- **iOS Web-App (Standalone PWA) Üst Boşluk & Netlik Düzeltmesi:** iPhone Web-App modunda üst durum/bildirim çubuğu bulanıklığının (`status-bar blur`) başlık ve logoya binmesini önleyen güvenli üst boşluk (`pt-safe-hub` ve `pt-safe-header`), durum çubuğu koruma katmanı (`ios-statusbar-shield`) ve filtre kaynaklı WebKit bulanıklığını ortadan kaldıran saf vektörel `BrandLogo` bileşeni eklendi.
- **Yeni Uygulama İkonu & iOS Ana Ekran Desteği:** Çift oyun kartlı (Vampir-Köylü & Kelime Sahtekarı) yeni Teneffüs ikonu tasarlandı; iOS Safari `apple-touch-icon` için `180x180` yüksek çözünürlüklü PNG (`apple-touch-icon.png`), PWA manifesti için `192x192` ve `512x512` PNG/SVG ikon setleri eklendi.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.4.6` olarak güncellendi.

## v1.4.5 (Kelime Sahtekarı v1.2.0 — 800 Kelimelik Genişletilmiş Havuz — 2026-11-21)
- **Kelime Sahtekarı `v1.2.0`:** 10 kategorinin tamamı kategori başına **45 → 80** kelimeye çıkarılarak toplam yerleşik kelime havuzu **450 → 800** benzersiz, günlük hayattan tanıdık Türkçe kelime ve dengeli tek kelimelik çağrışım ipucuna yükseltildi.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.4.5` olarak güncellendi.

## v1.4.4 (Vampir-Köylü v1.4.2 — Sadeleştirilmiş Tam Elden Ele Akış — 2026-11-21)
- **Vampir-Köylü `v1.4.2`:** Gereksiz *Anlatıcı Yardımcılı* mod seçeneği kaldırılarak kurulum ekranı ve oyun akışı doğrudan tek telefondan tam elden ele (*Pass-and-Play*) deneyime sadeleştirildi.
- **PWA Önbelleği:** Service Worker önbellek sürümü `teneffus-v1.4.4` olarak güncellendi.

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
