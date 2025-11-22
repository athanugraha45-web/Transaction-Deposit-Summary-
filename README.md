📦 atm-dashboard-project
│
├── data/
│   ├── raw/               # Data mentah dari berbagai sumber (file transaksi)
│   │   ├── file1.csv
│   │   ├── file2.csv
│   │   ├── file3.csv
│   │   └── file4.csv
│   ├── cleaned/           # Output setelah pembersihan & sinkronisasi tanggal
│   │   └── merged_cleaned.csv
│   └── sample/            # Random sampling 50.000 baris
│       └── dataset_50k.csv
│
├── notebook/
│   └── Notebook.ipynb     # Script Python untuk merging, cleaning, sampling
│
├── dashboard/
│   ├── google_sheet_link.txt   # Link dashboard Google Sheets (opsional)
│   └── screenshot_dashboard.png
│
└── README.md

