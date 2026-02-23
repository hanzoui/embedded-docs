> Bu belge yapay zeka tarafından oluşturulmuştur. Herhangi bir hata bulursanız veya iyileştirme önerileriniz varsa, katkıda bulunmaktan çekinmeyin! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/LoadTrainingDataset/tr.md)

Bu düğüm, daha önce diske kaydedilmiş kodlanmış bir eğitim veri kümesini yükler. Hanzo Studio çıktı dizini içinde belirtilen bir klasördeki tüm veri parçası dosyalarını arar ve okur, ardından eğitim iş akışlarında kullanılmak üzere birleştirilmiş gizli vektörleri ve koşullandırma verilerini döndürür.

## Girdiler

| Parametre | Veri Türü | Zorunlu | Aralık | Açıklama |
|-----------|-----------|----------|-------|-------------|
| `folder_name` | STRING | Hayır | N/A | Kaydedilmiş veri kümesini içeren klasörün adı. Hanzo Studio çıktı dizini içinde bulunur (varsayılan: "training_dataset"). |

## Çıktılar

| Çıktı Adı | Veri Türü | Açıklama |
|-------------|-----------|-------------|
| `latents` | LATENT | Her bir sözlüğün bir tensör içeren `"samples"` anahtarına sahip olduğu, gizli vektör sözlüklerinin bir listesi. |
| `conditioning` | CONDITIONING | Her bir iç listenin, karşılık gelen bir örnek için koşullandırma verisi içerdiği, koşullandırma listelerinin bir listesi. |