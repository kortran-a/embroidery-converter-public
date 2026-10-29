# Değişiklik günlüğü

Bu proje [Semantic Versioning](https://semver.org/) kullanır.

## [0.1.0] — İlk herkese açık sürüm

- Görsel/metin → nakış dosyası (.dst/.pes) dönüştürme işlem hattı
  (otomatik renk/bölge/dolgu planlama, benzerlik ölçümü, oto-ayar arama).
- Masaüstü arayüzü (PySide6): fotoğraf sepeti + kırpma, canlı katman
  düzenleme panosu, kıyafet kalıbı yerleşim rehberi, 3D kıyafet önizleme,
  nokta nokta dikiş editörü.
- Kurumsal/sade görsel tasarım sistemi (`theme.py`) + tutarlı çizgi ikon
  seti (`icons.py`).
- Linux ve Windows için tek-dosya (onefile) yürütülebilir paketleme.
- 460+ otomatik test (pytest), GitHub Actions ile her push'ta çalışır.
