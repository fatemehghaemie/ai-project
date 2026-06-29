# 🩺 AI Project 3: Diabetes Clinical Dataset Analysis & Modeling
## پروژه سوم هوش مصنوعی: تحلیل و مدل‌سازی داده‌های بالینی دیابت

This repository contains the third AI project for the **Amirkabir University of Technology (Tehran Polytechnic)**. The project focuses on Exploratory Data Analysis (EDA), preprocessing, and machine learning solutions applied to a clinical dataset of 100,000 diabetes records.

این مخزن شامل پروژه سوم درس هوش مصنوعی **دانشگاه صنعتی امیرکبیر (پلی‌تکنیک تهران)** است. تمرکز این پروژه بر روی تحلیل اکتشافی داده‌ها (EDA)، پیش‌پردازش و ارائه راهکارهای یادگیری ماشین بر روی یک دیتاست بالینی شامل ۱۰۰,۰۰۰ رکورد مربوط به بیماری دیابت است.

---

## 👥 Project Information / اطلاعات پروژه

* **University / دانشگاه:** Amirkabir University of Technology (Tehran Polytechnic) | دانشگاه صنعتی امیرکبیر
* **Course / درس:** Artificial Intelligence (AI) | هوش مصنوعی
* **Instructors / استادان درس:** Dr. Mehdi Ghatee & Mr. Behnam Yousefimehr | دکتر مهدی قطعی و آقای بهنام یوسفی‌مهر
* **Project Designers / طراحان پروژه:** Ilia Asadi, Mohammad Reza Sheikholeslami, Seyed Sina Negahban, Arian Jafari | ایلیا اسدی، محمدرضا شیخ الاسلامی، سید سینا نگهبان، آرین جعفری
* **Date / تاریخ:** Fall 1404 / پاییز ۱۴۰۴

---

## 🛠️ Tech Stack & Libraries / ابزارها و کتابخانه‌ها

The project utilizes the following Python libraries for data processing, clustering, and classification:
این پروژه از کتابخانه‌های زیر برای پردازش داده‌ها، خوشه‌بندی و دسته‌بندی استفاده می‌کند:

* **Data Handling:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
* **Dataset Management:** `opendatasets` (Kaggle API integration)
* **Resampling:** `imblearn` (SMOTE, SMOTEENN, RandomUnderSampler)
* **Clustering:** `KMeans`, `AgglomerativeClustering`, `DBSCAN`
* **Dimensionality Reduction:** `PCA`
* **Classification Models:** `LogisticRegression`, `RandomForestClassifier`, `XGBClassifier`, `SVC`
* **Hyperparameter Tuning:** `GridSearchCV`, `RandomizedSearchCV`

---

## 📊 Dataset Exploration (EDA) / بررسی اکتشافی داده‌ها

The dataset consists of **100,000 clinical records** downloaded directly from Kaggle via the `opendatasets` library:
[100,000 Diabetes Clinical Dataset](https://www.kaggle.com/datasets/priyamchoksi/100000-diabetes-clinical-dataset).

این دیتاست شامل **۱۰۰,۰۰۰ رکورد بالینی** است که مستقیماً از پلتفرم کگل دانلود می‌شود. ویژگی‌های کلیدی شامل موارد زیر است:

* `age`, `gender`, `bmi` (Body Mass Index)
* `hypertension`, `heart_disease`, `smoking_history`
* `hbA1c_level`, `blood_glucose_level`
* `race` columns (One-Hot Encoded: African-American, Asian, Caucasian, Hispanic, Other)
* **Target Feature / متغیر هدف:** `diabetes` (0 or 1)

### Technical Insight: Race Representation
* **English:** The race features are represented using **One-Hot Encoding** because each individual belongs to exactly one distinct ethnic category, ensuring no mutual inclusivity. Alternative representation methods include keeping a single categorical text column or converting it via **Label Encoding** (e.g., Caucasian=0, Asian=1, etc.). However, One-Hot Encoding is generally preferred for Machine Learning models to prevent numerical weight bias.
* **فارسی:** ویژگی‌های نژاد به روش **One-Hot Encoding** نمایش داده شده‌اند، زیرا هر فرد در یک زمان تنها به یک گروه نژادی تعلق دارد. روش‌های جایگزین شامل حفظ یک ستون متنی واحد یا تبدیل آن از طریق **Label Encoding** (مثلاً Caucasian=0 و Asian=1) است. با این حال، One-Hot Encoding به دلیل جلوگیری از سوءبرداشت مدل از وزن‌های عددی، ترجیح داده می‌شود.

---

## 🚀 Setup & Execution / نحوه اجرا

1. **Clone the repository / کلون کردن مخزن:**
   ```bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
   cd your-repo-name
