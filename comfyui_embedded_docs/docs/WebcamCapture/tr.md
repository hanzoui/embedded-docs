> Bu belge yapay zeka tarafından oluşturulmuştur. Herhangi bir hata bulursanız veya iyileştirme önerileriniz varsa, katkıda bulunmaktan çekinmeyin! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/WebcamCapture/tr.md)

WebcamCapture düğümü, bir web kamerası cihazından görüntü yakalar ve Hanzo Studio iş akışları içinde kullanılabilecek bir formata dönüştürür. LoadImage düğümünden türetilmiştir ve yakalama boyutları ile zamanlamayı kontrol etmek için seçenekler sağlar. Etkinleştirildiğinde, düğüm iş akışı kuyruğu her işlendiğinde yeni görüntüler yakalayabilir.

## Girdiler

| Parametre | Veri Türü | Zorunlu | Aralık | Açıklama |
|-----------|-----------|----------|-------|-------------|
| `görüntü` | WEBCAM | Evet | - | Görüntülerin yakalanacağı web kamerası giriş kaynağı |
| `genişlik` | INT | Hayır | 0 - MAX_RESOLUTION | Yakalanan görüntü için istenen genişlik (varsayılan: 0, web kameranın yerel çözünürlüğünü kullanır) |
| `yükseklik` | INT | Hayır | 0 - MAX_RESOLUTION | Yakalanan görüntü için istenen yükseklik (varsayılan: 0, web kameranın yerel çözünürlüğünü kullanır) |
| `kuyrukta_yakala` | BOOLEAN | Hayır | - | Etkinleştirildiğinde, iş akışı kuyruğu her işlendiğinde yeni bir görüntü yakalar (varsayılan: True) |

**Not:** Hem `width` hem de `height` 0 olarak ayarlandığında, düğüm web kameranın yerel çözünürlüğünü kullanır. Boyutlardan herhangi birini sıfır olmayan bir değere ayarlamak, yakalanan görüntüyü buna göre yeniden boyutlandıracaktır.

## Çıktılar

| Çıktı Adı | Veri Türü | Açıklama |
|-------------|-----------|-------------|
| `IMAGE` | IMAGE | Hanzo Studio'nin görüntü formatına dönüştürülmüş yakalanan web kamerası görüntüsü |