# Technical Architecture

## Genel Yapı

Uygulama katmanlı bir Spring Boot web uygulaması olarak ele alınmıştır.

```text
Web Browser
    │
    ▼
Thymeleaf Views
    │
    ▼
Spring Boot Application
    │
    ├── Controller Layer
    ├── Service / Business Logic
    └── Data Access Layer
            │
            ▼
      Relational Database
```

## Backend

Java ve Spring Boot kullanılarak HTTP isteklerinin karşılanması, iş mantığının yürütülmesi ve veri erişiminin yönetilmesi sağlanmıştır.

## View Layer

Thymeleaf kullanılarak sunucu taraflı dinamik web sayfaları oluşturulmuştur.

## Persistence

İlişkisel veri modeli JPA/Hibernate yaklaşımıyla yönetilmiştir.

## Örnek Varlık İlişkileri

```text
Customer 1 ──────── * Job
Personnel 1 ─────── * Job
Role 1 ──────────── * Job
```

Bu dokümandaki model, gerçek ticari verileri veya şirket içi özel şemayı temsil eden birebir bir kopya değildir; teknik yaklaşımı açıklayan soyut bir gösterimdir.
