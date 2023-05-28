# Homework_Pandas.Lovers
## Homework_EDA (Stage 1)

[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1og6cvaGaytVXbDfEG2YFAhy9YhaIQPVY?usp=sharing#scrollTo=fQlFGqU0NjD-)


## DATASET : HOLIDAY PACKAGE PREDICTION
#### PREPARATION

1. PROBLEM STATEMENT

    Perusahaan traveling 'Trips & TravelCom' membuat penawaran paket liburan terbaru. Agar lebih efektif, perusahaan ingin menyelesaikan permasalahan yang ada.

    Pada tahun lalu, hanya 18% pelanggan yang membeli paket liburan yang ditawarkan.
Revenue perusahaan tidak mengalami peningkatan yang signifikan.
2. GOAL

    Untuk menaikkan convertion rate dan revenue perusahaan.

3. OBJECTIVE

    Membuat model untuk memprediksi pelanggan yang akan membeli paket liburan terbaru.

4. BUSINESS METRICS

    - Total revenue
    - convertion rate


#### LIBRARY

| Library | Keterangan |
| ------ | ------ |
| Pandas | Import Library |
| matplotlib.pyplot | Import Library |
| numpy | Import Library |
| seaborn | Import Library |
| re | Import Library |
| matplotlib.patches | Import Library |
| matplotlib | Import Library |

#### Dataset
- Travel.csv

## EDA, INSIGHT & VISUALIZATION

##### 1. Descriptive Statistics
###### HASIL OBSERVASI
Hasil Observasi Team Pandas.Lovers yaitu sebagai berikut : 
> 1. Terdapat kolom dengan tipe data yang kurang sesuai, yaitu kolom NumberOfChildrenVisiting,DurationOfPitch, NumberOfFollowups, PreferredPropertyStar, NumberOfTrips & Age yang bertipe data float sehingga nantinya harus kita rubah menjadi tipe data integer.

> 2. Terdapat 9 kolom yang memiliki missing value, yaitu kolom Age,TypeofContact, DurationOfPitch,NumberOfFollowups, PreferredPropertyStar, NumberOfTrips, NumberOfChildrenVisitin & MonthlyIncome. Teramati 9 kolom memiliki missing value,<5.1% sehingga dapat dikatagorikan masih relatif aman.

> 3. Pada kolom NumberOfTrips, terdapat nilai (max = 22) dan (min = 1 ), Sedangkan memiliki mean = 3.23 yang lebih besar dari median = 3.000. mengindikasikan data tersebar pada nilai nilai yang memiliki value yang kecil. Atau bisa disebut terdistribusi (positif skewed).

> 4. Pada kolom MonthlyIncome memiliki mean yang lebih besar dibandingkan nilai mediannya, mengindikasikan sebaran data tersebut yaitu positive skewed.

> 5. Pada kolom MonthlyIncome pun terlihat memiliki standard deviation yang sangat tinggi, yang mengartikan terdapat data data yang tersebar sangat jauh dari nilai rata rata, yang kemungkinan menandakan adanya outlier.

> 6. Tidak terdapat data yang duplikasi pada dataset ini.

> 7. Terdapat kesalahan value pada kolom Gender yaitu adanya value 'Fe Male', yang nantinya harus kita handle pada saat preprocessing data.

> 8. Pada kolom MaritalStatus, terdapat value yang memiliki arti sama yaitu value Single & Unmarried.

#### 2. Univariate Analysis
Hasil Observasi Team Pandas.Lovers yaitu sebagai berikut :

> 1. Pada kolom Age distribusi datanya hampir mendekati normal.

> 2. Pada kolom DurationOfPitch terlihat distribusinya positive skewed dimana kebanyakan frekuensi data tersebar pada nilai <20. terlihat adanya outlier pada nilai > 120, sehingga nantinya akan kita ubah distribusi nya menjadi normal pada saat preprocessing data.

> 3. Pada kolom MonthlyIncome data tersebar pada nilai 20k - 30k. dimana terdapat data outlier pada nilai >80k & < 10k. Dan sama seperti kolom DurationOfPitch nantinya akan kita ubah distribusi data nya menjadi normal pada saat melakukan preprocessing data.

> 4. Terdapat outlier pada kolom NumberOfTrips, dimana adanya nilai ekstrim yang mencapai < 19. Sehingga nanti akan kita hilangkan outliernya pada saat pre-processing.

> 5. Customer yang memiliki Occupation sebagai freelancer sangat sedikit (0,04%) jika dibandingkan dengan Occupation yang lain.

> 6. Pada kolom target / ProdTaken. Terdapat class imbalance atau ketimpangan data, dimana customer yang mengambil paket liburan (ProdTaken = 1) memiliki frekuensi dibawah <1000. sedangkan customer yang tidak mengambil paket wisata (prodtaken =0 ) berjumlah sangat dominan, sekitar 4000 customer. Sehingga ketimpangan data pada target harus diproses dengan undersampling / oversampling pada saat data preprocessing nanti.

#### 3. Multivariate Analysis
Hasil Observasi Team Pandas.Lovers yaitu sebagai berikut :

> 1. Dapat dilihat nilai korelasi pada variable target kita yaitu ProdTaken, terdapat korelasi positif walaupun lemah antara variable Passport terhadap ProdTaken yang berarti semakin tinggi nilai passport customer (1), maka semakin tinggi pula nilai ProdTaken nya atau customer yang memiliki passport lebih cenderung membeli tawaran paket dibandingkan dengan customer yang tidak memiliki passport.

> 2. Terdapat korelasi negatif antara variable Age terhadap ProdTaken dan variable MonthlyIncome terhadap ProdTaken, yang berarti semakin kecil nilai Age/MonthlyIncome-nya maka semakin besar nilai ProdTaken-nya atau customer yang berumur kecil/muda lebih cenderung membeli tawaran paket liburan dibandingkan dengan customer yang berumur tua, dan customer yang bergaji kecil cenderung membeli tawaran paket liburan dibandingkan dengan customer yang bergaji besar.

> 3. Terdapat 2 fitur yang memiliki korelasi yang cukup kuat, yaitu NumberOfPersonVisiting dan NumberOfChildrenVisiting. dimana membentuk positif korelasi. Sehingga pada proses feature selection, kita dapat mengeliminasi fitur yang redundan(mempunyai informasi serupa) agar tidak terjadi overfitting pada model machine learning nantinya.

# Terima kasih





