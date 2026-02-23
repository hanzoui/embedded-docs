> Bu belge yapay zeka tarafından oluşturulmuştur. Herhangi bir hata bulursanız veya iyileştirme önerileriniz varsa, katkıda bulunmaktan çekinmeyin! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/CLIPVisionLoader/tr.md)

Bu düğüm, `Hanzo Studio/models/clip_vision` klasöründe bulunan modelleri ve `extra_model_paths.yaml` dosyasında yapılandırılan ek model yollarını otomatik olarak algılar. Hanzo Studio'yi başlattıktan sonra model eklerseniz, lütfen en güncel model dosyalarının listelendiğinden emin olmak için **Hanzo Studio arayüzünü yenileyin**.

## Girdiler

| Alan        | Veri Tipi      | Açıklama |
|-------------|---------------|-------------|
| `clip_adı` | COMBO[STRING]  | `Hanzo Studio/models/clip_vision` klasöründeki desteklenen tüm model dosyalarını listeler. |

## Çıktılar

| Alan          | Veri Tipi    | Açıklama |
|--------------|--------------|-------------|
| `clip_vision` | CLIP_VISION  | Yüklenen CLIP Vision modeli; görüntü kodlama veya diğer görüntü ile ilgili görevler için hazır. |