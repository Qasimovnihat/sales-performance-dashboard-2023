# 📈 Satış Performansı Analizi (2023) — Power BI + Excel

![Power BI](https://img.shields.io/badge/Visualization-Power%20BI-yellow?style=flat-square&logo=power-bi)
![Excel](https://img.shields.io/badge/Data%20Cleaning-Excel-green?style=flat-square&logo=microsoft-excel)
![Statistics](https://img.shields.io/badge/Analysis-Statistics-blue?style=flat-square)

## 📌 Layihənin İcmalı
Bu layihə **2023-cü ilin satış məlumatlarının** Excel-də təmizlənməsi, analiz edilməsi və interaktiv Power BI paneli (dashboard) vasitəsilə vizuallaşdırılmasını əks etdirir. Əsas məqsəd satış, endirim və mənfəət göstəricilərini müxtəlif seqmentlər üzrə izləmək və endirim səviyyələrinin mənfəət marjasına təsirini statistik metodlarla qiymətləndirməkdir.

---

## 🎯 Layihənin Məqsədləri
* **KPI Kartları:** 2023-cü il üzrə ümumi satış performansını izləmək.
* **Trend Analizi:** Aylıq satış və mənfəət dinamikasını təhlil etmək.
* **Seqment Müqayisəsi:** Region, kateqoriya, kanal, ödəniş növü və müştəri tipi üzrə performansı müqayisə etmək.
* **Statistik Yoxlama:** Korrelyasiya və **P-value** testlərindən istifadə edərək endirim ilə mənfəət marjası arasındakı əlaqəni ölçmək.

---

## 🛠 Məlumatların Hazırlanması (Excel)
Məlumatların təmizlənməsi və analize hazırlanması mərhələsində görülən işlər:
* **Təmizləmə:** Təkrarlanan (duplicate) qeydlər silindi və boş (null) dəyərlər biznes məntiqinə uyğun dolduruldu.
* **Formatlaşdırma:** Yanlış daxil edilmiş dəyərlər düzəldildi və düzgün məlumat tipləri (tarix, rəqəm, faiz) tətbiq edildi.
* **Hesablanmış Sütunlar:**
    * **Ümumi Satış:** `Quantity_Sold * Unit_Price * (1 - Discount)`
    * **Ümumi Xərc:** `Quantity_Sold * Unit_Cost`
    * **Mənfəət (Profit):** `Total_Sales - Total_Cost`
    * **Mənfəət Marjası:** `Profit / Total_Sales`

---

## 📊 Power BI Dashboard (2 Səhifə)

### 1. Satış Performansı 2023
Bu səhifə biznesin ümumi vəziyyətini sürətli şəkildə qiymətləndirməyə imkan verir:
* **KPI-lar:** Ümumi Satış, Endirim Məbləği, Ümumi Mənfəət, Mənfəət Marjası, Satılan Miqdar.
* **Vizuallar:** Aylıq Satış vs Mənfəət trendi.
* **Filtrlər (Slicers):** Region, Kateqoriya, Ödəniş Üsulu, Müştəri Tipi.

### 2. Endirim və Mənfəət Analizi
Endirimlərin rentabelliyə təsirini dərindən araşdırır:
* Aylıq Satış və Orta Endirim trendi.
* Kateqoriyalar üzrə endirim payı.
* **Scatter Plot:** Endirim % və Mənfəət Marjası arasındakı əlaqə.
* **Binned Analysis:** Endirim aralıqları üzrə mənfəət marjasının dəyişməsi.

---

## 🔍 Əsas Analitik Nəticələr
* **Tərs Mütənasiblik:** Yüksək endirim dərəcələri, xüsusilə pik hədlərdə mənfəət marjasının kəskin azalmasına səbəb olur.
* **Kateqoriya Fərqləri:** Endirim paylanması kateqoriyalar üzrə fərqlidir (məsələn, "Electronics" kateqoriyasında endirim payı daha yüksəkdir).
* **Statistik Təsdiq:** Endirim və mənfəət marjası arasındakı əlaqə statistik olaraq əhəmiyyətli (p-value < 0.05) müəyyən edilmişdir.

## Report Preview
https://app.powerbi.com/view?r=eyJrIjoiZDg3ZDVmYTEtNjU0ZS00YmY2LWE0MzgtMGFiNjExYWFmODdhIiwidCI6ImZkYTYyMDk1LWI3ZGQtNGNjOS05MTIwLWZkMDYzODg5Y2Q0OCIsImMiOjl9

