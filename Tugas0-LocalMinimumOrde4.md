# Flowchart Pencarian Local Minimum (Newton-Raphson)

```mermaid
flowchart TD
    A([Mulai]) --> B[Definisikan fungsi polinomial orde 4]
    B --> C[Hitung turunan pertama dan kedua fungsi target]
    C --> D[Inisialisasi tebakan awal untuk memulai iterasi Newton Raphson]
    D --> E[Mulai iterasi Newton Raphson]
    E --> F[Hitung nilai turunan pertama dan kedua]
    F --> G{Apakah turunan kedua nol?}
    G -- Ya --> H([Stop: Hindari pembagian nol])
    G -- Tidak --> I[Update nilai x]
    I --> J{Apakah sudah konvergen?}
    J -- Tidak --> E
    J -- Ya --> K[Peroleh titik kritis]
    K --> L{Apakah turunan kedua positif?}
    L -- Ya --> M[Simpan sebagai titik minimum lokal]
    L -- Tidak --> N[Abaikan titik tersebut]
    M --> O[Plot fungsi dan tandai hasil titik minimum lokal]
    N --> O
    O --> P([Selesai])
