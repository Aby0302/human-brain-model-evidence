# Kaynaklar ve atıflar

## Gerçek insan EEG referansı

- Payne, A. ve Ting, L., **Perturbation-evoked cortical responses associated
  with balance ability**. [Özgün Dryad veri kaydı](https://datadryad.org/dataset/doi:10.5061/dryad.qz612jm9x),
  DOI: 10.5061/dryad.qz612jm9x. [Zenodo aynası](https://zenodo.org/records/3898501).
  Sağlayıcı veriyi CC0 olarak yayımlar. Bu depoda ham veri dosyası yer almaz;
  yalnızca katılımcılar eşit ağırlıkla ortalanarak çizilen referans görseli vardır.
- İndirilen özgün dosyanın sağlayıcı MD5 kimliği doğrulandı:
  a3dc9824cf22d6608b0ae98d47d0c29f; 332.111.229 bayt.
  Gerçek dosya 20 katılımcı, 962 deneme, 2501 örnek ve −0,5…+2 s zaman ekseni
  içerir. Sağlayıcı açıklamasındaki 960 deneme ve −0,4 s başlangıç bilgisiyle
  fark bulunduğu için raporda incelenen dosyanın gerçek boyutları kullanıldı.

## Denge yanıtı ve yorum sınırları

- Jalilpour ve Müller-Putz (2023), denge pertürbasyonunda erken yanıt ile
  hata işlemeyi ayıran deney. [Birincil makalenin özeti](https://pubmed.ncbi.nlm.nih.gov/36921343/),
  [DOI: 10.1088/1741-2552/acc486](https://doi.org/10.1088/1741-2552/acc486).
  Erken N1 yanıtı tek başına hata farkındalığı veya duygu göstergesi olarak
  kullanılamaz.
- [MNE: EEG ileri çözümü](https://mne.tools/stable/documentation/glossary.html#term-forward-solution),
  [birimler](https://mne.tools/stable/documentation/implementation.html#internal-representation-units)
  ve [yeniden örnekleme](https://mne.tools/stable/auto_tutorials/preprocessing/30_filtering_resampling.html#resampling).
  Bölgesel model durumlarıyla kafa derisi gerilimi arasındaki ölçüm köprüsü ve
  örnekleme sınırları için resmi teknik başvuru kaynaklarıdır.

## Simülasyon ve anatomi bağlamı

- [NVIDIA Isaac Lab](https://github.com/isaac-sim/IsaacLab): bedensel öğrenme
  ve simülasyon altyapısı. Yerel deneyler release/3.0.0 kaynak sürümünü kullandı.
- [Newton](https://github.com/newton-physics/newton): fizik simülasyonu altyapısı.
- [Unitree G1](https://www.unitree.com/g1): simülasyonda temsil edilen robot bedeni.
- [Human Connectome Project](https://www.humanconnectome.org/): insan bağlantı
  verisinin proje bağlamı. Bu yayında bireysel tarama, bağlantı matrisi,
  katılımcı kimliği veya atlas dosyası dağıtılmamaktadır.

Bu kaynaklara atıf verilmesi projenin insan benzeri bilinç, duygu veya tam beyin
doğrulaması aldığı anlamına gelmez. Üçüncü tarafların yazılımları, ham veri
dosyaları ve robot varlıkları bu depoya eklenmemiştir.
