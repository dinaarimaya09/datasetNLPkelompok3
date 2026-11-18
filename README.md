# Dataset NLP Kelompok 3  

# [KELOMPOK 3A]
## AI Smart Learning Assistant

Sistem berbasis Natural Language Processing untuk mengubah materi pembelajaran PDF menjadi:

1. Ringkasan teks dengan pilihan panjang: pendek, sedang, dan panjang.
2. Bukti/highlight bagian materi yang menjadi dasar ringkasan.
3. Audio pembelajaran.
4. Soal pilihan ganda berbasis karakteristik UTBK Literasi Bahasa Indonesia.
5. Umpan balik berbasis bukti dari materi sumber.

## Fokus Utama

- Text Summarization
- Question Generation
- Quiz Evaluation
- PDF Extraction
- Text-to-Speech sebagai fitur pendukung
- Learning History sebagai fitur pendukung

## Struktur Dataset

### 1. Dataset Soal UTBK Literasi Bahasa Indonesia

File: `data/utbk_lbi_dataset.csv`

Dataset ini digunakan sebagai acuan karakteristik soal, kategori kemampuan literasi, dan contoh gaya soal untuk Question Generation.

Sumber dataset: [https://github.com/dinaarimaya09/datasetNLPkelompok3.git]

### 2. Dataset Materi Pembelajaran

Folder: `data/raw_materials/`

Dataset ini berisi PDF materi pembelajaran berbahasa Indonesia yang menjadi input sistem untuk summarization dan question generation.

Sumber materi: [tambahkan tautan sumber setiap materi]

## Cara Menjalankan

```bash
pip install -r requirements.txt
streamlit run src/app.py
```

## Batasan Sistem

- PDF harus berbasis teks, bukan hasil scan.
- Materi harus berbahasa Indonesia.
- Sistem difokuskan pada teks dan paragraf, bukan tabel atau gambar.
- Soal yang dihasilkan berasal dari materi yang diunggah pengguna, bukan disalin dari dataset UTBK.
