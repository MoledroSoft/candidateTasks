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

## Görev 3: Sunucu Yönetimi

### Görevler:
* Sunucu güvenliğini sağlamanız gerekiyor. Çözümünüz ne olur?

* Sunucu üzerinde bir SQL-Database instance kurun ve API ile bağlayın.

### Opsi̇yonel Görevler:
* API ve veritabanını barındırmak için Linux tabanlı bir sunucu (örn. Ubuntu) kurun.

* Kurulumdan sonra API ve veritabanına nasıl erişileceğine dair kısa bir kılavuz sağlayın.

## Görev 4: Docker Kullanarak ML Modeli Dağıtımı

### Senaryo: Yapay zeka ekibi, müşteri yorumlarının duygu analizi için eğitilmiş bir model sağladı. Sizin göreviniz bu modeli çıkarım için dağıtmaktır.

### Görevler:
* Makine öğrenimi modelini sunmak için bir Docker konteyneri oluşturun.

* Model, müşteri yorumlarını bir API uç noktası aracılığıyla girdi olarak kabul etmeli ve duyarlılık puanını ve kategorisini (olumlu/nötr/olumsuz) döndürmelidir.

### Opsi̇yonel Görevler:
* Canlı analiz sağlamak amacı ile ML konteyneriyle iletişim kuran API için ikinci bir konteyner oluşturun.

* Kullanılan veritabanı, backend API ve ML model API dahil olmak üzere tüm çözümü Dockerize edin.
