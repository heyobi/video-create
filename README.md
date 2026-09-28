# Fon krizi · sonsuz zoom videoları

İki sayfalık, tek dosyalık HTML aracı. Bütün çizimler Canvas 2D ile kodda üretilir. Build aracı, framework ya da npm bağımlılığı yoktur. Tek harici kaynak Google Fonts'tan "Bricolage Grotesque".

- `index.html`: Shorts/Reels çekim sayfası (9:16, 7 sahne, 50,0 saniyelik kusursuz döngü)
- `uzun/index.html`: Yatay uzun video kurgu sayfası (16:9, 10 sahne, 14 anlatım adımı)
- `gezegen/index.html` ve `gezegen/uzun/index.html`: Aynı format, ikinci video: bilinen en genç gezegen Elias 2-24 b

## Shorts çekim akışı (telefonda)

1. Sayfayı aç, **Animasyonu oluştur (1 tur)** düğmesine dokun. Hazırlık 50 saniye sürer; bu sırada ekranı kapatma, sekmeden çıkma.
2. Düğme **Animasyonu kaydet** olunca dokun. iPhone'da paylaşım sayfasından "Videoyu Kaydet" ile galeriye gider (`animasyon.mp4`).
3. **Çekim moduna geç (kamera)**. Ön kamera sol alttaki anlatıcı kutusunda görünür, prompter ekranın tepesindedir. "Prompter: tam metin / ipucu" ile iki görünüm arasında geçiş yapılır.
4. **Çekime başla**. 3 saniyelik geri sayım biter bitmez kayıt ve animasyon aynı anda başlar, tam 50,0 saniyede kayıt kendiliğinden durur.
5. **Kamera kaydını kaydet** ile `kamera.mp4` dosyasını galeriye al. Beğenmediysen **Tekrar çek**.

## Edits'te birleştirme

1. Yeni proje aç, ana iz olarak `animasyon.mp4` dosyasını ekle.
2. `kamera.mp4` dosyasını üst katman (overlay) olarak ekle ve iki klibi 0. saniyeden hizala. İkisi de aynı uzunluktadır.
3. Kamera katmanında arka planı kaldır (Cutout / arka planı sil), kutuyu sol alttaki anlatıcı alanına yerleştir.
4. Sesi kamera klibinden al. Animasyon klibinde efektler var; sesini istersen kıs.
5. Dışa aktar. Video başa sardığında son cümle ilk cümleye bağlanır.

## Uzun video

Boşluk, sağ ok, sahneye dokunma ya da **Sonraki** bir adım ilerletir; sol ok bir adım geri götürür. Her adımda görüntü yavaşça süzülür. Sonraki adım yeni sahnedeyse 3,4 saniyelik dalış yapılır. **Otomatik akış** adımları metin uzunluğuna göre kendisi ilerletir. **Tam metin** bütün senaryoyu gösterir; bir adıma dokununca oraya atlanır. **Temiz görüntü** ekran kaydı için yalnızca sahneyi bırakır. Çıkmak için ekrana dokun ya da C tuşuna bas.

## Kısayollar

- Shorts hazırlık: Boşluk oynat/duraklat, C temiz görüntüden çık
- Uzun: Boşluk / sağ ok ileri, sol ok geri, C temiz görüntüden çık

## İçerik notu

Rakamlar 27 Eylül 2026 itibarıyla. Eski bakanla ilgili bütün bilgiler Yeni Parti Sözcüsü Zeynel Emre'nin **iddiası** olarak verilir; gerçek kişilerin görseli çizilmez.

## Video 2: Bilinen en genç gezegen (`/gezegen/`)

Konu: Eylül 2026'da doğrulanan Elias 2-24 b.

- 1 milyon yaşından genç, 450 ışık yılı uzakta, Yılancı takımyıldızında.
- Keck teleskobunun 2018 ve 2020 arşiv görüntülerinde bulundu.
- Kütlesi Jüpiter'in 2 ila 4 katı.
- Yıldızına yaklaşık 55 AB uzaklıkta, diskteki dar bir boşlukta duruyor.

Çekim ve Edits akışı ilk videoyla aynı. Döngü cümlesi: "Ama her keşif aynı soruyla başlıyor: Bir gezegen kaç yaşında olabilir?"

Kaynaklar:

- NASA: "Newfound 'Baby' Planet Smashes Record for Youngest Known World"
- W. M. Keck Gözlemevi: keckobservatory.org/elias224b
- Diego Portales Üniversitesi (UDP) duyurusu
- The Astrophysical Journal Letters makalesi
- NASA Exoplanet Archive (6.300'den fazla ötegezegen)
