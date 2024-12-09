# Backend:
## *Görev 1*: API Oluşturulması ve Bakımı
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
