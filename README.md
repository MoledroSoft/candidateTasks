# Backend:
## Görev 1: API Oluşturulması ve Bakımı
### Senaryo: Şirketimizin müşteri memnuniyeti ve itibar analizini görüntülemek için web platformuna veri sunacak bir API ihtiyacı var.

### Görev: Aşağıdaki işlevlere sahip bir RESTful API oluşturun:

### Kimlik Doğrulama ve Yetkilendirme:
* JWT kullanarak kullanıcı kaydı ve oturum açma işlemlerini uygulayın.

### İşletme Yönetimi:
* İşletme varlıkları için CRUD işlemleri.
  
### Rol tabanlı erişim kontrolü: 
* Admin işletmelere ait veriler üzerinde oluşturma, okuma, güncelleme ve silme yetkinliğine sahip.
* İşletmeler yalnızca kendi verilerinin tamamını okuyabilir. Diğer işletmelerin belirli verilerini okuyabilir. 

### Veri Alma:
* Bir işletme için müşteri memnuniyeti puanları, duygu analizi sonuçları vb. verileri alın.
* Zaman aralığına, duygu kategorisine (olumlu/olumsuz/nötr) ve platforma (ör. Platfom1, platform2) göre filtrelemeli verileri alın.

### Veri Toplama Uç Noktası:
* Belirli bir işletme için toplu istatistikler yani müşteri dashboard'unun oluşturulması için gereken verilerin (ör. ortalama memnuniyet puanı, müşteri yorumlarındaki en yaygın anahtar kelimeler) bütününü döndüren bir uç nokta sağlayın.

### Teknik Gereksinimler:
* Veritabanı olarak SQL dilini kullanan araç seçilmeli.

## Görev 2: SQL Veritabanı Tasarımı ve Yönetimi

### Senaryo: Şirket, çeşitli web platformlarından toplanan yapılandırılmış verileri, yapay zeka analiz sonuçlarını ve analiz sonuçlarını depolamak için iyi tasarlanmış bir veritabanına ihtiyaç duyuyor.

### Görev: Aşağıdakileri destekleyen ilişkisel bir veritabanı şeması tasarlayın:
* Ham müşteri yorumlarının ve meta verilerinin (ör. yorum metni, yorumun yapıldığı tarih) saklanması.
* Her yorum için yapay zeka analiz sonuçlarının saklanması (örn. memnuniyet puanı, alt konu sınıfı).
* Toplu istatistiklerin (ör. haftalık memnuniyet eğilimleri, sık kullanılan alt konular).

### Şunlar için SQL komut dosyaları yazın:
* Belirli bir işletme için olumlu yorumlarda en sık geçen ilk 5 anahtar kelimeyi getirecek bir sorgu.
* Belirli bir zaman aralığında bir işletme için ortalama memnuniyet puanını hesaplayan bir sorgu.

## Görev 3: Veri Görselleştirme

### Senaryo: Bir veri tabanından çekilmiş sentiment_Result.csv adlı veri setinin görselleştirilmesi gerekmektedir.

### Görev: Veri setindeki score ve sentiment sütunlarını kullanarak aşağıdaki işlemleri gerçekleştiriniz:

### "Score" ile "Sentiment" arasındaki ilişkinin görselleştirilmesi:
* Bu ilişkiyi göstermek için grafik, çizelge veya diğer uygun görselleştirme yöntemlerini kullanınız.

### Değerlendirme Kriterleri:
* Score: Müşterilerin geri bildirimlerinde verdikleri puanlar.
* Sentiment: Müşterilerin geri bildirim metinlerine uygulanan duygu analizinin sonucu (ör. "Positive", "Neutral", "Negative").
