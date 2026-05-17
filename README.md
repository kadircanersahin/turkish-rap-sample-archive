# 🎵 Türkçe Rap Sample Arşivi

Bu proje, Türkçe rap müziğinde kullanılan sample'ların (örneklemelerin) ve orijinal kaynaklarının derlendiği, topluluk odaklı, açık kaynaklı bir arşivdir. 

Arşivdeki tüm veriler dinamik olarak [Web sayfası](https://kce.wtf/turkish-rap-sample-archive/) üzerinde listelenmektedir.

---

## 🚀 Nasıl Katkıda Bulunursunuz?

Bu arşivi birlikte büyütüyoruz! Eğer listede olmayan bir sample biliyorsanız, aşağıdaki iki yöntemden biriyle katkıda bulunabilirsiniz:

### Yöntem A: Kolay Yöntem (GitHub Bilgisi Gerektirmez)
1. Yukarıdaki sekmelerden **Issues** (Sorunlar/İstekler) kısmına gelin.
2. **New Issue** butonuna tıklayın.
3. Başlığa `Yeni Sample Önerisi` yazıp, içeriğe bildiğiniz sample'ın detaylarını (Sanatçı, Şarkı, Sample Kaynağı, Varsa Linkler) yazarak gönderin. Biz sizin yerinize arşive ekleriz!

### Yöntem B: Doğrudan Katkı (Pull Request)
Eğer GitHub kullanmayı biliyorsanız, veritabanına doğrudan ekleme yapabilirsiniz:
1. `samples.json` dosyasını açın ve sağ üstteki **Kalem (Edit)** ikonuna tıklayın (Bu işlem projeyi otomatik olarak forklayacaktır).
2. Dosyanın **en altındaki** köşeli parantezden `]` hemen önce bir virgül `,` koyarak yeni sample verinizi ekleyin.
3. Değişiklikleri kaydedip bir **Pull Request (Çekme İsteği)** oluşturun.

⚠️ **ÖNEMLİ:** JSON formatının bozulmaması için ekleme yaparken aşağıdaki şablona kesinlikle sadık kalmalısınız. Virgüllere ve tırnak işaretlerine dikkat edin.

```json
  // Örnek Şablon:
  {
    "artist": "Sagopa Kajmer",
    "song": "İskeletler Diyarında Bir Et Parçası",
    "sample_source": "George Winston - Colors Dance",
    "type": "sample",
    "category": "melody",
    "tags": "Sagopa Kajmer, Bir Pesimistin Gözyaşları, BPG, Karanlık Damlalar, Disc 2, CD 2, 2003, George Winston, Colors Dance, piano",
    "see_also": "Yunus Özyavuz, Dj Mic Check, Silahsız Kuvvet"
  }
