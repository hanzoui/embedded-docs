> Bu belge yapay zeka tarafından oluşturulmuştur. Herhangi bir hata bulursanız veya iyileştirme önerileriniz varsa, katkıda bulunmaktan çekinmeyin! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/CheckpointLoaderSimple/tr.md)

Bu, model dosyalarını belirtilen konumlardan yükleyen ve bunları üç temel bileşene ayıran bir model yükleyici düğümüdür: ana model, metin kodlayıcı ve görüntü kodlayıcı/kod çözücü.

Bu düğüm, `Hanzo Studio/models/checkpoints` klasöründeki tüm model dosyalarını ve `extra_model_paths.yaml` dosyanızda yapılandırılan ek yolları otomatik olarak algılar.

1.  **Model Uyumluluğu**: Seçilen modelin iş akışınızla uyumlu olduğundan emin olun. Farklı model türleri (SD1.5, SDXL, Flux vb.), karşılık gelen örnekleyiciler ve diğer düğümlerle eşleştirilmelidir.
2.  **Dosya Yönetimi**: Model dosyalarını `Hanzo Studio/models/checkpoints` klasörüne yerleştirin veya `extra_model_paths.yaml` aracılığıyla diğer yolları yapılandırın.
3.  **Arayüz Yenileme**: Hanzo Studio çalışırken yeni model dosyaları eklendiyse, açılır listede yeni dosyaları görmek için tarayıcıyı yenilemeniz (Ctrl+R) gerekir.

## Girdiler

| Parametre    | Veri Türü | Girdi Türü | Varsayılan | Aralık                           | Açıklama                                                                                             |
|--------------|-----------|------------|------------|----------------------------------|------------------------------------------------------------------------------------------------------|
| `ckpt_adı`  | STRING    | Widget     | null       | checkpoints klasöründeki tüm model dosyaları | Yüklenecek kontrol noktası model dosya adını seçin; bu, sonraki görüntü oluşturma için kullanılacak AI modelini belirler |

## Çıktılar

| Çıktı Adı | Veri Türü   | Açıklama                                                                       |
|-----------|-------------|--------------------------------------------------------------------------------|
| `MODEL`   | MODEL       | Görüntü gürültü giderme oluşturumu için kullanılan ana difüzyon modeli, AI görüntü oluşturmanın çekirdek bileşeni |
| `CLIP`    | CLIP        | Metin istemlerini kodlamak için kullanılan model, metin açıklamalarını AI'nın anlayabileceği bilgiye dönüştürür |
| `VAE`     | VAE         | Görüntü kodlama ve kod çözme için kullanılan model, piksel uzayı ve gizli uzay arasında dönüşümden sorumludur |