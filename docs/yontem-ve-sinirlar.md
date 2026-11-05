# Yöntem ve sonuçların sınırları

## Deney düzeni

Sanal beden Unitree G1; ortam NVIDIA Isaac Lab / Newton; motor öğrenme yöntemi
PPO'dur. Beyin bağlantı verisinden yararlanan 360 bölgeli etkinlik modeli,
bedenin hareket, yerçekimi yönü ve hareket komutlarına yanıt verir. Bölgesel
özellikler motor politikasına girdi olur. Bağlantı matrisi sabittir; bu yayında
öğrenilmiş bir insan beyni veya fizyolojik eklem-bölge eşlemesi iddia edilmez.

Ana izleme koşusu ve görüntülü koşu, kısmen eğitilmiş aynı motor politikasından
başlayan ayrı öğrenme devamlarıdır. Her biri 32 ortam, 60 ek güncelleme,
46.080 ortam adımı içerir. Toplam simülasyon süresi koşu başına 921,6 s'dir;
bu, tek bedenin kesintisiz 921,6 s yürümesi anlamına gelmez.

## Kayıt ve kontroller

- Bölgesel E/I durumları 50 Hz'de, fizik ve gözlem güncellemesinden sonra,
  otomatik ortam sıfırlamasından önce yakalanmıştır.
- Gövde temasıyla sonlandırmalar ve süre dolumları ayrı sayılmıştır.
- Ana analizde her düşüşün 1 s öncesi ve 1 s sonrası alınmıştır. Kesintisiz
  ön geçmiş aranmış, yakında başka düşüş içeren pencereler dışlanmıştır.
- Başlangıca göre değişimde −1 ile −0,6 s aralığı kullanılmıştır.
- Düşmeyen kontroller tam aynı bölüm yaşında eşleştirilmiştir; olaylar önce
  ortam içinde, sonra ortamlar arasında eşit ağırlıkla ortalanmıştır.
- Video kareleri ve etkinlik örnekleri aynı kontrol adımına bağlanmıştır.
  Kısa videonun 0,5× hızı açıkça gösterilir; ham video 1× hızdadır.

Kontroller hız/duruş ve rastlantısal politika eylemleriyle eşleştirilmemiştir.
Ana üç olay bir tohum ve bir öğrenme devamına aittir. Güven aralığı, duygu
sınıflaması veya insan benzerliği skoru üretilmemiştir.

## Sıfırlama ve fiziksel toparlanma

Düşüşten sonra ortam ve bölgesel durum yeniden başlar. Üç ana olayda da
sonraki başlangıç E=I=0,1'dir. Bu yazılımsal müdahale biyolojik baskılanma,
bilinç kaybı veya darbe sonrası duygu yanıtı olarak yorumlanamaz.

Yalnızca nöral sıfırlama kaldırılarak yapılan yeniden hesaplama, gerçek beden
girdilerini kullanır; bu girdilerdeki fiziksel sıfırlama devam eder. Alternatif
bir fiziksel gelecek veya yerden kalkma hareketi hesaplanmamıştır.

## EEG ve duygu için eksik ölçüm köprüsü

Model durumları boyutsuzdur. İnsanların kafa derisi EEG'si fiziksel gerilim
ölçümüdür. Karşılaştırma için gerekçeli bir kaynak-sensör ölçüm modeli,
biyolojik zaman kalibrasyonu, aynı olay/görev tanımı, uyumlu ön işleme ve
kalibrasyondan ayrı insan verisinde değerlendirme gerekir.

50 Hz simülasyon kaydının Nyquist sınırı, simülasyon saatinde 25 Hz'dir.
Örnekleri artırarak eksik hızlı dalgalanmalar geri getirilemez. Biyolojik
zaman eşlemesi bulunmadığından daha yavaş model dalgalanmaları da doğrudan
insan EEG bantları olarak adlandırılmaz.

Duygusal benzerlik ayrıca bağımsız duygu ölçümleri ve açık bir hipotez
gerektirir. Denge bozulmasına yanıt, tek başına korku veya acı kanıtı değildir.
İnsan referansı destek yüzeyi hareketidir; gövde temasıyla aynı olay değildir.

## Dosyalarla neler denetlenebilir?

Yayımlanan dosyaların SHA-256 kimlikleri, medya süreleri, çözünürlükleri ve
kare sayıları denetlenebilir. Rapordaki özetler ve gerçek görüntüler okunabilir.
Yereldeki izler ve kaynak kodu paylaşılmadığından tam eğitim, etkinlik analizi
ve insan EEG çıkarımı bu depodan tek başına yeniden çalıştırılamaz.

Yerel ana test ortamında 91 test geçti; 7 isteğe bağlı test atlandı. Ayrı
simülasyon ortamında bu 7 testi de kapsayan 28 test geçti. Bu, iki ortam
üzerinden 98 benzersiz testtir; 91+28 bağımsız test olarak toplanmaz. Test
sonuçları yazılım ölçüm hattıyla ilgilidir, biyolojik doğrulama değildir.

[Kaynaklar](kaynaklar.md) · [Yayın kapsamı](../PUBLICATION.md)
