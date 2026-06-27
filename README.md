# genomescope
Mini Project Bioinformatika menggunakan Python untuk menganalisis GC Content pada genom tiga organisme yang diperoleh dari NCBI.
# Deskripsi

Project ini bertujuan untuk menghitung dan membandingkan kandungan GC Content dari tiga organisme menggunakan data genom lengkap (complete genome) yang diunduh langsung dari National Center for Biotechnology Information (NCBI).

Analisis dilakukan menggunakan Biopython, Pandas, NumPy, dan Matplotlib.

# Tujuan
Mengambil data genom dari NCBI menggunakan Accession Number.
Membaca file FASTA menggunakan Biopython.
Menghitung frekuensi nukleotida (A, T, G, C).
Menghitung GC Content setiap organisme.
Mengurutkan organisme berdasarkan GC Content.
Membuat visualisasi hasil analisis.
Mengekspor hasil ke format CSV.

# Dataset
Organisme	Accession
Escherichia coli	NC_000913.3
Psychrobacter arcticus	NC_007204.1
Methanocaldococcus jannaschii	NC_000909.1

Sumber data: National Center for Biotechnology Information (NCBI).

# Workflow
Download genome dari NCBI.
Parsing file FASTA.
Menyimpan data menggunakan List dan Dictionary.
Menghitung frekuensi nukleotida.
Menghitung GC Content.
Sorting berdasarkan GC Content.
Visualisasi hasil.
Export hasil analisis ke CSV.

# Output
Tabel hasil analisis GC Content.
Grafik profil GC Content.
Grafik komposisi basa nitrogen.
Scatter plot panjang genom vs GC Content.
File CSV hasil analisis.

📁 Struktur Repository
gc-content-genome-analyzer
│
├── notebook/
├── data/
├── outputs/
├── laporan/
├── README.md
├── requirements.txt
└── LICENSE

# Library
Biopython
Pandas
NumPy
Matplotlib
