# Naar Nederland - Hollandaca Öğrenme Uygulaması

Flash kartlar, arama ve pratik modları ile Hollandaca kelime öğrenmek için mobil uyumlu web uygulaması.

## Özellikler

- **15 Günlük Öğrenme Planı**: Les 21-65 yapılandırılmış müfredat
- **İnteraktif Flash Kartlar**: Pratik modu için çevrilebilir kartlar
- **Akıllı Arama**: Hem Hollandaca hem de Türkçe arama
- **Sesli Telaffuz**: Hollandaca kelimeler için metinden konuşma
- **Mobil Optimize**: Telefon/tablet kullanımı için mükemmel
- **İlerleme Takibi**: Görsel ilerleme göstergeleri

## Cloudflare Pages'e Yayınlama

### Adım 1: GitHub Deposu Oluştur
1. [GitHub](https://github.com) sitesine gidin ve yeni depo oluşturun
2. Adı: `naar-nederland-app`
3. Herkese açık veya özel seçebilirsiniz
4. README ile başlatmayın (biz zaten bir tane oluşturduk)

### Adım 2: GitHub'a Gönder
```bash
# GitHub deponuzu remote olarak ekleyin (YOUR_USERNAME kısmını değiştirin)
git remote add origin https://github.com/YOUR_USERNAME/naar-nederland-app.git
git branch -M main
git push -u origin main
```

### Adım 3: Cloudflare Pages'e Yayınla
1. [Cloudflare Panel](https://dash.cloudflare.com) gidin
2. **Pages** bölümüne gidin
3. **"Create a project"** tıklayın
4. **"Connect to Git"** seçin
5. GitHub'ı seçin ve yetkilendirme gerekiyorsa yapın
6. `naar-nederland-app` deponuzu seçin
7. **Build Ayarları**:
   - **Framework preset**: None
   - **Build command**: Boş bırakın
   - **Build output directory**: Boş bırakın (kök dizin)
8. **"Save and Deploy"** tıklayın

### Adım 4: URL'nizi Alın
Yayınlamadan sonra Cloudflare size verecek:
- **Preview URL**: Test için
- **Production URL**: Canlı siteniz (genellikle `your-project.pages.dev`)

## Özel Alan Adı (İsteğe Bağlı)
1. Cloudflare Pages proje ayarlarından
2. **"Custom domains"** gidin
3. Alan adınızı ekleyin (örneğin, `naar-nederland.com`)
4. DNS kayıtlarını talimatlara göre güncelleyin

## Proje Yapısı
```
leren/
├── index.html          # Ana uygulama dosyası
└── README.md          # Bu dosya
```

## Kullanılan Teknolojiler
- **HTML5** anlamsal işaretleme
- **Tailwind CSS** CDN üzerinden stil için
- **Font Awesome** ikonlar için
- **Vanilla JavaScript** fonksiyonellik için
- **Web Speech API** telaffuz için

## Notlar
- Derleme süreci gerekmiyor - statik HTML dosyası
- Tüm bağımlılıklar CDN üzerinden yüklenir
- Tamamen duyarlı tasarım
- Yüklendikten sonra çevrimdışı çalışır
