> Bu belge yapay zeka tarafından oluşturulmuştur. Herhangi bir hata bulursanız veya iyileştirme önerileriniz varsa, katkıda bulunmaktan çekinmeyin! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/GLIGENLoader/tr.md)

Bu düğüm, `Hanzo Studio/models/gligen` klasöründe bulunan modelleri tespit edecek ve ayrıca extra_model_paths.yaml dosyasında yapılandırılan ek model yollarından da modelleri okuyacaktır. Bazen, Hanzo Studio arayüzünün ilgili klasörden model dosyalarını okuyabilmesi için **Hanzo Studio arayüzünü yenilemeniz** gerekebilir.

`GLIGENLoader` düğümü, özel üretim modelleri olan GLIGEN modellerini yüklemek için tasarlanmıştır. Bu modellerin belirtilen yollardan alınmasını ve başlatılmasını kolaylaştırarak, onları daha sonraki üretim görevleri için hazır hale getirir.

## Girdiler

| Alan        | Comfy Veri Türü   | Açıklama                                                                           |
|-------------|-------------------|-----------------------------------------------------------------------------------|
| `gligen_adı`| `COMBO[STRING]`    | Yüklenecek GLIGEN modelinin adı. Hangi model dosyasının alınacağını ve yükleneceğini belirtir, GLIGEN modelinin başlatılması için çok önemlidir. |

## Çıktılar

| Alan     | Veri Türü | Açıklama                                                              |
|----------|-----------|-----------------------------------------------------------------------|
| `gligen` | `GLIGEN`  | Yüklenen GLIGEN modeli, üretim görevlerinde kullanılmaya hazır, belirtilen yoldan yüklenen tamamen başlatılmış modeli temsil eder. |