# 💵 Türkçe Rap Sample Arşivi

Türkçe rap müziğinde kullanılan sample'ların ve orijinal kaynaklarının derlendiği, topluluk odaklı açık kaynaklı arşiv. Tüm veriler [web arayüzünde](https://kce.wtf/turkish-rap-sample-archive/) dinamik olarak listelenmektedir.

## 🤷🏻 Amaç

Forum ve interaktif sözlüklerin boklu, düzensiz, güvensiz ve şımarık yapısından kurtulmak.

---

## ✨ Katkıda Bulunmak

### Yöntem A: Issues (Kolay)
GitHub bilgisi gerektirmez. **Issues → New Issue** ile sanatçı, şarkı ve sample bilgilerini bildirin, author'un gönülsüzce eklemesini sağlayın.

### Yöntem B: Pull Request (Doğrudan)

1. [Data Generator](https://kce.wtf/turkish-rap-sample-archive-data-generator/) aracını açın
2. Formu doldurun — sağda gerçek zamanlı JSON önizlemesi görünür
3. **JSON İndir** ile güncel `data.json`'ı indirin
4. Bu repodaki `data.json` dosyasını açın, sağ üstteki kalem ikonuyla düzenleyin
5. İndirdiğiniz dosyanın içeriğiyle tamamen değiştirin
6. **Pull Request** [açın](https://github.com/kadircanersahin/turkish-rap-sample-archive/pulls)

> Generator aracı mevcut arşiv verisini otomatik çeker; duplicate kontrolü ve format doğrulaması yapar.

---

## 📐 JSON Yapısı 😎🤏😳🕶🤏

Her kayıt tek bir sample ilişkisini temsil eder. Bir şarkıda birden fazla sample varsa her biri ayrı satır olarak girilir.

```json
{
  "id": "sagopa-kajmer-iskeletler-george-winston-colors-dance",
  "artist": "Sagopa Kajmer",
  "song": "İskeletler Diyarında Bir Et Parçası",
  "sample_artist": "George Winston",
  "sample_track": "Colors Dance",
  "type": "sample",
  "category": "melody",
  "tags": "Sagopa Kajmer, Bir Pesimistin Gözyaşları, BPG, 2003, piano",
  "see_also": "Yunus Özyavuz, Dj Mic Check, Silahsız Kuvvet"
}
```

| Alan | Zorunlu | Açıklama |
|---|---|---|
| `id` | ✓ | `artist-song-sample_artist-sample_track` slug formatında, benzersiz |
| `artist` | ✓ | Sample kullanan sanatçı |
| `song` | ✓ | Sample kullanan şarkı |
| `sample_artist` | ✓ | Orijinal kaynak sanatçı |
| `sample_track` | ✓ | Orijinal kaynak şarkı |
| `type` | ✓ | `sample`, `interpolation`, `remix`, `cover` |
| `category` | ✓ | `melody`, `drums`, `vocal`, `bass`, `fx`, `other` |
| `tags` | — | Virgülle ayrılmış arama etiketleri |
| `see_also` | — | İlgili isimler veya alternatif aramalar, virgülle ayrılmış |

`tags` ve `see_also` array değil, **virgülle ayrılmış string** olmalıdır.
