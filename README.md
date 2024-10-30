# labpy02

## Flowchart Ticket
````mermaid
flowchart TD
    A([Start]) --> B[/Input jenis ticket/]
    B --> C{Jenis ticket}
    C -- vip --> D[harga_ticket = vip]
    C -- reguler --> E[harga_ticket = reguler]
    C -- tidak valid --> F[/Cetak 'Input tidak valid' & keluar/]
    D --> G[/Input kartu member/]
    E --> G
    G --> H{Member=='ya'?}
    H -- True --> I[Diskon 20%]
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
    E -- lainnya --> J[Cetak 'Input tidak valid' & keluar]
    F --> K[/Cetak Hasilnya/]
    G --> K
    H --> K
    I --> K
    K --> L([End])

````
