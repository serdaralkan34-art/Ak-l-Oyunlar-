# Akıl Oyunları — telefondan APK alma

## Dürüst durum
Bu paket Android uygulama kaynak projesidir; içinde hazır APK yoktur. Bu ortamda Android SDK/Gradle derleyicisi bulunmadığı için APK'yı burada derleyemiyorum. Projede GitHub Actions bulut derleme akışı vardır.

## Telefonda yapılacaklar
1. Telefonda tarayıcıdan GitHub hesabı açın veya giriş yapın.
2. Yeni, herkese açık olmayan (Private) bir repository oluşturun: `akil-oyunlari`.
3. Bu ZIP'i telefona indirin ve arşivden çıkarın.
4. GitHub mobil web sitesinde repository içine dosyaları yükleyin. Klasör yapısını koruyarak tüm dosyaları ekleyin; `.github/workflows/build-apk.yml` dosyası da yüklenmiş olmalı.
5. Repository > Actions bölümüne girin. `Android APK` iş akışını seçip `Run workflow` düğmesine dokunun.
6. İşlem tamamlanınca ilgili çalıştırmayı açın, Artifacts bölümünden `Akil-Oyunlari-debug-APK` dosyasını indirin.
7. ZIP içindeki `app-debug.apk` dosyasını açıp Android'in istediği uygulama yükleme iznini verin.

## Uygulamanın bu sürümdeki durumu
- Android WebView kabuğu ve Türkçe örnek arayüz vardır.
- Futbol/basketbol sekmeleri ve maç detay ekranı örnek içerikle çalışır.
- Maçlar, tarihler ve olasılık alanları gerçek zamanlı veri değildir. Olasılıklar bilerek `—` gösterilir.
- Henüz API bağlantısı, sunucu, bildirim, gerçek tahmin modeli veya kapsamlı arşiv yoktur.
- Bu bir debug/test APK'sıdır; Play Store yayını için imzalı release, gizlilik politikası, veri lisansları ve testler gerekir.

## Güvenlik
API anahtarlarını Android uygulamasına gömmeyin ve herkese açık GitHub deposuna koymayın. Gerçek veri bağlantısı için anahtarlar sunucu tarafında tutulmalıdır.
