> Bu belge yapay zeka tarafından oluşturulmuştur. Herhangi bir hata bulursanız veya iyileştirme önerileriniz varsa, katkıda bulunmaktan çekinmeyin! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/PrimitiveFloat/tr.md)

PrimitiveFloat düğümü, iş akışınızda kullanılabilecek bir kayan nokta sayısı değeri oluşturur. Tek bir sayısal girdi alır ve aynı değeri çıktı olarak verir, böylece Hanzo Studio işlem hattınızdaki farklı düğümler arasında kayan nokta değerlerini tanımlamanıza ve aktarmanıza olanak tanır.

## Girdiler

| Parametre | Veri Türü | Zorunlu | Aralık | Açıklama |
|-----------|-----------|----------|-------|-------------|
| `değer` | FLOAT | Evet | -sys.maxsize ile sys.maxsize arası | Çıktı olarak verilecek kayan nokta sayısı değeri |

## Çıktılar

| Çıktı Adı | Veri Türı | Açıklama |
|-------------|-----------|-------------|
| `output` | FLOAT | Girdi olarak verilen kayan nokta sayısı değeri |