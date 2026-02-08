# UML_School_Project
Modeling a digital content platform similar to Netflix using UML diagrams.
# Nesneye Yönelik Sistem Analizi: Dijital İçerik Platformu (Netflix Modeli)

Bu proje, okul dersim kapsamında; karmaşık sistemleri analiz etme, soyutlama (abstraction) ve nesneye yönelik programlama (OOP) prensiplerini uygulama amacıyla geliştirilmiş bir **UML Modelleme** çalışmasıdır.

## 🎯 Proje Özeti
Bu çalışma, Netflix benzeri bir dijital içerik platformunun mimarisini ele alır. Projenin ana odak noktası, bir sistemin kullanıcı, yönetici ve arka plan yönetim süreçleri arasındaki mantıksal bağları doğru bir şekilde kurgulamaktır.

## 🧠 Nesneye Yönelik Yaklaşım ve Soyutlama
Proje geliştirilirken aşağıdaki OOP prensipleri temel alınmıştır:

*   **Soyutlama (Abstraction):** `İçerik` sınıfı soyut (abstract) olarak tasarlanmış; Film ve Dizi gibi somut sınıflar bu temelden türetilmiştir.
*   **Kalıtım (Inheritance):** `Yönetici` sınıfı, `Kullanıcı` sınıfından miras alarak kod tekrarı önlenmiş ve yetki seviyeleri netleştirilmiştir.
*   **Güçlü İçerme (Composition):** `Kullanıcı` ve `Profil` arasındaki ilişki, profilin kullanıcı olmadan var olamayacağı mantığı üzerine kurulmuştur.
*   **İçerme (Aggregation):** `İzleme Listesi` ve `İçerik` arasındaki ilişki, liste silinse dahi içeriğin sistemde kalmaya devam edeceği mantığıyla tasarlanmıştır.

---

## 📊 Sistem Diyagramları

### 1. Sınıf Diyagramı (Class Diagram)
Sistemin veri yapısını, niteliklerini ve sınıflar arası hiyerarşiyi gösterir.
- **Kritik Sınıflar:** Kullanıcı, Yönetici, İçerik (Abstract), Film, Dizi, Profil, İzleme Listesi, Ödeme.

![Sınıf Diyagramı](Diagram-Images/Class_Diagram.jpg)

### 2. Kullanım Durumu Diyagramı (Use Case Diagram)
Sistemin fonksiyonel gereksinimlerini aktör bazlı olarak özetler.
- **Aktörler:** Kullanıcı (İçerik izleme, abonelik), Yönetici (İçerik/Kullanıcı yönetimi), Yönetim Sistemi (Otomatik ödeme, yedekleme).

![Use Case Diyagramı](Diagram-Images/UseCase_Diagram.jpg)

### 3. Nesne Diyagramı (Object Diagram)
Sistemin belirli bir andaki somut çalışma durumunu (örnek senaryo) gösterir.
- **Senaryo:** "Kullanıcı_1" adlı üyenin aktif bir abonelik üzerinden "Inception" filmini izleme ve favorilerine ekleme süreci modellenmiştir.

![Nesne Diyagramı](Diagram-Images/Object_diagram.jpg)

### 4. Bileşen Diyagramı (Component Diagram)
Sistemin fiziksel ve mantıksal mimarisini modüler yapıda sunar.
- **Modüller:** Front-End (Kullanıcı Uygulaması/Yönetici Paneli), Back-End (Yönetim Çekirdeği), İçerik ve Oynatma İşlemleri, Finans Modülü.

![Bileşen Diyagramı](Diagram-Images/compoment_Diagram.jpg)

---

## ⚙️ Sistemin İşleyişi (Teknik Detaylar)

1.  **Kullanıcı Perspektifi:** Kayıt, giriş, çoklu profil oluşturma, içerik filtreleme, izleme listesi yönetimi ve çevrim içi ödeme süreçlerini kapsar.
2.  **Yönetici Perspektifi:** Standart kullanıcı yetkilerine ek olarak; içerik ekleme/silme, kategori yönetimi ve kullanıcı denetimi gibi idari yetkileri içerir.
3.  **Yönetim Sistemi (Arka Plan):** İnsan müdahalesi gerektirmeyen; ödeme doğrulama, sistem bakımı, yedekleme ve raporlama gibi kritik süreçleri otonom olarak yürütür.

---

## 📁 Proje Yapısı
- **Diagram-Images/:** Tüm diyagramların görsel (JPEG/PNG) dosyaları.
- **Source-Files/:** Diyagramların düzenlenebilir orijinal çizim dosyaları.

---
## 👩‍💻 Geliştirici

**Seyma Tezel** - [GitHub](https://github.com/seymatezel) / [LinkedIn](https://www.linkedin.com/in/seymatezel) 
*Not: Bu proje bir üniversite grup ödevi kapsamında bireysel tasarlanmış ve tüm mimarisi bizzat kurgulanmıştır.*
