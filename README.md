# 🐼 Marketing Package by Pandas Lovers 🐼
## HOLIDAY PACKAGE PREDICTION

![Green and Yellow Modern Playful Tour and Travel Banner-min](https://github.com/Astryon/final_project/assets/68798868/0e13866e-cc22-4637-bba1-a34fe43bccdc)


[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1og6cvaGaytVXbDfEG2YFAhy9YhaIQPVY?usp=sharing#scrollTo=fQlFGqU0NjD-)
DATASET : [HOLIDAY PACKAGE PREDICTION](https://www.kaggle.com/datasets/susant4learning/holiday-package-purchase-prediction)

# MACHINE LEARNING MODELLING & EVALUATION

## Preparation
Melakukan Preparation pada Data : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/768be690-5659-4950-bccb-5fb94ac6a7bb)

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/1334049a-3c7d-4e87-b427-17541af48835)

## Modelling
Setelah melakukan Preparation lalu melakukan Modelling Pada Data : 

1. Medelling menggunakan KNN : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/6d334e68-4686-4248-8c84-2ce428482ed7)

2. Modelling menggunakan Decision Tree : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/5a7e296b-329b-4d52-89fe-318886f9cbd9)

3. Modelling menggunakan Random Forest Classifier : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/1d413cf0-b753-4703-983f-832545bcbec0)

4. Modelling menggunakan Ada Boost Classifier : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/0eedf664-caee-43ff-b16a-7da810de04bd)

5. Modelling menggunakan XGBoost : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/fb8b1da5-6035-4a98-b4ff-50f87985f830)

## Model Evaluation 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/8998f7cb-f275-4f36-a2aa-c1a47e33139b)

Dari Modelling data yang telah di lakukan, Karena hasil dari precision nya kurang bagus, maka kami melakukan iterasi kembali ke feature selection.

# FEATURE SELECTION (2)

1. Memanggilkembali data yang sudah di Pre-pocessing :

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/312b7231-a1ab-4e6f-8f82-5f3b3c62d10f)

2. Memilah kembali Feature yang tidak di pakai : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/ecf78b92-3e98-4a0b-a18f-6c71d9df5c29)

3. Mengecek kembali datanya : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/53146c7c-70ea-4fa0-9573-3a55c6d1247d)

4. Cek Fitur Train Set : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/29742e3e-e078-4de3-9591-cbfa260f64af)

5. Membagi Dataset menjadi 70 : 30 :

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/29286eb3-a84a-4196-8722-e88f004185c2)

6. Split data X dan Y : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/5e112379-8609-4374-bfcf-c4dfdb160792)

7. Mengecek Data pada Baris X dan Y (Train dan Test) : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/31494989-6226-4524-954e-cc31d62da56d)

8. cek precision fitur menggunakan xgboost : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/77001eb6-f723-46d6-80ef-aa75dccceefb)

Dari data yang sudah di Feature Selection yaitu walaupun hasil dari precision sudah membaik tetapi modelnya masih overfit, maka kita akan coba mendrop beberapa fitur yg tidak terlalu penting dengan cara melihat feature importance-nya.

9. Cek Feature Importancenya : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/c95dd132-b5d7-4209-81e1-991c95b67740)

10. Melakukan drop fitur yg tidak terlalu penting : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/506e1a2e-18dc-44a6-8716-fdd9a90bf58f)

11. Cek Fitur : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/4a8e58a8-07f9-47cb-aea3-0d5297869cb8)

12. Melakukan cek korelasi features untuk melihat apakah ada fitur yg redundant

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/35ef19c9-ec2e-4e01-b290-2877ce8f3ca4)

13. Membagi data Train dan Test 70 : 30 : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/0a7cba7c-519c-4c06-ada8-b9a713b73b6e)

14. Split X dan Y 

15. Melakukan data Train SMOTE : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/59bf202c-cd70-4900-a2d6-60b37cba44fe)

16. Pint data Train dan Test : 

![image](https://github.com/Astryon/Stage3_Final_Project/assets/68798868/314f6090-0f85-49e8-b26d-03247e353dc5)









