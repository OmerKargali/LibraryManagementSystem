LibraryManagementSystem

Yazılım Mimarisi ve Tasarımı dersi kapsamında geliştirilen bu Kütüphane Yönetim Sistemi, Java programlama dili kullanılarak nesne yönelimli prensiplere, katmanlı mimariye ve tasarım desenlerine uygun biçimde tasarlanmıştır. Proje, masaüstü ortamda çalışan Java Swing tabanlı grafiksel kullanıcı arayüzü (GUI) ile kullanıcı etkileşimini sağlamakta; arka planda ise iş mantığı (logic), veri modelleri (models) ve kullanıcı arayüzü (ui) katmanları birbirinden ayrılarak sürdürülebilir ve genişletilebilir bir yapı sunmaktadır.

Sistemin mimarisinde, kod tekrarını önlemek ve bakım maliyetini düşürmek amacıyla çeşitli tasarım desenleri etkin bir şekilde kullanılmıştır. Veritabanı bağlantı ve erişim işlemleri Singleton deseni ile tek bir merkezden yönetilerek kaynak kullanımının kontrol altında tutulması sağlanmıştır. Kullanıcı nesnelerinin (Üye / Personel) oluşturulmasında Factory deseni uygulanarak rol bazlı nesne üretimi soyutlanmıştır. Kitapların ödünç alma ve iade süreçlerinde farklı durumları (Available, Loaned vb.) yönetmek için State deseni kullanılmış; böylece kitap durumuna bağlı davranışlar merkezi ve esnek bir yapı ile kontrol altına alınmıştır. Ayrıca sistem genelinde kitap, kullanıcı ve ödünç işlemlerinde meydana gelen değişikliklerin arayüzlere otomatik olarak yansıtılması amacıyla Observer deseni uygulanmış, bu sayede veri güncellemeleri anlık ve tutarlı biçimde sağlanmıştır.

Proje, Üye (Member) ve Personel (Admin) olmak üzere iki temel kullanıcı rolü üzerine inşa edilmiştir. Personel kullanıcılar; kitap ve üye ekleme, silme ve güncelleme (CRUD) işlemlerini gerçekleştirebilmekte, sistemdeki tüm ödünç alma işlemlerini ve gecikme cezalarını takip edebilmektedir. Üyeler ise kütüphane kataloğu üzerinden detaylı kitap araması yapabilmekte, kitapların stok ve müsaitlik durumlarını görüntüleyebilmekte, kendi ödünç aldıkları kitapları, iade tarihlerini ve varsa gecikme cezalarını sistem üzerinden takip edebilmektedir. Ödünç süresi aşımı durumunda sistem otomatik olarak ceza hesaplaması yapmakta ve bu bilgi hem kullanıcı profiline hem de yönetici ekranına yansıtılmaktadır.

Komutların kullanıcı arayüzünden bağımsız şekilde çalıştırılabilmesi için Command deseni kullanılmış; ödünç alma ve iade işlemleri komut nesneleri aracılığıyla gerçekleştirilmiştir. Bu yaklaşım, arayüz ile iş mantığı arasındaki bağımlılığı azaltarak sistemin test edilebilirliğini ve genişletilebilirliğini artırmıştır. Tüm bu yapı, Facade deseni ile birleştirilerek arayüz katmanının karmaşık iş mantığına doğrudan erişimi engellenmiş ve sistem tek bir merkezden kontrol edilir hâle getirilmiştir.

Sonuç olarak bu proje; nesne yönelimli programlama ilkelerine uygun, tasarım desenleriyle güçlendirilmiş, modüler, okunabilir ve geliştirilmeye açık bir kütüphane otomasyon sistemi sunmaktadır. Gerçek hayattaki kütüphane süreçlerini temel alan bu yapı, akademik gereksinimlerin yanı sıra pratik yazılım mimarisi yaklaşımlarını da başarıyla yansıtmaktadır.

Proje Ekibi

Bu proje aşağıdaki ekip üyeleri tarafından geliştirilmiştir:

Arda TEKİN – 1230505052
GitHub: https://github.com/ardatekin0

Fatma Sude GÖK – 1230505048
GitHub: https://github.com/fatmasudegok

Ömer KARGALI – 1220505069
GitHub: https://github.com/OmerKargali
