# Saha Ziyaret – Telefon uygulaması kurulumu

Bu proje GitHub Pages üzerinde **PWA** olarak çalışacak şekilde hazırlanmıştır.

## Android telefona kurulum
1. Chrome'da `https://kapgan1453.github.io/SAHA/` adresini açın.
2. Menüden **Uygulamayı yükle** veya **Ana ekrana ekle** seçin.
3. Uygulama, ayrı bir uygulama penceresinde açılır.

## Güncellemeler
GitHub'a yeni commit gönderildiğinde GitHub Pages yeni `index.html` dosyasını yayınlar. Service worker her açılışta ana dosyayı ağdan kontrol eder; yeni sürüm bulunursa ekranda **Güncelle** düğmesi görünür.

## Gerçek APK
APK istenirse bu uygulama Capacitor veya Trusted Web Activity ile paketlenebilir. Uygulama URL'si aynı kaldığı sürece APK'nın kendisini yeniden yayınlamadan GitHub Pages'teki web kodu güncellenir. Ancak APK'nın çevrimdışı çalışması ve uygulama mağazasında yayınlanması için ayrıca Android imzalama/mağaza ayarları gerekir.

## Önemli güvenlik notu
Firebase bağlantı ayarları istemci tarafında görünür; bu normaldir. Ancak Firestore güvenlik kuralları ve kullanıcı parolaları mutlaka Firebase Console'da güvenli şekilde yapılandırılmalıdır. Gerçek kullanıcı şifrelerini yalnızca HTML içinde tutmayın.
