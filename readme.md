# KENTRAPORUM
## WebGIS Tabanlı Akıllı Şehir Raporlama Sistemi

> KentRaporum, vatandaşların altyapı sorunlarını konum bazlı bildirmesini ve yerel yönetimlerin bu verileri dinamik bir panel üzerinden yönetmesini sağlayan kapsamlı bir **WebGIS** platformudur.

---

### `ÖZELLİKLER`

* **Vatandaş Modülü**
  `Firebase Auth` ile güvenli giriş ve `Leaflet.js` entegrasyonu sayesinde harita üzerinde gerçek zamanlı sorun ihbarı

* **Dinamik Harita**
  `Firestore` verileriyle beslenen; sorun tipine ve çözüm durumuna (Beklemede/Çözüldü) göre dinamik renk değiştiren `Smart Markers` sistemi

* **Admin Dashboard**
  `Chart.js` destekli mahalle bazlı sorun yoğunluğu grafikleri ve yerel yönetimler için şeffaf veri takip mekanizması

* **Şeffaf Yönetim**
  Vatandaş ve belediye arasındaki bürokrasiyi dijitalleştirerek çözüm sürecini hızlandıran karar destek yapısı

---

### `TEKNOLOJİ YIĞINI`

```text
Frontend    :  React.js / Vue.js & Tailwind CSS
Backend     :  Firebase (Auth, Firestore, Storage)
GIS Engine  :  Leaflet.js
Analytics   :  Chart.js

graph LR
    A[Vatandaş] --> B(WebGIS Raporlama)
    B --> C{Firestore (db) }
    C --> D[Belediye/Admin Paneli]
    D --> E(Sorun Çözümü & Onay)

