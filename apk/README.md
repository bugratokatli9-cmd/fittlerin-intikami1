# Fittlerin İntikamı – APK

## En kolay yol (bilgisayara kurulum yok): GitHub ile
1. github.com'da ücretsiz hesap aç, yeni bir depo (repository) oluştur.
2. Bu klasörün içindekileri (.github klasörü dahil) depoya yükle.
3. Depoda "Actions" sekmesine gir, "APK olustur" çalışmasının bitmesini bekle (3-6 dk).
4. Çalışmanın sayfasında en altta "fittlerin-intikami-apk" dosyasını indir, zip'ten çıkan app-debug.apk'yı telefona at.
5. Telefonda "bilinmeyen kaynaklardan yükleme"ye izin ver ve APK'ya dokun.

## Bilgisayarda kendin derlemek istersen
Gerekenler: Node.js 18+, JDK 17, Android Studio (SDK ile).
    npm install
    npx cap add android
    npx cap sync android
    cd android && ./gradlew assembleDebug
APK: android/app/build/outputs/apk/debug/app-debug.apk

Oyunu değiştirmek için www/index.html dosyasını düzenle.
