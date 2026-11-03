# Analisis Tracer Study Alumni FST UIN Jakarta: Pemetaan Karir dan Evaluasi Kurikulum Menggunakan K-Prototypes Clustering

Pelaksanaan akademik dan penyusunan kurikulum perguruan tinggi yang relevan dengan kebutuhan industri membutuhkan umpan balik yang terukur, salah satunya melalui *tracer study*. Namun, data primer yang diperoleh langsung dari survei kuesioner alumni umumnya masih berupa data mentah yang penuh dengan *noise*, *missing values*, dan ketidakkonsistenan format pengisian. Oleh karena itu, diperlukan ekstraksi, pembersihan, dan pemodelan data secara analitik guna mengubah 435 baris data mentah tersebut menjadi *insight* yang berharga.

Sebagai Data Analyst, saya melakukan pemrosesan data dan eksplorasi *clustering* untuk mengelompokkan karakteristik alumni berdasarkan masa studi, tingkat penghasilan, dan status karir. Proses ini bertujuan untuk memberikan wawasan berbasis data (*data-driven insight*) kepada Rektor dan Pusat Karir (Puskarir) UIN Jakarta agar evaluasi kurikulum, penguatan jejaring alumni, dan proses akreditasi dapat berjalan secara optimal dan objektif.

# Import Library & Tech Stack

Ekstraksi, transformasi, dan pemodelan pada projek ini dibangun menggunakan *Tech Stack* analitik berikut:

* **Python (Pandas, NumPy):** Digunakan untuk manipulasi *dataframe*, ekstraksi data, transformasi tipe data, serta *feature engineering*.


* **Scikit-Learn & K-Modes:** Digunakan untuk prapemrosesan (*StandardScaler*, *LabelEncoder*) dan algoritma *clustering* (K-Prototypes) guna menangani dataset yang memiliki campuran tipe data numerik dan kategorikal.


* **Matplotlib & Seaborn:** Digunakan untuk Visualisasi Data Eksploratif (EDA) guna mendeteksi *outliers* dan memetakan hasil analisis secara visual.



# Pengumpulan Data

Data primer dikumpulkan melalui kuesioner Google Form yang disebarkan kepada alumni Fakultas Sains dan Teknologi (FST) UIN Jakarta. Dataset mentah ini memuat metrik penting seperti tahun masuk, waktu mendapatkan pekerjaan, kesesuaian kurikulum, dan status saat ini.

# Preprocessing & Feature Engineering

Pendekatan *preprocessing* dilakukan secara komprehensif agar model dapat membaca data yang bersih, konsisten, dan bermakna:

* **Data Reduction & Formatting:** Mengeliminasi kolom yang tidak relevan atau berisi data pribadi (seperti *Timestamp*, No HP, dan email) serta kolom yang sepenuhnya kosong. Karakter khusus pada penamaan kolom juga dibersihkan agar lebih terstruktur.


* **Noise Handling & Data Standardization:** Menormalisasi ambiguitas input data nominal, seperti memperbaiki format penulisan "Penghasilan" yang bervariasi (contoh: mengubah format '300,000' menjadi 0.3 dan '49' menjadi 4.9) serta menstandarisasi ragam penulisan nama institusi lanjutan menjadi seragam (UI, UGM, ITB).


* **Feature Engineering:** Menciptakan fitur analitik baru, yaitu `Lama Studi` (dihitung dari selisih tahun wisuda dan tahun masuk), serta mengelompokkan status karir alumni ke dalam klasifikasi makro pada fitur `Kelompok Status` (Kerja, Melanjutkan Studi, Belum Kerja, Ibu Rumah Tangga, Magang).


* **Data Filtering:** Mengeksklusi anomali logika pada data, seperti masa studi yang tidak wajar (1-2 tahun), untuk mempertahankan integritas dataset sebelum tahapan analisis lanjutan.



# Visualisasi Data Eksploratif (EDA) & Outlier Handling

Tahap ini memuat proses standardisasi nilai numerik serta mendeteksi sebaran data yang ekstrem (*outlier*) menggunakan visualisasi *Boxplot*. Karena sifatnya sebagai survei primer, data *outlier* (berkisar 242 data) dan *missing values* dipertahankan dengan perlakuan khusus (*imputation*) agar objektivitas informasi dan representasi populasi alumni tetap terjaga secara nyata.

---

*Tertarik dengan proses pembersihan data tingkat lanjut dan kode pemodelan clustering di balik layar?*
Silakan telusuri tahapan lengkapnya melalui Jupyter Notebook di repositori ini. Jika Anda memiliki *feedback*, masukan, atau ingin berdiskusi mengenai peluang kolaborasi dan karir di bidang data, mari terhubung melalui [LinkedIn Saya](https://www.linkedin.com/in/deswita-nur-ardias-farsha-53a251284?utm_source=share_via&utm_content=profile&utm_medium=member_android) atau jangkau saya melalui email di **deswitanaf.work@gmail.com**.
