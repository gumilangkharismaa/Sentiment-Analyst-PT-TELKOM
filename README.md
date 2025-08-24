# Analisis Sentimen Berita dan Dokumen Telkom Indonesia

Project ini bertujuan untuk melakukan **analisis sentimen** terhadap **artikel berita online** maupun **dokumen lokal** (PDF/TXT) yang terkait dengan PT Telkom Indonesia. Analisis ini menggunakan Python dengan library seperti `newspaper3k`, `NLTK`, `VADER Sentiment Analyzer`, dan `Matplotlib` untuk pemrosesan data dan visualisasi.

## Fitur Utama

1. **Analisis Berita Online**
   - Mengambil artikel dari berbagai URL terkait Telkom Indonesia.
   - Membersihkan teks dari URL, karakter non-alphabet, dan stopwords.
   - Menggunakan **VADER Sentiment Analyzer** untuk mengklasifikasikan teks menjadi:
     - **Positif**: jika skor sentimen > 0.05  
     - **Negatif**: jika skor sentimen < -0.05  
     - **Netral**: jika skor sentimen antara -0.05 sampai 0.05
   - Menampilkan **distribusi sentimen** dengan diagram pie.
   - Menyimpan hasil analisis dalam DataFrame untuk review.

2. **Analisis Dokumen Lokal**
   - Membaca file PDF dan TXT yang berisi laporan analisis saham Telkom.
   - Membersihkan dan memproses teks seperti pada berita online.
   - Mengklasifikasikan sentimen menggunakan **VADER**.
   - Menampilkan **distribusi sentimen dokumen** dengan pie chart.
   - Mendukung banyak dokumen sekaligus.
