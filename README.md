🏥 Hastane Yönetim Sistemi (Hospital Management System)

C# Windows Form ve MSSQL veritabanı altyapısı ile geliştirilmiş, çok kullanıcılı bir hastane otomasyon sistemidir. Proje, bir hastanenin temel iş akışlarını dijital ortamda yönetmek için tasarlanmıştır.

📋 Proje Genel Bakış

Bu sistem; Sekreter, Doktor ve Hasta olmak üzere 3 farklı kullanıcı panelinden oluşmaktadır. ADO.NET teknolojisi kullanılarak merkezi bir SQL bağlantı yönetimi (sqlbaglantisi.cs) ile veriler gerçek zamanlı olarak işlenmektedir.

🌟 Temel Modüller ve Özellikler

👤 Sekreter Paneli (Yönetim Merkezi)

Kayıt Yönetimi: Doktor ve Branş ekleme, silme, güncelleme (CRUD) işlemleri.

Randevu Organizasyonu: Randevu saatlerini tanımlama, randevuları listeleme ve durum güncelleme.

İletişim: Tüm personelin görebileceği sistem duyuruları oluşturma.

👨‍⚕️ Doktor Paneli

Randevu Takibi: Kendisine atanan hastaların listesini görme ve randevu detaylarını inceleme.

Profil Yönetimi: Kişisel bilgilerini güncelleme.

Duyuru Ekranı: Sekreter tarafından yayınlanan hastane içi bildirimleri izleme.

🤒 Hasta Paneli

Üyelik Sistemi: TC Kimlik No ile sisteme güvenli kayıt ve giriş.

Randevu İşlemleri: Poliklinik (Branş) ve Doktor seçimi yaparak kolayca randevu alma.

Geçmiş İzleme: Aktif randevularını ve randevu geçmişini görüntüleme.

🖼️ Uygulama Ekranları

Ana Giriş Ekranı

Sekreter Yönetim Paneli

Hasta Detay Ekranı







Doktor Giriş

Branş Yönetimi

Doktor Paneli







🗄️ Veritabanı Mimarisi (MSSQL)

Proje, ilişkisel veritabanı modeli üzerine kurulmuştur. Kullanılan temel tablolar şunlardır:

dbo.TBL_Hastalar: Hasta kişisel verileri ve giriş şifreleri.

dbo.TBL_Doktorlar: Doktor uzmanlık alanları ve bilgileri.

dbo.TBL_Randevular: Tarih, saat, branş ve doktor eşleşmeleri.

dbo.TBL_Branslar: Hastane poliklinik listesi.

dbo.TBL_Sekreter: Yetkili giriş bilgileri.

dbo.TBL_Duyurular: Sistem geneli bildirimler.

🛠️ Teknik Detaylar

Platform: .NET Framework / Windows Forms

Veritabanı: Microsoft SQL Server

Bağlantı Katmanı: ADO.NET (Merkezi sqlbaglantisi.cs sınıfı)

Kontroller: MaskedTextBox (TC/Tel), DataGridView (Listeleme), ComboBox (İlişkisel Seçim)
