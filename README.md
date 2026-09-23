# Kurumsal Web Uygulaması – Staj Projesi

> Ticari olarak kullanılan bir kurumsal web uygulamasının geliştirme sürecinde gerçekleştirilen staj çalışmasının, gizlilik korunarak hazırlanmış teknik portföy dokümantasyonu.

## Proje Hakkında

Staj sürecinde Java ve Spring Boot kullanılarak geliştirilen, kurum içindeki iş süreçlerinin ve görevlerin takip edilmesini sağlayan web tabanlı bir uygulamanın geliştirilmesinde görev aldım.

Proje; işlerin oluşturulması ve takip edilmesi, müşterilerin ve personelin yönetilmesi, görev/rol ilişkilerinin oluşturulması ve işlerin durumlarının izlenmesi gibi süreçleri tek bir sistem üzerinden yönetmeyi amaçlamaktadır.

Proje ticari kullanımda olduğu için kaynak kodu, gerçek arayüz ekran görüntüleri, müşteri/kurum bilgileri ve uygulamaya özgü yapılandırmalar bu repository'de paylaşılmamaktadır.

Bu repository yalnızca yaptığım çalışmayı ve teknik kapsamı göstermek amacıyla hazırlanmış **gizlilik uyumlu portföy dokümantasyonudur.**

## Üzerinde Çalıştığım Alanlar

### İş Takibi
- Yeni iş kayıtlarının oluşturulması ve düzenlenmesi
- İş türü, öncelik ve durum bilgilerinin yönetilmesi
- Talep, başlangıç ve teslim tarihleri gibi zaman bilgilerinin takip edilmesi
- Gecikme nedenlerinin kayıt altına alınması
- Müşteri ile ilişkili birden fazla işin yönetilebilmesi

### Personel ve Rol Yönetimi
- Personel kayıtlarının işlerle ilişkilendirilmesi
- Personel–rol ilişkilerinin yönetilmesi
- Bir personelin birden fazla rolde görev alabilmesine uygun veri modeli
- Yetki ve görünürlük ihtiyaçlarına göre farklı kullanıcı deneyimleri

### Performans Takibi
- İşlerin tamamlanma durumu ve teslim süreleri üzerinden performans takibine yönelik yapı
- İş durumlarının düzenli olarak değerlendirilmesi
- Gecikme ve teslim süreçlerinin raporlanmasına uygun veri modeli

> Uygulamanın ticari işleyişine ait özel performans formülleri ve iş kuralları paylaşılmamıştır.

### Müşteri Paneli
- Müşterilerin kendi iş süreçlerini takip edebilmesine yönelik ayrı görünüm
- İç kullanıcılar için gerekli olan bazı operasyonel bilgilerin müşteri tarafında gösterilmemesi
- İş durumunun müşteriye anlaşılır şekilde sunulması

## Teknik Yapı

| Alan | Kullanılan Teknolojiler |
|---|---|
| Backend | Java, Spring Boot |
| Web Arayüzü | Thymeleaf, HTML, CSS |
| Veri Katmanı | JPA / Hibernate, SQL |
| Proje Yönetimi | Maven |
| Mimari | Katmanlı web uygulaması |
| Temel Yaklaşım | CRUD, ilişkisel veri modeli, rol/yetki yönetimi |

## Veri Modeli

Uygulamada iş süreçlerinin yönetimi için birbirleriyle ilişkili temel varlıklar kullanılmıştır:

```text
Customer
   │
   └──────< Job >────── Personnel
                │
                └────── Role
```

`Job` yapısında iş adı, iş türü, müşteri, personel, rol, tarihler, durum, öncelik, gecikme nedeni ve açıklama gibi iş takibine yönelik bilgiler bulunmaktadır.

Bu repository'de gerçek veritabanı şeması, müşteri kayıtları veya ticari veriler paylaşılmamıştır.

## Geliştirme Yaklaşımı

Geliştirme sırasında özellikle aşağıdaki konular üzerinde çalıştım:

- Backend tarafında Spring Boot ile uygulama geliştirme
- MVC tabanlı web uygulaması yapısı
- Thymeleaf ile dinamik sayfaların oluşturulması
- Veritabanı varlıklarının modellenmesi
- Varlıklar arasındaki ilişkilerin kurulması
- CRUD işlemleri
- Kullanıcı rollerine göre bilgi görünürlüğünün düzenlenmesi
- İş durumlarının ve teslim süreçlerinin takip edilmesi
- Uygulama arayüzünün kullanıcı ihtiyaçlarına göre düzenlenmesi

## Gizlilik Notu

Bu proje ticari kullanımda olduğu için aşağıdakiler repository'ye dahil edilmemiştir:

- Kaynak kodu
- Gerçek müşteri/kurum bilgileri
- Gerçek kullanıcı kayıtları
- Uygulamaya ait ekran görüntüleri
- Ticari iş kuralları
- Gerçek veritabanı
- Şifreler, tokenlar veya erişim bilgileri
- Kuruma özel yapılandırma dosyaları

Bu repository, yalnızca **staj kapsamında üstlendiğim teknik çalışmayı ve proje kapsamını göstermek** amacıyla hazırlanmıştır.

## Kazanımlar

Bu proje sayesinde özellikle:

- Java ve Spring Boot ile backend geliştirme
- Web uygulaması mimarisi
- İlişkisel veri modelleme
- JPA/Hibernate
- Thymeleaf
- CRUD uygulamaları
- Rol ve yetki mantığı
- İş takip sistemlerinin tasarlanması
- Ticari bir yazılım projesinde geliştirme süreçleri

konularında deneyim kazandım.
