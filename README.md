# Clockify Dashboard

Kategori bazlı çalışma saatlerini gösteren, Clockify API'sinden canlı veri çeken bir dashboard.

## Özellikler

- **Kategoriye göre çalışma saatleri**: Recht, Makroökonomie, Statistik, Deutsch lernen
- **Günlük çizgi grafik**: son 30 günün günlük çalışma süreleri
- **7 günlük hareketli ortalama** (turuncu çizgi)
- **30 günlük hareketli ortalama** (yeşil çizgi)
- **Otomatik yenileme**: her 5 dakikada bir Clockify API'sinden güncel veri çeker
- Verileriniz sadece tarayıcınızda saklanır (localStorage), hiçbir sunucuya gönderilmez

## Kurulum

1. Bu repoyu GitHub Pages ile yayınlayın (Settings → Pages → Branch: main → / (root))
2. Siteyi açın, [Clockify API Key](https://app.clockify.me/user/settings) alanına kendi API anahtarınızı girin
3. "Kaydet ve Yükle" butonuna basın

## Kategori Eşleştirme

Dashboard, Clockify'daki **proje adlarını** veya **etiketleri (tags)** aşağıdaki isimlerle eşleştirir:

- `Recht`
- `Makroökonomie`
- `Statistik`
- `Deutsch lernen`

Bu isimlerle bir proje veya etiket oluşturup zaman kayıtlarınızı bunlara atadığınızda otomatik olarak grafiklere yansır.

## Teknoloji

Sadece HTML + vanilla JS + [Chart.js](https://www.chartjs.org/) kullanır. Build adımı veya backend gerektirmez.
