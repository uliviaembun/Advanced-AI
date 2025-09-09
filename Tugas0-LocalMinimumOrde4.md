# Flowchart Pencarian Local Minimum (Newton-Raphson)

```mermaid
flowchart TD
    A([Mulai]) --> B["Definisikan fungsi f(x) dan turunannya f'(x), f''(x)"]
    B --> C["Inisialisasi nilai awal x0"]
    C --> D[Iterasi]
    D --> E["Hitung f'(x) dan f''(x)"]
    E --> F["Update x = x - f'(x)/f''(x)"]
    F --> G{"Cek konvergensi?"}
    G -- Tidak --> D
    G -- Ya --> H["Output local minimum x*, f(x*)"]
    H --> I([Selesai])
