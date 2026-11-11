# akomodasi_kintamani_2501010046
# Akuisisi Data Akomodasi di Kecamatan Kintamani

- **Nama Mahasiswa:** Putu Intan Cahyanti Putri[cite: 1]
- **NIM:** 2501010046[cite: 1]
- **Mata Kuliah:** BIFP-243 Akuisisi dan Manajemen Data (INSTIKI)[cite: 1]

## Tujuan
Mengakuisisi data akomodasi di Kecamatan Kintamani secara etis melalui Overpass API OpenStreetMap, membersihkan dan mengubahnya ke dalam format tabular, serta menilai kelengkapannya terhadap data resmi BPS[cite: 1, 2, 3].

## Sumber Data & Atribusi
Data diakuisisi dari **OpenStreetMap melalui Overpass API** (https://overpass-api.de/api/interpreter)[cite: 3].
> © OpenStreetMap contributors (Lisensi ODbL)[cite: 3].

## Metode Akuisisi & Batasan Etika
- Menggunakan endpoint resmi Overpass API dengan penanganan *retry* dan *timeout*[cite: 5, 6].
- Menerapkan prinsip minimisasi data dengan mengecualikan informasi kontak pribadi[cite: 6, 10].
- Tidak menggunakan sumber terlarang seperti OTA atau web scraping Google Maps[cite: 3].

## Cara Menjalankan Ulang
1. Pastikan pustaka Python `requests` dan `pandas` terinstal di lingkungan kerja Anda.
2. Jalankan notebook di folder `notebooks/akuisisi_akomodasi.ipynb` untuk mengunduh ulang data mentah atau gunakan data yang tersedia di `data/raw/`[cite: 8].
3. Jalankan pemrosesan perataan data (*flattening*) untuk menghasilkan file tabular di `data/interim/akomodasi_kintamani.csv`[cite: 6, 8].
