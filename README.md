# Backend:
## *Görev 1*: API'lerin Oluşturulması ve Bakımı
### Senaryo: Şirketinizin müşteri memnuniyeti ve itibar analizini görüntülemek için web platformuna veri sunacak bir API'ye ihtiyacı var.

### Görev: Aşağıdaki işlevlere sahip bir RESTful API oluşturun:

### Kimlik Doğrulama ve Yetkilendirme:
* JWT kullanarak kullanıcı kaydı ve oturum açma işlemlerini uygulayın.
* Rol tabanlı erişim kontrolü: Yöneticiler işletmeleri yönetebilir ve işletmeler yalnızca kendi verilerini görüntüleyebilir.

### İşletme Yönetimi:
* İşletme varlıkları için CRUD (Oluştur, Oku, Güncelle, Sil) işlemleri.

### Veri Alma:
* Bir işletme için müşteri memnuniyeti puanlarını, duygu analizi sonuçlarını ve diğer yapay zeka türevli içgörüleri alın.
* Zaman aralığına, duygu kategorisine (olumlu/olumsuz/nötr) ve platforma (ör. TripAdvisor, Booking.com) göre filtrelemeyi etkinleştirin.

### Veri Toplama Uç Noktası:
* Belirli bir işletme için toplu istatistikler (ör. ortalama memnuniyet puanı, müşteri yorumlarındaki en yaygın anahtar kelimeler) döndüren bir uç nokta sağlayın.

### Teknik Yığın Gereksinimleri:
* Arka uç için Node.js veya Python (Flask/FastAPI/Django) kullanın.
* Veritabanı olarak PostgreSQL kullanın.