> Bu belge yapay zeka tarafından oluşturulmuştur. Herhangi bir hata bulursanız veya iyileştirme önerileriniz varsa, katkıda bulunmaktan çekinmeyin! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/VAESave/tr.md)

VAESave düğümü, VAE modellerini ve bunlara ait istemleri ve ek PNG bilgilerini içeren meta verileri belirtilen bir çıktı dizinine kaydetmek için tasarlanmıştır. Model durumunu ve ilişkili bilgileri bir dosyaya serileştirme işlevselliğini kapsar, böylece eğitilmiş modellerin korunmasını ve paylaşılmasını kolaylaştırır.

## Girdiler

| Parametre | Veri Türü | Açıklama |
|-----------|-------------|-------------|
| `vae`     | VAE       | Kaydedilecek VAE modeli. Serileştirilecek ve depolanacak modeli temsil ettiği için bu parametre hayati öneme sahiptir. |
| `dosyaadı_öneki` | STRING   | Modelin ve meta verilerinin altında kaydedileceği dosya adı için bir önek. Bu, modellerin düzenli bir şekilde depolanmasına ve kolayca geri getirilmesine olanak tanır. |

## Çıktılar

Bu düğümün çıktı türleri yoktur.