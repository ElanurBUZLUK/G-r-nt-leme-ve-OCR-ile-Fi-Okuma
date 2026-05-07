# Görüntü İşleme ve OCR ile Fiş Okuma

Bu proje, market fişlerinin fotoğraflarından otomatik olarak veri çıkarmak için hazırlanmış bir Jupyter Notebook çalışmasıdır. OpenCV tabanlı görüntü ön işleme, EasyOCR metin tanıma ve düzenli ifadeler (regex) ile fiş üzerindeki önemli alanlar tespit edilip yapılandırılmış hâle getirilir.

## Özellikler

- Market adı, adres, vergi no, fiş/belge no
- Tarih ve saat bilgisi
- Ürün satırları ve ara toplam
- KDV kırılımları (%1, %8, %18) ve toplam KDV
- Genel toplam, ödeme türü, para üstü, kasiyer
- WhatsApp / fotoğraf kaynaklı rotasyon problemlerini çözmek için çoklu ön işleme kombinasyonları
- Sonuçları DataFrame ve JSON olarak kaydetme

## Dosya

- `Görüntü_İşleme_ve_OCR_ile_Fİş_Okuma.ipynb` : Projenin çalışma mantığını ve örnek adımları içeren ana notebook.

## Kurulum

1. Python ortamı oluşturun veya Google Colab kullanın.
2. Gerekli paketleri yükleyin:

```bash
pip install easyocr opencv-python-headless pandas matplotlib gdown
```

## Kullanım

1. `Görüntü_İşleme_ve_OCR_ile_Fİş_Okuma.ipynb` dosyasını açın.
2. Gerekli kütüphaneleri içe aktarın ve proje dizinlerini tanımlayın.
3. Fiş görsellerini işleyin.
4. OCR çıktısını regex ile analiz edin ve yapılandırılmış tablo/JSON formatında dışa aktarın.

## Notlar

- Notebook, farklı görsel kalite ve döndürme durumları için 4 yön × 4 ön işleme kombinasyonunu deneyerek en iyi OCR adayını seçer.
- Çıkarılan veriler, daha sonra muhasebe veya raporlama için kolayca kullanılabilir.

## Lisans

Bu depoda açık kaynak lisansı belirtilmemiştir. Kendi kullanımınıza göre lisans ekleyebilirsiniz.
