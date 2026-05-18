🛡️ Network Database Manager Dashboard

📌 Deskripsi Project

Network Database Manager adalah sebuah analytical tool berbasis web yang dirancang untuk memproses, menyimpan, dan memvisualisasikan log lalu lintas jaringan (network traffic logs).

Project ini mensimulasikan pipeline data sederhana: mengekstrak data mentah dari format CSV, mentransformasikannya dan menyimpannya ke dalam database SQLite yang terstruktur, lalu menampilkannya melalui dashboard interaktif menggunakan Streamlit.

✨ Fitur Utama

Automated Data Pipeline: Script ETL (analysis.py) untuk memproses data CSV mentah menjadi database relasional (SQLite).

Interactive Dashboard: Antarmuka web responsif untuk memantau metrik jaringan.

Key Metrics Tracking: Menampilkan total log, jumlah protokol unik, dan rata-rata ukuran paket data (bytes).

Data Visualization: Visualisasi distribusi protokol jaringan menggunakan Pie Chart dari Matplotlib.

🛠️ Teknologi yang Digunakan

Bahasa Pemrograman: Python

Frontend/Dashboard: Streamlit

Database: SQLite

Data Manipulation: Pandas

Data Visualization: Matplotlib

📂 Struktur Direktori

📦 project-folder
 ┣ 📂 data
 ┃ ┗ 📜 network_data_raw.csv    # Data mentah log jaringan
 ┣ 📜 analysis.py               # Script untuk generate SQLite DB dari CSV
 ┣ 📜 app.py                    # Script utama Dashboard Streamlit
 ┣ 📜 model.py                  # Script untuk logic/model data tambahan
 ┣ 📜 requirements.txt          # Daftar dependensi library Python
 ┗ 📜 README.md                 # Dokumentasi project


🚀 Cara Instalasi dan Menjalankan Project

Ikuti langkah-langkah di bawah ini untuk menjalankan project secara lokal:

1. Clone Repositori (Opsional)

git clone <link-repo-github-kamu>
cd <nama-folder-repo>


2. Install Dependensi
Pastikan kamu sudah menginstal Python. Lalu jalankan perintah ini untuk menginstal semua library yang dibutuhkan:

pip install -r requirements.txt


3. Generate Database
Sebelum menjalankan dashboard, kamu wajib membuat database SQLite-nya terlebih dahulu dari data CSV mentah.

python analysis.py


(Proses ini akan menghasilkan file network_manager.db di dalam folder project).

4. Jalankan Dashboard Streamlit
Setelah database berhasil dibuat, jalankan aplikasi web dengan perintah:

streamlit run app.py

Dashboard akan otomatis terbuka di browser kamu pada alamat http://localhost:8501.

👨‍💻 Author
desianafw
www.linkedin.com/in/desianafw
