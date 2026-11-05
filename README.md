# Human Brain Model — görsel kanıt arşivi

İnsan beyni bağlantı verisinden yararlanan bölgesel bir modelin, sanal bir
bedenin yürüme öğrenmesiyle birlikte incelendiği pilot çalışmanın raporları,
görselleri ve gerçek simülasyon kayıtları. Yayın tarihi: **5 Kasım 2026**.

**Bu depo yalnızca dokümantasyon ve kanıt medyası içerir. Projenin kaynak kodu,
eğitim betikleri, model ağırlıkları ve ham beyin verileri paylaşılmamıştır.**

## Düşüş ve aynı andaki bölgesel etkinlik

[![Gerçek öğrenme sırasında düşüş ve eşzamanlı etkinlik](previews/fall-activity.gif)](https://github.com/Aby0302/human-brain-model-evidence/releases/download/evidence-2026-11-05/fall-with-activity.mp4)

[Videoyu aç / indir](https://github.com/Aby0302/human-brain-model-evidence/releases/download/evidence-2026-11-05/fall-with-activity.mp4)
· [Kesintisiz 28,8 saniyelik kayıt](videos/fall-learning-raw.mp4)
· [Bütün videolar](docs/gorsel-katalog.md)

Görüntü gerçek fizik simülasyonundan alınmıştır; hareketler üretilmiş bir video
veya hazır animasyon değildir. Sağdaki eğriler, görüntüdeki bedenin **aynı
kontrol adımında ve otomatik sıfırlamadan önce** kaydedilen bölgesel E/I
etkinliğidir. Altı saniyelik klip **0,5× hızda** oynatılır; üç saniyelik
simülasyon aralığını gösterir.

## Ne gözlendi?

| İnceleme | Kapsam | Gözlem |
| --- | --- | --- |
| Ana düşüş analizi | 32 ortam, 60 ek öğrenme güncellemesi, 46.080 ortam adımı | Üç ayrı ortamda 3 düşüş; 360 bölgenin E/I etkinliği 50 Hz'de kaydedildi. |
| Görüntülü öğrenme koşusu | Ayrı bir 32 ortam / 60 güncelleme koşusu | Toplam 6 düşüş; videodaki 8 numaralı ortamda 1 düşüş. Ana analizle sayılar birleştirilmedi. |
| Son yürüme politikasının değerlendirmesi | 3 değerlendirme tohumu, 16'şar ortam, ortam başına 20 s | Toplam 960 simülasyon saniyesinde 1 düşüş; ortalama ileri hız yaklaşık 0,349 m/s, hedef 0,5 m/s. |
| İnsan EEG referansı | 20 katılımcı, yayımlanmış 962 deneme | Denge bozucu destek yüzeyi hareketine kilitli gerçek Cz EEG; robot düşüşü veya duygusal etiketli veri değil. |

Düşüş öncesinde duyusal/motor girdi alan bölgelerde etkinlik farkı gözlendi.
Düşüşten hemen sonraki keskin azalma, **yazılımın model durumunu yeniden
başlatmasından** kaynaklanır. Bu değişim korku, acı veya başka bir duygu ölçümü
olarak yorumlanamaz.

**İnsan benzeri elektriksel veya duygusal sinyal ürettiği henüz doğrulanmadı.**
Model çıktıları boyutsuz bölgesel durumlardır; insan referansı mikrovolt
cinsinden EEG'dir. Biyolojik zaman kalibrasyonu, EEG ölçüm modeli ve bağımsız
duygu etiketleri bulunmadığından sayısal insan benzerliği skoru verilmemiştir.

## Görseller ve raporlar

![360 bölgenin düşüş çevresindeki etkinliği](images/fall-activity.png)

[Ayrıntılı deney raporu](docs/deney-raporu.md)
· [Yöntem ve sınırlar](docs/yontem-ve-sinirlar.md)
· [İnsan EEG referansı](images/human-eeg-reference.png)
· [Kaynaklar](docs/kaynaklar.md)

[![Son yürüme politikasının gerçek simülasyon kaydı](previews/walking.gif)](videos/walking-trained.mp4)

[Erken ve son politika: yan yana video](videos/walking-comparison.mp4).
Bu videolar, kaydedilmiş politikaların yeniden yürütümüdür; özgün eğitim
görüntüsü değildir. Erken ve son modeller farklı eğitim bütçeleri kullandığı
için karşılaştırma, beyin bağlantı girdisinin bağımsız yararını kanıtlamaz.

## Dosya bütünlüğü ve yayın kapsamı

Seçilmiş videoların süreleri, kare sayıları ve SHA-256 kimlikleri
[medya manifestinde](metadata/media-manifest.json), sayısal özetler
[sonuç dosyasında](metadata/results.json) yer alır. Yayımlanan dosyaların
bütünlük listesi [SHA256SUMS](SHA256SUMS) dosyasındadır.

Kaynak kodu ve ağırlıklar bu yayının dışında tutulduğundan bu depo tek başına
eğitimi yeniden çalıştırmaya yetmez. [Yayın kapsamı ve paylaşım sınırı](PUBLICATION.md).
