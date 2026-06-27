# GC Content Genome Analysis

Mini Project Bioinformatika untuk menganalisis komposisi nukleotida dan **GC Content** pada genom tiga organisme menggunakan Python dan data sekuens dari National Center for Biotechnology Information (NCBI).

## Deskripsi Proyek

GenomeScope merupakan pipeline analisis bioinformatika sederhana yang dikembangkan untuk membaca data genom dalam format FASTA, menghitung frekuensi nukleotida, menghitung nilai GC Content, melakukan pengurutan berdasarkan kandungan GC, serta menyajikan hasil analisis dalam bentuk tabel, visualisasi, dan file CSV.

Data genom diperoleh langsung dari basis data NCBI menggunakan accession number. Analisis dilakukan menggunakan Python dengan bantuan beberapa pustaka, yaitu Biopython, Pandas, NumPy, dan Matplotlib.

## Tujuan

Project ini bertujuan untuk:

1. Mengambil data genom dari NCBI menggunakan accession number.
2. Membaca dan memproses file FASTA menggunakan Biopython.
3. Menyimpan data sekuens menggunakan struktur data list dan dictionary.
4. Menghitung frekuensi nukleotida A, T, G, C, dan N.
5. Menghitung nilai GC Content pada setiap organisme.
6. Mengurutkan organisme berdasarkan nilai GC Content.
7. Membuat visualisasi hasil analisis.
8. Mengekspor hasil analisis ke dalam format CSV.

## Dataset

Dataset yang digunakan berupa genom lengkap dari tiga organisme dengan karakteristik adaptasi suhu yang berbeda.

| Organisme                       | Accession Number | Karakteristik   |
| ------------------------------- | ---------------- | --------------- |
| *Escherichia coli*              | NC_000913.3      | Mesofilik       |
| *Psychrobacter arcticus*        | NC_007204.1      | Psikrofilik     |
| *Methanocaldococcus jannaschii* | NC_000909.1      | Hipertermofilik |

Sumber data: National Center for Biotechnology Information (NCBI).

## Workflow Analisis

Tahapan analisis dilakukan sebagai berikut:

1. Menentukan organisme dan accession number.
2. Mengunduh data genom dari NCBI menggunakan Bio.Entrez.
3. Membaca file FASTA menggunakan Bio.SeqIO.
4. Menyimpan data sekuens ke dalam struktur list dan dictionary.
5. Menghitung frekuensi nukleotida A, T, G, C, dan N.
6. Menghitung nilai GC Content dan AT Content.
7. Mengurutkan organisme berdasarkan nilai GC Content.
8. Membuat visualisasi hasil analisis.
9. Menyusun hasil dalam bentuk DataFrame.
10. Mengekspor hasil analisis ke file CSV.

## Output

Output yang dihasilkan dari project ini meliputi:

* Tabel hasil analisis GC Content.
* Tabel detail komposisi nukleotida.
* Grafik profil GC Content antarspesies.
* Grafik komposisi basa nitrogen.
* Scatter plot hubungan panjang genom dan GC Content.
* File CSV hasil analisis.

## Hasil Analisis

Hasil analisis menunjukkan bahwa *Escherichia coli* memiliki nilai GC Content tertinggi, diikuti oleh *Psychrobacter arcticus*, sedangkan *Methanocaldococcus jannaschii* memiliki nilai GC Content terendah.

| Rank | Organisme                       | Accession Number | GC Content (%) |
| ---- | ------------------------------- | ---------------- | -------------- |
| 1    | *Escherichia coli*              | NC_000913.3      | 50.7907        |
| 2    | *Psychrobacter arcticus*        | NC_007204.1      | 42.8002        |
| 3    | *Methanocaldococcus jannaschii* | NC_000909.1      | 31.4265        |

## Struktur Repository

```text
gc-content-genome-analyzer/
│
├── GenomeScope.ipynb
├── genome_sequences_3organisms.fasta
├── hasil_gc_content.csv
├── 1_komposisi_basa_per_spesies.png
├── 2_gc_content_per_spesies.png
├── 3_panjang_vs_gc_content.png
├── requirements.txt
├── README.md
├── LICENSE
└── .gitignore
```

## Library yang Digunakan

Project ini menggunakan beberapa pustaka Python berikut:

```text
biopython
numpy
pandas
matplotlib
```

Instalasi library dapat dilakukan dengan perintah:

```bash
pip install -r requirements.txt
```

## Cara Menjalankan

1. Clone repository ini atau download file project.
2. Buka file notebook `MiniProject_GC_Content_Analysis.ipynb` menggunakan Google Colab atau Jupyter Notebook.
3. Jalankan setiap cell secara berurutan.
4. Hasil analisis akan ditampilkan dalam bentuk tabel, grafik, dan file CSV.

## Ringkasan

Project ini menunjukkan penerapan dasar bioinformatika menggunakan Python untuk menganalisis komposisi nukleotida dan GC Content pada data genom. Selain memenuhi pipeline analisis FASTA dan GC Content, project ini juga menerapkan struktur data list dan dictionary dalam proses pengolahan data.
