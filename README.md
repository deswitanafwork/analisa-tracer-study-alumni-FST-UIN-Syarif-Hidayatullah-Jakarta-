  Mengubah data survei mentah yang berantakan menjadi rekomendasi strategis. Proyek ini menganalisis data Tracer Study Alumni Fakultas Sains dan Teknologi (FST) UIN Jakarta untuk memetakan tren karir, masa tunggu kerja, dan keterserapan lulusan di industri.
  Data berasal dari survei primer (Google Form) yang tidak terstandarisasi, memiliki banyak typo, anomali logika input responden, dan variasi kategorikal yang tumpang tindih. Pendekatan Saya:
  Advanced Data Cleaning: Menormalisasi ratusan variasi nama perusahaan/universitas dan mengkoreksi outlier yang tidak logis (misal: memperbaiki input gaji '300,000' atau '49' menjadi format jutaan yang seragam berdasarkan konteks data).
  Feature Engineering: Mengekstraksi variabel baru yang lebih bermakna untuk analisis, seperti menghitung 'Lama Studi' dari tahun masuk dan lulus, serta mengelompokkan 'Masa Tunggu Kerja' ke dalam rentang waktu yang terstruktur.
  Strategic Justification: Mempertahankan missing values pada kondisi tertentu karena secara realitas hal tersebut merepresentasikan karakteristik responden survei yang valid.
Didapatkan temuan (Key Insights) dari projek ini adalah:
- Tren Masa Tunggu: Mayoritas alumni FST UIN Jakarta berhasil mendapatkan pekerjaan pertama dalam kurun waktu [X] hingga [Y] bulan.
- Segmentasi Alumni (Clustering): Melalui algoritma K-Modes, alumni dapat dikelompokkan ke dalam [X] cluster utama yang menunjukkan pola korelasi antara IPK, lama studi, dan kisaran penghasilan.
- Rekomendasi Bisnis: Memberikan insight berbasis data kepada pihak rektorat/fakultas untuk evaluasi kurikulum demi mempercepat adaptasi lulusan di dunia kerja.
Tech Stack & Tools yang digunakan pada projek ini ialah:
- Python (Pandas, NumPy): Manipulasi data, pembersihan data (data wrangling), dan rekayasa fitur.
- Scikit-Learn & K-Modes: Label encoding, standarisasi data, dan pemodelan clustering untuk data kategorikal.
- Matplotlib & Seaborn: Visualisasi data eksploratif (EDA) untuk menemukan pola tersembunyi.

Tertarik dengan proses analisis di balik layar? Silakan telusuri Jupyter Notebook di repositori ini. Jika Anda memiliki feedback atau ingin berdiskusi mengenai peluang kolaborasi dan karir di bidang data, mari terhubung melalui LinkedIn saya (https://www.linkedin.com/in/deswita-nur-ardias-farsha-53a251284?utm_source=share_via&utm_content=profile&utm_medium=member_android) atau email saya deswitanaf.work@gmail.
