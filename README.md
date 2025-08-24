# 🎬 izletiyo.com

**Gerçek zamanlı senkronize film izleme platformu**

Arkadaşlarınızla mesafe tanımadan beraber film izleyin! izletiyo.com, YouTube videolarını senkronize bir şekilde çoklu kullanıcılarla izlemenizi sağlayan bir web uygulamasıdır.

## ✨ Özellikler

### 🎯 Temel Özellikler
- **Gerçek Zamanlı Senkronizasyon**: Tüm izleyiciler aynı anda play/pause olur
- **Otomatik URL Tanıma**: YouTube linkini yapıştırın, otomatik başlasın
- **Film Arama**: YouTube API ile binlerce filme kolayca erişim
- **Süre Gösterimi**: Her film için detaylı süre bilgisi
- **Önceden Seçilmiş İçerik**: Popüler Türk filmleri ve içerikleri

### 🔧 Teknik Özellikler
- **Socket.IO**: Gerçek zamanlı iletişim
- **YouTube API v3**: Gelişmiş arama ve video detayları
- **Responsive Tasarım**: Mobil, tablet ve masaüstü uyumlu
- **Otomatik Room Oluşturma**: Benzersiz kanal kodları
- **Host/Guest Sistemi**: İlk başlatan kişi kontrolü sağlar

## 🚀 Nasıl Kullanılır

### 1. Hızlı Başlangıç
- [izletiyo.com](https://izletiyo.com) adresini ziyaret edin
- Otomatik olarak yeni bir oda oluşturulur
- Üst kısımdaki share kodunu arkadaşlarınızla paylaşın

### 2. Film Seçimi
**YouTube URL ile:**
```
https://www.youtube.com/watch?v=VIDEO_ID
veya
https://youtu.be/VIDEO_ID
```
- URL'yi arama kutusuna yapıştırın
- Enter'a basın veya "Ara" butonuna tıklayın
- Video otomatik başlar

**Arama ile:**
- Film adını yazın (örnek: "Üç Kağıtçı")
- Arama sonuçlarından istediğinizi seçin
- Tıkladığınız video başlar

### 3. Senkronize İzleme
- Host (ilk başlatan) kontrolü sağlar
- Play/pause işlemleri tüm katılımcılara yansır
- Yeni katılanlar otomatik senkronize olur

## 🛠️ Teknik Detaylar

### Kullanılan Teknolojiler
- **Frontend**: Vanilla JavaScript, HTML5, CSS3
- **Real-time**: Socket.IO 4.5.3
- **Video Player**: YouTube IFrame API
- **API**: YouTube Data API v3
- **Font**: Google Fonts (Nunito)
- **Framework**: Documenter.js

### Sistem Mimarisi
```
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   İstemci 1     │    │  Signal Server   │    │   İstemci 2     │
│                 │◄──►│  (kuruyo.com)    │◄──►│                 │
│  YouTube API    │    │  Socket.IO       │    │  YouTube API    │
└─────────────────┘    └──────────────────┘    └─────────────────┘
```

### Signal Sistemi
- **Room Management**: Otomatik kullanıcı takibi
- **Message Broadcasting**: Anlık komut iletimi
- **Reconnection**: Otomatik yeniden bağlanma
- **Channel Codes**: Benzersiz oda tanımlayıcıları

## 📱 Responsive Tasarım

- **Masaüstü**: 3 sütunlu grid düzeni
- **Tablet**: 2 sütunlu düzen
- **Mobil**: Tek sütun, flex düzeni
- **Touch Optimized**: Mobil dokunma deneyimi

## 🎨 UI/UX Özellikleri

- **Hover Efektleri**: Kartlar üzerinde scale animasyonu
- **Loading States**: Buton loading animasyonları
- **Success Feedback**: ✔ işareti ile başarı bildirimi
- **Gradient Overlays**: Film başlıkları için okunabilirlik
- **Duration Badges**: Sağ üst köşede süre göstergesi

## 🔐 Güvenlik

- **HTTPS Only**: Güvenli bağlantı zorunluluğu
- **API Key Protection**: YouTube API anahtarı koruması
- **Cross-Origin**: CORS politikaları
- **Input Validation**: URL doğrulama kontrolleri

## 🌐 Canlı Demo

**Web Sitesi**: [izletiyo.com](https://izletiyo.com)

### Test için örnek URL'ler:
```
https://www.youtube.com/watch?v=wmPSBa1SRA4  (Üç Kağıtçı)
https://www.youtube.com/watch?v=YHEQO9slYjI  (Sahte Kabadayı)
https://youtu.be/UQRc5I6jeSA               (Korkusuz Korkak)
```

## 🤝 Katkıda Bulunun

1. Repo'yu fork edin
2. Feature branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Değişikliklerinizi commit edin (`git commit -m 'Add amazing feature'`)
4. Branch'i push edin (`git push origin feature/amazing-feature`)
5. Pull Request açın

## 📄 Lisans

Bu proje MIT lisansı altında lisanslanmıştır. Detaylar için [LICENSE](LICENSE) dosyasına bakın.

## 🏢 Geliştirici

**topluyo** tarafından geliştirilmiştir.

---

💝 **izletiyo.com** - Mesafe tanımayan dostluklar için!
