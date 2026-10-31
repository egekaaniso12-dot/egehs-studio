# EgeHS Studio

EgeHS Studio, görsel üretimi ve düzenleme, YouTube kapak fikirleri, referans kütüphanesi ve video üretimini tek bir galeride birleştiren yerel çalışma alanıdır. Bu sürüm, kullanıcı tarafından sağlanan açık kaynak Banana Studio kod tabanından MIT lisansı altında uyarlanmıştır. Orijinal telif ve lisans bildirimi `LICENSE` dosyasında korunmuştur.

## Özellikler

- Görsel üretimi: GPT Image 2.5, Nano Banana Pro ve Nano Banana 2.1.
- Görsel düzenleme: referans görsel, bölge seçimi, maske ve kaynak/sonuç karşılaştırması.
- Brainstorm ve Enhance ile fikir ve prompt hazırlama.
- Seedance ve MiniMax sağlayıcılarıyla video üretimi.
- Galeri, klasörler, arama, favoriler, kişi ve referans kütüphanesi.
- Sağlayıcı ve model seçimi, üretim öncesi maliyet tahmini ve geçmiş maliyet bilgileri.
- Tek tıkla ekonomik görsel ayarı: 1K, Low kalite ve tek çıktı.
- Windows masaüstü uygulamasında API anahtarlarının Windows Credential Manager'da saklanması.

## Windows'ta kullanma

Bu kaynak arşivi Windows uygulamasını kendi bilgisayarınızda paketlemek içindir. Hazır Windows uygulaması oluşturmak için Windows 10/11 x64, .NET 8 SDK ve Node.js 22 gerekir. Proje kökünde:

```powershell
npm ci
npm run build
npm run build:desktop
```

Paket `.build/staging-windows/EgeHS Studio` dizinine çıkar. İlk açılışta **Provider API Keys…** menüsünden kullanacağınız sağlayıcının anahtarını kaydedin. Yalnızca kullanacağınız servisler için anahtar ekleyin. Anahtarlar uygulama tarafından Windows Credential Manager'da tutulur; kaynak koduna veya galeri kayıtlarına yazılmaz.

## Maliyeti düşük tutma

API kullanım ücretini ilgili sağlayıcı belirler; EgeHS Studio üretim başına abonelik veya kredi ücreti almaz. Üretimden önce model ve sağlayıcıyı seçin, maliyet tahminini kontrol edin, mümkün olduğunda **Ekonomi** düğmesiyle 1K/Low/tek görsel ayarını kullanın. Referans görselleri, daha yüksek kalite/çözünürlük ve video süresi fiyatı artırabilir. Tahmin kesin fiyat veya harcama limiti değildir; gerçek kullanım ücreti sağlayıcının döndürdüğü tüketim bilgisine göre değişir.

## Web sürümü

Bu kaynakta web dağıtım bileşenleri de yer alır. Web çalışma alanında sağlayıcı anahtarlarını tarayıcıya koymayın; dağıtımın sunucu tarafı ayarlarını yapılandırın. Kurulum ve mimari notları `docs/` içindedir.

## Lisans ve kaynak

Bu uyarlama MIT lisanslıdır. Orijinal telif bildirimi ve lisans koşulları `LICENSE` içinde yer alır. Üçüncü taraf bileşenlerin bildirimleri `docs/THIRD_PARTY_NOTICES.md` dosyasındadır.
