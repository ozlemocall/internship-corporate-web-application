# Functional Scope

Bu doküman gerçek uygulamadaki ticari detayları açıklamadan, proje kapsamında geliştirilen temel fonksiyonları özetler.

## İş Yönetimi

İş kayıtları; müşteri, sorumlu personel, rol, durum, öncelik ve tarih bilgileriyle takip edilebilecek şekilde modellenmiştir.

Temel süreç:

```text
Talep
  ↓
İş Kaydı
  ↓
Personel / Rol Ataması
  ↓
Başlangıç
  ↓
İş Takibi
  ↓
Teslim
  ↓
Durum / Performans Değerlendirmesi
```

## Müşteri Yönetimi

Bir müşterinin birden fazla iş kaydıyla ilişkilendirilebilmesi için ilişkisel veri modeli kullanılmıştır.

## Personel ve Rol Yönetimi

Personel ve rol ilişkileri, aynı personelin farklı görevlerde çalışabilmesini destekleyecek şekilde tasarlanmıştır.

## Müşteri Görünümü

Müşteri tarafında operasyonel olarak gerekli olmayan iç bilgilerin gösterilmemesi ve iş durumunun anlaşılır biçimde sunulması hedeflenmiştir.

## Performans

İşlerin teslim zamanı ve durum bilgileri performans değerlendirmesinde kullanılan temel veri alanları arasında yer almaktadır.

Ticari uygulamaya özgü puanlama ve ağırlıklandırma kuralları paylaşılmamıştır.
