# İlim Takip — çevrimdışı PWA

## Dosyalar
- `index.html`: uygulama ekranları
- `styles.css`: tablet ve telefon uyumlu görünüm, açık/koyu tema
- `app.js`: program, yerel kayıtlar, sayaç, raporlar ve JSON yedekleme
- `manifest.webmanifest`: PWA kurulum bilgileri
- `sw.js`: uygulama dosyalarını çevrimdışı önbelleğe alma
- `icon.svg`: uygulama simgesi

## Önemli sınırlama
Bu proje PWA'dır; Android APK değildir. Tarayıcıdan kurulduğunda desteklenen tarayıcılarda uygulama gibi açılır. İlk kez yüklemek ve servis çalışanını kurmak için bir HTTPS adresi gerekir. Kurulum/önbellekleme tamamlandıktan sonra uygulamanın temel özellikleri çevrimdışı çalışır. Veriler yalnızca aynı tarayıcının yerel depolamasındadır; tarayıcı verilerini silmek kayıtları silebilir. JSON yedeğini düzenli alın.

## Çalıştırma
1. Klasörün bütün dosyalarını bir HTTPS statik site barındırıcısına yükleyin; dosyaların hepsi aynı klasörde olmalı.
2. Samsung tablette Chrome veya Samsung Internet ile sitenin adresini açın.
3. Sayfanın ilk açılışının tamamlanmasını ve çevrimdışı önbelleğin kurulmasını bekleyin. Sonra bir kez yenileyin.
4. Tarayıcı menüsünden **Uygulamayı yükle** veya **Ana ekrana ekle** seçeneğini kullanın. Menü metni tarayıcı sürümüne göre değişebilir.
5. Kurulumdan sonra interneti kapatıp uygulamayı açarak deneyin.

## Yerel geliştirme testi
`file://` üzerinden açıldığında arayüz çalışabilir fakat PWA servis çalışanı kurulmaz. PWA testi için HTTPS veya localhost gerekir.
