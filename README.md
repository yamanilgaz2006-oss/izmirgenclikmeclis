# İzmir Kent Konseyi Gençlik Meclisi — Web Sitesi

İzmir Kent Konseyi Gençlik Meclisi'nin tanıtım web sitesi. Tek sayfalık (single-page),
statik bir site olup Tailwind CSS ve FontAwesome CDN üzerinden çalışır — derleme adımı gerektirmez.

## Dosya Yapısı

```
.
├── index.html              # Sitenin tamamı (HTML + stil + JS aynı dosyada)
├── images/
│   ├── logo.png            # Meclis logosu
│   ├── hero-bg.png         # Ana bölüm arka plan görseli
│   └── events/             # Etkinlik fotoğrafları
│       ├── stem-zirvesi.jpeg
│       ├── oryantasyon.jpg
│       ├── meclis-simulasyonu.jpeg
│       ├── deniz-muzesi-gezisi.jpeg
│       ├── kibris-ziyareti.jpg
│       └── genclik-kampi.jpeg
└── README.md
```

## Çalıştırma

Tarayıcıda doğrudan `index.html` dosyasını açmanız yeterlidir. Alternatif olarak
yerel bir sunucu ile:

```bash
python3 -m http.server 8000
# ardından: http://localhost:8000
```

## Notlar

- Başvuru butonları `openFormUrl()` fonksiyonu üzerinden başvuru formuna yönlendirir.
  Form adresi `index.html` içindeki `defaultFormUrl` değişkeninden güncellenebilir.
- Etkinlikler `index.html` içindeki `defaultEvents` dizisinden düzenlenir; her etkinliğin
  görseli `images/events/` klasöründen referanslanır.
