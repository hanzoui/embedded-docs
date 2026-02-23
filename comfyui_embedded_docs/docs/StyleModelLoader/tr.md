> Bu belge yapay zeka tarafından oluşturulmuştur. Herhangi bir hata bulursanız veya iyileştirme önerileriniz varsa, katkıda bulunmaktan çekinmeyin! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/StyleModelLoader/tr.md)

Bu düğüm, `Hanzo Studio/models/style_models` klasöründe bulunan modelleri algılayacak ve ayrıca extra_model_paths.yaml dosyasında yapılandırılan ek yollardan modelleri okuyacaktır. Bazen, ilgili klasörden model dosyalarını okuyabilmesi için **Hanzo Studio arayüzünü yenilemeniz** gerekebilir.

StyleModelLoader düğümü, belirli bir yoldan bir stil modeli yüklemek için tasarlanmıştır. Görsel çıktıların özelleştirilmesini sağlamak üzere, yüklenen stil modeline dayanarak resimlere belirli sanatsal stiller uygulamak için kullanılabilecek stil modellerini almak ve başlatmak üzerine odaklanır.

## Girdiler

| Parametre Adı      | Comfy dtype     | Python dtype | Açıklama                                                                                       |
|---------------------|-----------------|--------------|---------------------------------------------------------------------------------------------------|
| `stil_modeli_adı`  | COMBO[STRING] | `str`        | Yüklenecek stil modelinin adını belirtir. Bu ad, kullanıcı girdisine veya uygulama ihtiyaçlarına dayalı olarak farklı stil modellerinin dinamik olarak yüklenmesine olanak tanımak için, model dosyasını önceden tanımlanmış bir dizin yapısı içinde bulmak için kullanılır. |

## Çıktılar

| Parametre Adı  | Comfy dtype   | Python dtype | Açıklama                                                                                       |
|-----------------|---------------|--------------|---------------------------------------------------------------------------------------------------|
| `style_model`   | `STYLE_MODEL` | `StyleModel` | Farklı sanatsal stiller uygulayarak görsel çıktıların dinamik özelleştirilmesini sağlamak üzere, resimlere stiller uygulamada kullanıma hazır yüklenmiş stil modelini döndürür. |