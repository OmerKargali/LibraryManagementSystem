# 📚 Library Management System

# Java Tabanlı, Tasarım Desenleri ile Güçlendirilmiş Kütüphane Otomasyonu

---

# 🧩 Proje Hakkında

**Library Management System**, Yazılım Mimarisi ve Tasarımı dersi kapsamında geliştirilmiş; **nesne yönelimli programlama ilkelerini**, **katmanlı mimariyi** ve **modern yazılım tasarım desenlerini** merkeze alan kapsamlı bir kütüphane otomasyon sistemidir. Proje, **Java** programlama dili kullanılarak geliştirilmiş olup masaüstü ortamda çalışan **Java Swing tabanlı grafiksel kullanıcı arayüzü (GUI)** ile kullanıcı etkileşimini sağlamaktadır.

Sistem; **kullanıcı deneyimi**, **kod sürdürülebilirliği** ve **genişletilebilirlik** hedeflenerek tasarlanmış, gerçek bir kütüphane ortamında karşılaşılabilecek tüm temel süreçleri kapsayacak şekilde modellenmiştir.

---

# 🏗️ Mimari Yapı

Proje; **ui**, **logic** ve **models** olmak üzere üç ana katmandan oluşmaktadır:

* **UI (User Interface)**
  Kullanıcı etkileşimini sağlayan Swing tabanlı ekranları içerir. Arayüz katmanı, iş mantığından tamamen izole edilmiştir.

* **Logic (İş Mantığı)**
  Ödünç alma, iade, ceza hesaplama, kullanıcı ve kitap yönetimi gibi tüm operasyonel süreçler bu katmanda yürütülür.

* **Models (Veri Modelleri)**
  Kitap, kullanıcı, rol ve durum gibi sistem varlıklarını temsil eden sınıfları içerir.

Bu yapı sayesinde sistem **bakımı kolay**, **test edilebilir** ve **ölçeklenebilir** bir mimari sunmaktadır.

---

# 🎯 Kullanılan Tasarım Desenleri

Projede, yazılım kalitesini artırmak ve karmaşıklığı yönetmek amacıyla aşağıdaki tasarım desenleri etkin biçimde uygulanmıştır:

🔹 **Singleton Pattern**
Veritabanı bağlantısının tek bir örnek üzerinden yönetilmesini sağlar. Kaynak kullanımını optimize eder.

🔹 **Factory Pattern**
Kullanıcı nesnelerinin (Üye / Personel) rol bazlı olarak oluşturulmasını sağlar.

🔹 **Facade Pattern**
Karmaşık iş mantığını tek bir merkezden sunarak arayüz katmanının sistemle sade bir şekilde iletişim kurmasını sağlar.

🔹 **State Pattern**
Kitapların *müsait*, *ödünçte* gibi durumlara göre farklı davranışlar sergilemesini sağlar.

🔹 **Observer Pattern**
Kitap, kullanıcı ve ödünç işlemlerindeki değişikliklerin arayüzlere anlık olarak yansıtılmasını sağlar.

🔹 **Command Pattern**
Ödünç alma ve iade işlemlerinin komut nesneleri aracılığıyla yürütülmesini sağlar ve arayüz–iş mantığı bağımlılığını azaltır.

---

# 👥 Kullanıcı Rolleri ve Yetkiler

# 👨‍💼 Personel (Admin)

* Kitap ekleme, silme, güncelleme (CRUD)
* Üye yönetimi
* Ödünç kitap takibi
* Gecikme ve ceza kontrolü
* Sistem genelinde raporlama

# 👤 Üye (Member)

* Detaylı kitap arama
* Kitap stok ve durum kontrolü
* Kitap ödünç alma ve iade
* Kendi ödünç geçmişini görüntüleme
* Gecikme cezası takibi

---

# ⏱️ Ceza ve Ödünç Yönetimi

Sistem, kitapların iade tarihlerini otomatik olarak takip eder. Süresi geçen kitaplar için gecikme cezası hesaplanır ve:

* Üye profiline
* Personel kontrol ekranına

eş zamanlı olarak yansıtılır.
Personel kullanıcılar cezalardan **muaf**, üyeler için ise ceza mekanizması aktif şekilde çalışır.

---

# 🚀 Projenin Kazanımları

Bu proje ile;

✔ Tasarım desenlerinin gerçek bir sistemde nasıl uygulanacağı
✔ Katmanlı mimarinin avantajları
✔ Java Swing ile büyük ölçekli GUI geliştirme
✔ OOP prensiplerine uygun sürdürülebilir yazılım geliştirme

konularında güçlü bir deneyim kazanılmıştır.

---

# 👨‍💻 Proje Ekibi

| İsim               | Öğrenci No | GitHub                                                                |
| ------------------ | ---------- | --------------------------------------------------------------------- |
| **Arda TEKİN**     | 1230505052 | 🔗 [https://github.com/ardatekin0](https://github.com/ardatekin0)     |
| **Fatma Sude GÖK** | 1230505048 | 🔗 [https://github.com/fatmasudegok](https://github.com/fatmasudegok) |
| **Ömer KARGALI**   | 1220505069 | 🔗 [https://github.com/OmerKargali](https://github.com/OmerKargali)   |

