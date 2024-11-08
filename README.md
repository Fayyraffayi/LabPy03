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

![WhatsApp Image 2024-11-06 at 14 34 55 (1)](https://github.com/user-attachments/assets/58c0626a-705a-4a96-b22a-c8d62bedb063)

# 1. Inisialisasi

       laba_bulanan = []  # Array kosong untuk menyimpan laba per bulan
       total_laba = 0     # Variabel untuk menyimpan total laba
       modal_awal = 100000000  # Modal awal (tersirat dari output)

# 2. Proses Perhitungan Laba (Loop pertama)

    FOR bulan FROM 1 TO 8:
    1. Set laba = 0
    
    2. Hitung laba berdasarkan bulan:
       IF bulan <= 2:           # Bulan 1-2
          laba = 0
       ELSE IF bulan <= 4:      # Bulan 3-4
          laba = modal_awal * 1% (0.01)
       ELSE IF bulan <= 7:      # Bulan 5-7
          laba = modal_awal * 5% (0.05)
       ELSE:                    # Bulan 8
          laba = modal_awal * 2% (0.02)
    
    3. Simpan laba ke array laba_bulanan
    4. Tambahkan laba ke total_laba

Flowchart algoritma:

         Start
          ↓
      [Inisialisasi variabel]
          ↓
      ┌─────────────────────┐
      │ For bulan 1 to 8   │
      └─────────┬───────────┘
                ↓
         [Set laba = 0]
                ↓
         [Cek kondisi bulan]
                ↓
        ┌─────────────────┐
        │ Bulan 1-2: 0%   │
        │ Bulan 3-4: 1%   │
        │ Bulan 5-7: 5%   │
        │ Bulan 8: 2%     │
        └────────┬────────┘
                 ↓
           [Hitung laba]
                 ↓
         [Simpan ke array]
                 ↓
        [Update total_laba]
                 ↓
       ┌─────────────────────┐
        │ For each laba      │
       └─────────┬───────────┘
                 ↓
      [Tampilkan laba per bulan]
                 ↓
     [Tampilkan total laba]
                 ↓
                end

Output Program:

       laba bulan ke- 1 sebesar: 0
       laba bulan ke- 2 sebesar: 0
       laba bulan ke- 3 sebesar: 1000000.0
       laba bulan ke- 4 sebesar: 1000000.0
       laba bulan ke- 5 sebesar: 5000000.0
       laba bulan ke- 6 sebesar: 5000000.0
       laba bulan ke- 7 sebesar: 5000000.0
       laba bulan ke- 8 sebesar: 2000000.0
       Total laba adalah: 19000000.0

Penjelasan Logika Bisnis:

       Bulan 1-2: Belum ada laba (0%)
       Bulan 3-4: Laba 1% dari modal
       Bulan 5-7: Laba meningkat jadi 5% dari modal
       Bulan 8: Laba turun menjadi 2% dari modal

Program ini mendemonstrasikan konsep:

      Array dan operasi append
      Perulangan (for loop)
      Pengambilan keputusan berjenjang (if-elif-else)
      Perhitungan persentase
      Akumulasi nilai
      Format string untuk output

# LATIHAN 3

![WhatsApp Image 2024-11-06 at 14 34 55 (2)](https://github.com/user-attachments/assets/58274ebd-701a-4c5b-8f39-997fb28e60c0)

# 1. Inisialisasi Program

        def atm_simulator():
             saldo = 1000000  # Saldo awal

# 2. Alur Utama

LOOP Program ATM:
    1. Tampilkan menu:
       - 1. Tarik Uang
       - 2. Keluar
    
    2. Minta input pilihan menu (1/2)
    
    3. CASE Pilihan:
       CASE "1" (Tarik Uang):
          a. Minta input jumlah penarikan
          b. Validasi penarikan:
             IF jumlah > saldo:
                Tampilkan "Maaf, saldo tidak mencukupi!"
             ELSE IF jumlah <= 0:
                Tampilkan "Jumlah penarikan tidak valid!"
             ELSE:
                Kurangi saldo dengan jumlah penarikan
                Tampilkan "Penarikan berhasil!"
       
       CASE "2" (Keluar):
          a. Tampilkan "Terima kasih telah menggunakan ATM!"
          b. Keluar dari program (break)
       
       DEFAULT:
          Tampilkan "Pilihan tidak valid!"

Flowchart algoritma:

                         Start
                           ↓
                  [Inisialisasi saldo]
                           ↓
                 ┌─────────────────────┐
                 │ Loop ATM Program   │←─────────┐
                 └─────────┬───────────┘         │
                           ↓                     │
                     [Tampilkan Menu]            │
                           ↓                     │
                     [Input Pilihan]             │
                           ↓                     │
                     [Cek Pilihan]               │
                           ↓                     │
                     ┌─────────────────┐         │
                     │ Pilihan = 1     │──→[Input Jumlah]    
                     │ Pilihan = 2     │──→[Tampil Terima Kasih]→[Exit]
                     │ Pilihan Invalid │──→[Tampil Error]     │
                     └────────┬────────┘         │
                              ↓                  │
                      [Validasi Jumlah]          │
                           ↓                     │
                      [Update Saldo]             │
                           ↓                     │
                      [Tampil Status]            │
                           └─────────────────────┘

Output Program yang terlihat:

      Saldo saat ini: Rp 1000000
      1. Tarik Uang
      2. Keluar
      Pilih menu (1/2): 1
      Masukkan jumlah penarikan: 500000
      Penarikan berhasil!

      Saldo saat ini: Rp 500000
      1. Tarik Uang
      2. Keluar
      Pilih menu (1/2): 2
      Terima kasih telah menggunakan ATM!

# Penjelasan Detail:
#      1. Struktur Data

              - Variabel saldo: menyimpan saldo rekening
              - Variabel pilihan: menyimpan pilihan menu
              - Variabel jumlah: menyimpan jumlah penarikan

#      2. Validasi

                - Validasi pilihan menu (harus 1 atau 2)
                - Validasi jumlah penarikan:
                   - Tidak boleh melebihi saldo
                   - Tidak boleh negatif atau nol


#       3. Fitur

            - Cek saldo
            - Penarikan uang
            - Keluar dari program

       Program ini mendemonstrasikan konsep:

                     - Function definition
                     - Loop control (break)
                     - Conditional statements (if-elif-else)
                     - Input/output handling
                     - Basic error handling
                     - Variable manipulation
                     - Menu-driven interface
