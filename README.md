# Sistem Pembelian Tiket
Program sederhana untuk menghitung harga tiket berdasarkan jenis tiket dan status keanggotaan.

## Deskripsi
Program ini memungkinkan pengguna untuk:

Memilih jenis tiket (VIP/Reguler)
Menentukan status keanggotaan
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
