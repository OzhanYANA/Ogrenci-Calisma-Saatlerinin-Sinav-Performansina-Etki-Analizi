# Öğrenci Çalışma Saatlerinin Sınav Performansına Etki Analizi 

[![TR](https://img.shields.io/badge/Lang-TR-red.svg)](#türkçe) [![EN](https://img.shields.io/badge/Lang-EN-blue.svg)](#english)

---

## 🇹🇷 Türkçe

### Proje Hakkında
Bu proje, BİL 3013 Veri Madenciliğine Giriş dersi kapsamında gerçekleştirilmiş bir ilişki analizi ve tahminleme çalışmasıdır. Temel amaç, BİL 1016 Bilgisayar Bilimlerine Giriş II dersini alan öğrencilerin haftalık ders dışı çalışma süreleri ile sınav başarı puanları arasındaki ilişkiyi incelemek ve farklı çalışma sürelerine göre başarı tahminleri yapabilmektir.

**Hazırlayan:** Özhan YANA

### Veri Toplama Süreci
Bu projede hazır bir veri seti kullanılmamış; veriler tamamen **özgün olarak ekibimiz tarafından toplanmıştır**. 
- Dersi alan **12 öğrenciye** Google Forms üzerinden anket uygulanmıştır.
- Öğrencilerin dersi alma tekrar sayıları, ders dışı çalışma saatleri ve vize notları birincil elden derlenerek analiz edilebilir hale getirilmiştir.

### Kullanılan Modeller ve Yöntemler
Çalışma süresi ile sınav notu arasındaki ilişkiyi modellemek için 3 farklı regresyon algoritması kullanılmıştır:
1. **Lineer Regresyon (Linear Regression)**
2. **Polinom Regresyon (Polynomial Regression)**
3. **Karar Ağacı Regresyonu (Decision Tree Regressor)**

### Bulgular ve Sonuç
- Yapılan korelasyon analizinde, ders dışı çalışma süresi ile sınav puanı arasında **zayıf pozitif bir ilişki (r = 0.1171)** bulunmuştur.
- Modellerin performansları (R² ve MSE metrikleri) karşılaştırıldığında, en yüksek başarıyı **R² = 0.0447** skoru ile **Polinom Regresyon** ve **Karar Ağacı** modelleri göstermiştir.
- Haftada fazladan 1 saatlik ek çalışmanın, sınav puanını ortalama **4.27 puan** artırma eğiliminde olduğu gözlemlenmiştir.
- Sınırlı veri boyutu (12 kişi) ve düşük korelasyon, sınav başarısının sadece çalışma saatine bağlı olmadığını; derse katılım veya önceki altyapı gibi diğer faktörlerin de modele dahil edilmesi gerektiğini göstermektedir.

### Dosya Yapısı
- [**VeriMadenciligiOdeviKod.ipynb**](./VeriMadenciligiOdeviKod.ipynb): Veri analizi, görselleştirmeler ve regresyon modellerinin kurulup karşılaştırıldığı Python Notebook dosyası.
- [**BİL 3013 Veri Madenciliğine Giriş 2.docx**](./BİL%203013%20Veri%20Madenciliğine%20Giriş%202.docx): Veri toplama sürecini, analiz bulgularını ve güncel model çıktılarını detaylandıran proje raporu.
- [**Bil-1016-Veriler.csv**](./Bil-1016-Veriler.csv): Anket yoluyla kendi topladığımız 12 satırlık ham veri seti.
- [**E-Tablo-Linki.txt**](./E-Tablo-Linki.txt): Verilerin toplandığı Google Forms ve yanıtların tutulduğu Google Sheets bağlantılarını içeren metin belgesi.

---

## 🇬🇧 English

### About the Project
This project is a correlation analysis and prediction study developed for the Introduction to Data Mining course. The main objective is to examine the relationship between students' weekly extracurricular study hours and their exam scores in the Introduction to Computer Science II course, and to predict exam grades based on different study durations.

**Author:** Özhan YANA

### Data Collection
No pre-existing dataset was used in this project; the data was **uniquely collected by our team**.
- A Google Forms survey was conducted with **12 students** taking the course.
- Data regarding the number of course retakes, extracurricular study hours, and midterm grades were gathered first-hand for analysis.

### Models and Methodology
Three different regression algorithms were used to model the relationship between study duration and exam scores:
1. **Linear Regression**
2. **Polynomial Regression**
3. **Decision Tree Regressor**

### Findings and Conclusion
- The correlation analysis revealed a **weak positive relationship (r = 0.1171)** between extracurricular study time and exam scores.
- When comparing the performance of the models (R² and MSE metrics), the **Polynomial Regression** and **Decision Tree** models achieved the highest success with an **R² score of 0.0447**.
- It was observed that 1 hour of additional study per week tends to increase the exam score by an average of **4.27 points**.
- The limited dataset size (12 records) and low correlation indicate that exam success does not depend solely on study hours; other factors such as class attendance or prior foundational knowledge should be included in future models.

### Repository Structure
- [**VeriMadenciligiOdeviKod.ipynb**](./VeriMadenciligiOdeviKod.ipynb): The Python Notebook containing data analysis, visualizations, and the implementation/comparison of regression models.
- [**BİL 3013 Veri Madenciliğine Giriş 2.docx**](./BİL%203013%20Veri%20Madenciliğine%20Giriş%202.docx): The project report detailing the data collection process, analysis findings, and updated model outputs.
- [**Bil-1016-Veriler.csv**](./Bil-1016-Veriler.csv): The raw dataset of 12 instances collected uniquely through our survey.
- [**E-Tablo-Linki.txt**](./E-Tablo-Linki.txt): Text file containing the links to the Google Forms survey and the Google Sheets where the responses were recorded.
