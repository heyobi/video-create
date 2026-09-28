# Fon krizi · sonsuz zoom videoları

İki sayfalık, tek dosyalık HTML aracı. Bütün çizimler Canvas 2D ile kodda üretilir. Build aracı, framework ya da npm bağımlılığı yoktur. Tek harici kaynak Google Fonts'tan "Bricolage Grotesque".

- `index.html`: Shorts/Reels çekim sayfası (9:16, 7 sahne, 50,0 saniyelik kusursuz döngü)
- `uzun/index.html`: Yatay uzun video kurgu sayfası (16:9, 10 sahne, 14 anlatım adımı)
- `gezegen/index.html` ve `gezegen/uzun/index.html`: Aynı format, ikinci video: bilinen en genç gezegen Elias 2-24 b
- `sinek/index.html` ve `sinek/uzun/index.html`: Üçüncü video: FlySoul, meyve sineği beyni Dark Souls III oynuyor

## Shorts çekim akışı (telefonda)

1. Sayfayı aç, **Animasyonu oluştur (1 tur)** düğmesine dokun. Hazırlık 50 saniye sürer; bu sırada ekranı kapatma, sekmeden çıkma.
2. Düğme **Animasyonu kaydet** olunca dokun. iPhone'da paylaşım sayfasından "Videoyu Kaydet" ile galeriye gider (`animasyon.mp4`).
3. **Çekim moduna geç (kamera)**. Kayıttan önce ön kamera büyük, dikey bir kutuda görünür; kadrajını buna göre ayarla. Kutuda kameranın tam kadrajı, kırpılmadan görünür. Kayıt başlayınca kutu sol alttaki anlatıcı köşesine küçülür. Prompter ekranın tepesindedir; "Prompter: tam metin / ipucu" ile iki görünüm arasında geçilir.
4. **Çekime başla**. 3 saniyelik geri sayım biter bitmez kayıt ve animasyon aynı anda başlar, tam 50,0 saniyede kayıt kendiliğinden durur.
5. **Kamera kaydını kaydet** ile `kamera.mp4` dosyasını galeriye al. Beğenmediysen **Tekrar çek**.

Kamera görüntüsü kırpılmadan, tam kadraj kaydedilir (ön kameradan 3:4, 1440x1920 istenir). Telefon dik tutulduğunda dosya dikey çıkar. Kadraj ve kırpma Edits'te yapılır. Kaydedilen dosya aynalı değildir; önizleme ise ön kamera alışkanlığına uygun olarak aynalı gösterilir.

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

## Video 3: FlySoul (`/sinek/`)

Konu: [heyobi/flysoul](https://github.com/heyobi/flysoul) projesi. MaleCNS v1.0 meyve sineği beyin haritasından (166.700 nöron, 125 milyon sinaps; Cell 2026) kurulan bir devre, Dark Souls III'te Iudex Gundyr ile dövüşüyor.

Bütün rakamlar projenin README'sindeki sonuç tablolarından alındı:

- Sinek yaklaşık 5.200 dövüşte 8 kez kazandı ve öğrenme eğrisi düz kaldı.
- Beynin dışında eğitilen sentetik ağ ("3b") son 1.800 dövüşün yüzde 28 ile 32'sini kazandı.

Shorts sekiz sahneli ve döngü 55,8 saniye. Hikâye şu sırayla ilerler:

1. Sinek yaklaşık 5.200 dövüşte 8 kez kazandı ve öğrenme eğrisi düz kaldı: sineğin beyni yetmedi.
2. Beynin yanına küçük bir yapay ağ eklendi. Bu ağ aynı oyun bilgisini okuyup kararı verdi ve dövüşlerin üçte birini kazandı.

Metin, zaferi getirenin eklenen ağ olduğunu açıkça söyler; bunu sineğin kendi öğrenmesi gibi anlatmaz.

Bu video, diğer iki videodan farklı olarak gerçek görüntüler de kullanır. Görüntüler `sinek/assets/` klasöründedir ve flysoul reposundan alınmıştır:

- `gundyr_dik.jpg` ve `gundyr_genis.jpg`: Aynı kaydın 17,2. saniyesinden alınmış Gundyr karesi. Oyun arayüzü dışarıda kalacak şekilde kırpıldı; sayfada renk ve kenar karartmasıyla sinematik bir görünüm veriliyor. Açılışta ve kapanışta kullanılıyor. Durağan bir kare olduğu için döngü noktasında kesme oluşmuyor.
- `v_*.jpg`: Gerçek oyun kaydının (`media/victory_3b_1x_2026-09-19.mp4`) son 8 saniyesi, saniyede 8 kare. Bu, ek ağla kazanılan dövüşün zafer anı. "Beyne bir ek" sahnesine girildiğinde baştan başlıyor ve bir kez oynuyor.
- `b_*.jpg`: FlySoul görselleştiricisinin kaydından (`media/flysoul_brain_sleep.gif`) "dreaming" (uyku tekrarı) bölümü, 21 kare. Kareler ileri geri oynatılıyor. Arka plan tam siyaha çekildi ve kenarlar yumuşatıldı; görsel eklemeli karışımla çizildiği için sahneye kenar izi bırakmadan karışıyor. Modellenen devre, gerçek MaleCNS nöron şekilleri üzerinde çiziliyor. Nöron şekilleri MaleCNS'ten alınmıştır, lisansı CC-BY.

Kareler, pencere çubuğu ve arayüz yazıları kırpılarak `ffmpeg` ile çıkarıldı.
