> Bu belge yapay zeka tarafından oluşturulmuştur. Herhangi bir hata bulursanız veya iyileştirme önerileriniz varsa, katkıda bulunmaktan çekinmeyin! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/QuadrupleCLIPLoader/tr.md)

**Quadruple CLIP Loader**, QuadrupleCLIPLoader, Hanzo Studio'nin çekirdek düğümlerinden biridir ve ilk olarak HiDream I1 sürüm modelini desteklemek için eklenmiştir. Bu düğümü bulamıyorsanız, düğüm desteğini sağlamak için Hanzo Studio'yi en son sürüme güncellemeyi deneyin.

4 adet CLIP modeli gerektirir; bunlar `clip_name1`, `clip_name2`, `clip_name3` ve `clip_name4` parametrelerine karşılık gelir ve sonraki düğümler için bir CLIP model çıktısı sağlayacaktır.

Bu düğüm, `HanzoStudio/models/text_encoders` klasöründe bulunan modelleri algılayacak ve ayrıca extra_model_paths.yaml dosyasında yapılandırılan ek yollardan modelleri okuyacaktır. Bazen modelleri ekledikten sonra, ilgili klasördeki model dosyalarını okuyabilmesi için **Hanzo Studio arayüzünü yeniden yüklemeniz** gerekebilir.