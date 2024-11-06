# LabPy03

# LATIHAN 1

![WhatsApp Image 2024-11-06 at 14 34 55](https://github.com/user-attachments/assets/26a10ecb-b31f-467c-84c8-2dbdb397f56d)

Saya akan menjelaskan alur algoritma dari kode tersebut secara terstruktur:

# Inisialisasi

   - Import fungsi random untuk menghasilkan angka acak
   - Meminta input nilai N dari user
   - Set counter awal = 1

# Proses Utama (Loop While)

WHILE counter <= N:

    A. Generate angka random antara 0-1
    
    B. IF angka random < 0.5:
    
        - Tampilkan "data ke-{counter} => {angka random}"
        - Tambah counter dengan 1
        
        
    C. IF angka random >= 0.5:
    
        - Tidak melakukan apa-apa
        
        - Kembali ke langkah 1

# Kondisi Terminasi

    A. Loop berhenti ketika counter > N
    B. Tampilkan "Selesai"

Flowchart algoritma:

     Start
     ↓
    [Input nilai N]
     ↓
    [Set counter = 1]
     ↓
    ┌─────────────────────┐
    │ While counter <= N  │←──────┐
    └─────────┬───────────┘       │
              ↓                   │
        [Generate random]         │
              ↓                   │
        [Cek random < 0.5]        │
              ↓                   │
         [Jika Ya]──→[Print data] │
               ↓         ↓        │
         [Jika Tidak]   [counter++]
          │         │        │
          └─────────┘        │
               ↑             │
               └─────────────┘
               ↓
      [Print "Selesai"]
       ↓
       End

# Penjelasan Detail:

1. Program meminta user memasukkan nilai N yang menentukan berapa banyak angka random < 0.5 yang diinginkan
   
2. Program akan terus menghasilkan angka random sampai mendapatkan N buah angka yang nilainya < 0.5

   - Jika angka random ≥ 0.5: diabaikan dan generate angka baru
   - Jika angka random < 0.5: dicetak dan counter bertambah
  
4. Dari output yang terlihat:

   - User memasukkan N = 5
   - Program menghasilkan 5 angka random < 0.5
     
      data ke: 1 => 0.22422725915012398
     
      data ke: 2 => 0.08143383880445236
     
      data ke: 3 => 0.29455614142741193
     
      data ke: 4 => 0.12537763804880175
     
      data ke: 5 => 0.46041201475820446

2. Setelah mendapatkan 5 angka yang memenuhi syarat, program selesai dan mencetak "Selesai"

   - Program ini mendemonstrasikan konsep:

   - Perulangan dengan kondisi (while loop)

   - Pengambilan keputusan (if condition)

   - Pembangkitan angka random

   - Pencacahan (counter)

   - Format string untuk output

   - Saya akan menjelaskan alur algoritma dari kode perhitungan laba tersebut:

# LATIHAN 2
