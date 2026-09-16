# 🎬 Netflix Content Data Analysis & Exploratory Data Analysis (EDA)

Bu proje, Netflix kataloğunda bulunan film ve dizilerin veri temizleme, değişken mühendisliği (feature engineering), veri görselleştirme ve keşifsel veri analizi (EDA) süreçlerini içermektedir. 

Projenin temel amacı, platformdaki içerik dağılımını, üretim odağındaki ülkeleri ve veri yapısını sistemli, adım adım ve görsel bir analitik yaklaşımla incelemektir.

---

## 📌 Proje Özeti & Öne Çıkan Bulgular

* **İçerik Dağılımı:** Netflix kataloğundaki içeriklerin **%69.6'sı Film (6,131 adet)**, **%30.4'ü Dizi / TV Show (2,676 adet)** olarak tespit edilmiştir. Katalogda film sayısı dizilerin yaklaşık 2.3 katıdır.

<img width="863" height="390" alt="icerikdagilimi" src="https://github.com/user-attachments/assets/9a73968d-abb9-4976-b90d-2cb0aac3f141" />

* **En Çok İçerik Üreten İlk 10 Ülke:** Üretim hacminde **ABD** açık ara lider konumdadır. ABD'yi **Hindistan** ve **İngiltere (UK)** takip etmektedir. Hindistan'daki içeriklerin neredeyse tamamına yakınının film odaklı olması dikkat çekici bir bulgudur.

<img width="770" height="474" alt="ulkeiceriksayisi" src="https://github.com/user-attachments/assets/f4a723a0-16d5-4754-a2d9-bb5c17d46dea" />


* **Veri Kalitesi & Temizleme:** 
  * Toplam 8,807 satırlık veri setinde mükerrer (duplicate) kayıt bulunmamaktadır.
  * Eksik değerler analiz edilmiş; `director` (%29.9), `cast` (%9.4) ve `country` (%9.4) sütunlarındaki eksik veri yapıları incelenerek veri bütünlüğü korunmuştur.
* **Tarih & Değişken Mühendisliği:**
  * `date_added` metin sütunu `datetime` veri tipine dönüştürülmüştür.
  * İçeriklerin platforma eklendiği yıl (`added_year`), ay (`added_month`) ve gün (`added_day_name`) bilgileri türetilmiştir.
  * `duration` sütunundan filmler için dakika cinsinden süre (`movie_duration`), diziler için sezon sayısı (`season_count`) ayrıştırılmıştır.

---

## 🛠️ Kullanılan Teknolojiler ve Kütüphaneler

* **Programlama Dili:** Python 3.x
* **Veri Analizi & İşleme:** `pandas`, `numpy`
* **Veri Görselleştirme:** `matplotlib`, `seaborn`
* **Geliştirme Ortamı:** Jupyter Notebook / VS Code

---

## 📂 Proje Yapısı

* `netflix_titles.csv` - Orijinal Netflix veri seti
* `netflix_analiz.ipynb` - Veri temizleme, görselleştirme ve EDA notebook'u
* `README.md` - Proje dokümantasyonu

---

👤 **Hazırlayan:** [Ramazan Eroğlu](https://github.com/IE-RamazanEroglu)
