# Embroidery Converter

Bir fotoğrafı ya da metni, nakış makinenizin okuyabileceği bir dikiş
dosyasına (**.dst** / **.pes**) otomatik olarak çeviren, sade ve
profesyonel görünümlü bir masaüstü uygulaması.

Yalnızca bir "görsel → anahat" çevirici değildir: ürettiği dikiş planını
fiziksel olarak **simüle eder**, kaynak görselle **karşılaştırıp puanlar**
ve dikiş bütçesine sığan en benzer sonucu otomatik olarak seçer.

![Ana pencere](docs/screenshots/ana-pencere.png)

## İndir

[Releases](../../releases) sayfasından işletim sisteminize uygun tek
dosyayı indirin — başka kuruluma gerek yok, Python ya da başka bir
bağımlılık kurmanıza gerek yok:

- **Linux**: `EmbroideryConverter-linux-x86_64` — indirin,
  `chmod +x EmbroideryConverter-linux-x86_64` yapıp çalıştırın.
- **Windows**: `EmbroideryConverter-windows-x86_64.exe` — indirin, çift
  tıklayıp çalıştırın.

> Not: tek-dosya paket ilk açılışta biraz yavaş başlayabilir (kendini
> geçici bir klasöre açar) — bu normaldir, sonraki açılışlar daha hızlıdır.

## Öne çıkan özellikler

- **Görselden nakışa** — fotoğraf/logo yükle, otomatik renk azaltma +
  bölge/dolgu planlaması ile dikiş dosyası üret.
- **Metin ve monogram** — düz yazı, dairesel rozet yerleşimi ya da klasik
  3 harfli monogram; birden fazla hazır font + kendi `.ttf` dosyanı kullanma.
- **Canlı katman düzenleme** — birden fazla görseli/katmanı sürükle,
  boyutlandır, döndür; sıralamayı değiştir.

  ![Nokta nokta düzenleyici](docs/screenshots/nokta-editoru.png)

- **Kırpma araçları** — dikdörtgen, poligon ve serbest-çizim kırpma,
  her zaman geri alınabilir (orijinal görsel hiç bozulmaz).
- **Kıyafet kalıbı yerleşim rehberi** — tasarımını gömlek/tişört gibi
  yaygın kalıpların neresine koyacağını görsel olarak planla.
- **3D kıyafet önizleme** — son dikişi gerçek bir kumaş yüzeyine sarıp
  birkaç açıdan render et.
- **Nokta nokta dikiş editörü** — üretilen dikişi tek tek düzenle, elle
  şekil çiz (dolgu/satin/düz dikiş), geri al/yinele ile güvenle oyna.
- **Otomatik ayar arama** — benzerlik ölçütüne göre birden fazla aday
  yapılandırma dener, dikiş bütçesine sığan en iyisini seçer.
- **Kalite raporu** — örtme, yoğunluk, iplik uzunluğu, tahmini dikiş
  süresi gibi ölçülebilir bir rapor üretir.
- **Çoklu format** — `.dst` ve `.pes`.

### Örnekler

| Girdi | Sonuç (simülasyon) |
|---|---|
| Basit bir çiçek motifi | ![çiçek nakış simülasyonu](examples/ornek_cicek.simulasyon.png) |
| "ABC" monogram | ![monogram nakış simülasyonu](examples/ornek_monogram.simulasyon.png) |

Üretilen tüm dosyalar (`.dst`, `.pes`, önizleme, kalite raporu) `examples/`
klasöründe bulunur.

## Kullanım

1. Sol üstten **görsel** ya da **metin/monogram** girdisini seçin.
2. Kasnak boyutunu, renk sayısını ve kumaşı ayarlayın (varsayılanlar çoğu
   kullanım için yeterlidir).
3. **Dönüştür**'e basın; sağ paneldeki "Dönüştürme sonucu" sekmesinde
   önizleme ve günlüğü izleyin.
4. Beğendiyseniz **İndir/Kaydet** ile `.dst`/`.pes` dosyasını kaydedin,
   isterseniz **Nokta nokta düzenle** ile son rötuşları yapın.

## Sorun bildirimi / istek

Bu depo yalnızca hazır programı dağıtmak için kullanılır (kaynak kodu
kapalıdır). Hata bildirimi ya da özellik isteği için [Issues](../../issues)
sekmesini kullanabilirsiniz.

## Lisans

Bu yazılım **ücretsiz kullanım ve dağıtım** için açıktır, ancak
**yazılımın kendisinin satılması/ticarileştirilmesi yasaktır**. Yazılımı
kullanarak ürettiğiniz çıktıları (nakış dosyaları, fiziksel ürünler) ise
**hiçbir kısıtlama olmadan ticari olarak satabilirsiniz**. Tam metin için
[LICENSE](LICENSE) dosyasına bakın. Üçüncü taraf font/veri lisansları için
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
