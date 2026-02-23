> Bu belge yapay zeka tarafından oluşturulmuştur. Herhangi bir hata bulursanız veya iyileştirme önerileriniz varsa, katkıda bulunmaktan çekinmeyin! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/CenterCropImages/tr.md)

Center Crop Images düğümü, bir görüntüyü merkezinden belirtilen bir genişlik ve yüksekliğe kırpar. Girdi görüntüsünün merkezi bölgesini hesaplar ve tanımlanan boyutlarda dikdörtgen bir alan çıkarır. İstenen kırpma boyutu görüntüden büyükse, kırpma işlemi görüntünün sınırlarıyla kısıtlanır.

## Girdiler

| Parametre | Veri Türü | Zorunlu | Aralık | Açıklama |
|-----------|-----------|----------|-------|-------------|
| `image` | IMAGE | Evet | - | Kırpılacak girdi görüntüsü. |
| `width` | INT | Hayır | 1 - 8192 | Kırpma alanının genişliği (varsayılan: 512). |
| `height` | INT | Hayır | 1 - 8192 | Kırpma alanının yüksekliği (varsayılan: 512). |

## Çıktılar

| Çıktı Adı | Veri Türü | Açıklama |
|-------------|-----------|-------------|
| `image` | IMAGE | Merkez kırpma işlemi sonucunda elde edilen görüntü. |