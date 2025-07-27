# js-developer-bootcamp2025-finalproject-selamicetin

LC Waikiki Product Carousel Implementation
Bu proje, LC Waikiki ürün sayfaları için modern ve tamamen responsive bir ürün karoseli uygulamasıdır. Kullanıcılar "Beğenebileceğiniz Diğer Ürünler" bölümünde benzer ürünleri görüntüleyebilir, favorilerine ekleyebilir ve ürün detaylarını inceleyebilir.

Özellikler
Responsive Tasarım: Masaüstü, tablet ve mobil cihazlarda mükemmel uyum

Favori Yönetimi: Ürünleri favorilere ekleme/çıkarma ve localStorage'da saklama

Karosel Navigasyonu: Yatay kaydırma, ok tuşları ve nokta navigasyonu

Gerçek Veri Entegrasyonu: Harici API'den ürün verilerini çekme

Performans Optimizasyonu: Verileri önbelleğe alma ve lazy loading

Teknik Yaklaşım
Code

graph TD
    A[Kullanıcı Ürün Sayfasını Ziyaret Eder] --> B[Karosel Scripti Yüklenir]
    B --> C{Ürün Sayfası mı?}
    C -->|Evet| D[Verileri Yükle]
    C -->|Hayır| E[İşlemi Sonlandır]
    D --> F{Veriler Önbellekte mi?}
    F -->|Evet| G[Önbellekten Yükle]
    F -->|Hayır| H[API'den Çek]
    G --> I[Karoseli Oluştur]
    H --> I
    I --> J[Favori Durumlarını Yükle]
    J --> K[Etkinlikleri Bağla]
    K --> L[Kullanıcı Etkileşimi]
    L --> M[Karosel Navigasyonu]
    L --> N[Favori İşlemleri]
    L --> O[Ürün Detayına Git]




Kurulum ve Kullanım
Projeyi kullanmak için aşağıdaki adımları izleyin:

Repoyu klonlayın:

bash
git clone https://github.com/Selami7321/js-developer-bootcamp2025-finalproject-selamicetin.git
Gerekli bağımlılıkları yükleyin:

bash
npm install
Geliştirme sunucusunu başlatın:

bash
npm run dev
Üretim için build alın:

bash
npm run build

Teknoloji Stacki
Vanilla JavaScript: Temel işlevler için saf JavaScript

SASS: Modern CSS yönetimi

Webpack: Modül paketleme ve optimizasyon

Babel: JavaScript uyumluluğu

ESLint ve Prettier: Kod kalitesi ve formatlama

Katkıda Bulunma
Katkılarınızı memnuniyetle karşılıyoruz! Lütfen katkıda bulunmadan önce aşağıdaki adımları izleyin:

Repoyu fork'layın

Yeni bir branch oluşturun (git checkout -b feature/amazing-feature)

Değişikliklerinizi commit edin (git commit -m 'Add some amazing feature')

Branch'inize push yapın (git push origin feature/amazing-feature)

Pull request açın

Lisans
Bu proje MIT lisansı altında lisanslanmıştır - detaylar için LICENSE dosyasına bakın.
