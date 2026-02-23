> Bu belge yapay zeka tarafından oluşturulmuştur. Herhangi bir hata bulursanız veya iyileştirme önerileriniz varsa, katkıda bulunmaktan çekinmeyin! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/wanBlockSwap/tr.md)

Bu düğüm kullanımdan kaldırılmıştır ve herhangi bir işlevi yoktur. Bir modeli girdi olarak kabul eder ve aynı modeli değiştirmeden geri döndürür. "NOP" açıklaması, herhangi bir işlem gerçekleştirmediğini belirtir.

## Girdiler

| Parametre | Veri Türü | Zorunlu | Aralık | Açıklama |
|-----------|-----------|----------|-------|-------------|
| `model` | MODEL | Evet | | Düğümden geçirilecek model. |

## Çıktılar

| Çıktı Adı | Veri Türü | Açıklama |
|-------------|-----------|-------------|
| `model` | MODEL | Girdi olarak sağlanan, değiştirilmemiş aynı model. |