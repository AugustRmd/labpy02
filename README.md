# Sistem Pembelian Tiket
Program sederhana untuk menghitung harga tiket berdasarkan jenis tiket dan status member.

## Deskripsi
Program ini memungkinkan pengguna untuk:

Memilih jenis tiket (VIP/Reguler)
Menentukan status member
Mendapatkan perhitungan harga tiket final dengan diskon jika memiliki kartu member

## Flowchart Program
````mermaid
flowchart TD
    A([Start]) --> B[/Input jenis ticket/]
    B --> C{Jenis ticket}
    C -- vip --> D[harga_ticket = vip]
    C -- reguler --> E[harga_ticket = reguler]
    C -- tidak valid --> F[/Cetak 'Input tidak valid'/]
    F --> K
    D --> G[/Input kartu member/]
    E --> G
    G --> H{Member=='ya'?}
    H -- True --> I[harga_ticket -= harga_ticket*0,2]
    H -- False --> K[/Cetak harga ticket/]
    I --> K
    K --> L([End])

````

## Contoh Output Program




## Cara Kerja Program:

1. Program menentukan harga awal:
   - Tiket VIP: Rp 100.000
   - Tiket Reguler: Rp 50.000

2. User diminta memilih jenis tiket:
   - Jika memilih "vip", harga diset Rp 100.000
   - Jika memilih "reguler", harga diset Rp 50.000
   - Jika input selain keduanya, program berhenti dengan pesan "Input tidak valid"

3. User diminta konfirmasi kepemilikan kartu member:
   - Jika memiliki kartu member (input "ya"), akan mendapat diskon 20%
   - Jika tidak memiliki (input "tidak"), tidak ada diskon

4. Program menampilkan harga akhir setelah perhitungan diskon

Contoh perhitungan:
- Jika pilih VIP dan punya member:
  Rp 100.000 - (20% × Rp 100.000) = Rp 80.000
- Jika pilih Reguler dan punya member:
  Rp 50.000 - (20% × Rp 50.000) = Rp 40.000




# Program Kalkulator Sederhana
Program kalkulator sederhana untuk menghitung inputan dari user.

## Deskripsi Program
Program kalkulator sederhana yang mampu melakukan operasi dasar matematika dengan dua bilangan.

## Flowchaart Kalkulator


````mermaid
flowchart TD
    A([Start]) --> B[/Input angka pertama/]
    B --> C[/Input angka kedua/]
    C --> D[/Input operator/]
    D --> E{Operator}
    E -- ' + ' --> F[Hasil = a + b]
    E -- ' - ' --> G[Hasil = a - b]
    E -- ' * ' --> H[Hasil = a * b]
    E -- ' / ' --> I[Hasil = a / b]
    E -- Else --> J[Cetak 'Input tidak valid']
    J --> L
    F --> K[/Cetak Hasilnya/]
    G --> K
    H --> K
    I --> K
    K --> L([End])

````

## Contoh Output Program


## Cara Kerja Program

### Alur Proses Kalkulator
1. Program meminta input angka pertama
2. Program meminta input angka kedua
3. Program meminta input operator matematika
4. Fungsi `kalkulator()` memproses input sesuai operator
5. Menampilkan hasil perhitungan

