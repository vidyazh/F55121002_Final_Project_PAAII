# F55121002_Final_Project_PAAII
F55121002_Vidya Az Zahra_A (Final Project PAA II)

# Bubble Sort dan Insertion Sort Analisis Algoritma

## Worst Case
- Dalam analisis worst case, kita menghitung **batas atas** dari waktu eksekusi sebuah algoritma.
- Kita harus mengetahui kasus yang menyebabkan **jumlah operasi maksimum** yang harus dilakukan.
- Untuk bubble sort, worst case terjadi ketika array **terurut menurun**. Dalam kasus ini, algoritma harus melakukan **n-1 perbandingan** dan **n-1 pertukaran** di setiap iterasi, dan ada **n-1 iterasi** secara total. Oleh karena itu, kompleksitas waktu worst case dari bubble sort adalah **O(n^2)**.
- Untuk insertion sort, worst case juga terjadi ketika array **terurut menurun**. Dalam kasus ini, algoritma harus **menggeser setiap elemen** ke kanan sebanyak satu posisi di setiap iterasi, dan ada **n-1 iterasi** secara total. Oleh karena itu, kompleksitas waktu worst case dari insertion sort juga adalah **O(n^2)**.

## Best Case
- Dalam analisis best case, kita menghitung **batas bawah** dari waktu eksekusi sebuah algoritma.
- Kita harus mengetahui kasus yang menyebabkan **jumlah operasi minimum** yang harus dilakukan.
- Untuk bubble sort, best case terjadi ketika array **sudah terurut naik**. Dalam kasus ini, algoritma hanya melakukan **n-1 perbandingan** dan **tidak ada pertukaran** di iterasi pertama, dan kemudian berhenti karena tidak ada pertukaran. Oleh karena itu, kompleksitas waktu best case dari bubble sort adalah **Ω(n)**.
- Untuk insertion sort, best case juga terjadi ketika array **sudah terurut naik**. Dalam kasus ini, algoritma hanya melakukan **n-1 perbandingan** dan **tidak ada penggeseran** di setiap iterasi. Oleh karena itu, kompleksitas waktu best case dari insertion sort juga adalah **Ω(n)**.

## Average Case
- Dalam analisis average case, kita mengambil semua kemungkinan input dan menghitung **jumlah rata-rata operasi** untuk setiap ukuran input.
- Kita harus mengetahui (atau memprediksi) **distribusi kasus** untuk setiap ukuran input.
- Untuk bubble sort, mari kita asumsikan bahwa semua kasus memiliki distribusi seragam (termasuk best case dan worst case). Jadi kita menjumlahkan semua kasus dan membagi jumlahnya dengan (n!). Berikut ini adalah nilai kompleksitas waktu average case.

| n | Jumlah kasus | Jumlah perbandingan | Jumlah pertukaran |
|---|--------------|---------------------|-------------------|
| 1 | 1            | 0                   | 0                 |
| 2 | 2            | 1                   | 0.5               |
| 3 | 6            | 3                   | 1.5               |
| 4 | 24           | 6                   | 3                 |
| ...| ...          | ...                 | ...               |
| n | n!           | n(n-1)/2            | n(n-1)/4          |


Oleh karena itu, kompleksitas waktu average case dari bubble sort juga adalah **Θ(n^2)**.

- Untuk insertion sort, mari kita asumsikan bahwa setiap elemen dalam array memiliki probabilitas yang sama untuk lebih kecil atau lebih besar dari elemen lain. Jadi kita bisa mengharapkan bahwa setengah dari elemen dalam array lebih kecil dari elemen saat ini dan setengahnya lagi lebih besar. Oleh karena itu, kita bisa mengharapkan bahwa setiap elemen harus digeser sebanyak setengah dari posisinya di setiap iterasi. Berikut ini adalah nilai kompleksitas waktu average case.

| n | Jumlah perbandingan | Jumlah penggeseran |
|---|---------------------|--------------------|
| 1 | 0                   | 0                  |
| 2 | 0.5                 | 0.5                |
| 3 | 1.5                 | 1.5                |
| 4 | 3                   | 3                  |
| ...| ...                 | ...                |
| n | (n^2 - n)/4         | (n^2 - n)/4        |


Oleh karena itu, kompleksitas waktu average case dari insertion sort juga adalah **Θ(n^2)**.

# **TSP dan Dijkstra Analisis Algoritma**
# **Worst case**

*   TSP: Algoritma TSP memiliki kompleksitas faktorial O(n!), sehingga dalam kasus terburuknya, dengan banyaknya vertex yang besar, algoritma ini akan membutuhkan waktu yang sangat lama dan tidak efisien.
*   Dijkstra: Jika semua vertex saling terhubung dengan bobot yang sama, algoritma Dijkstra memiliki kompleksitas O(|V|^2), dimana |V| adalah jumlah vertex. Jika ada banyak vertex, algoritma ini akan membutuhkan waktu yang cukup lama.

# **Best case**



*   TSP: Algoritma TSP memiliki kinerja terbaik saat hanya terdapat sedikit vertex yang saling terhubung, sehingga jumlah permutasi yang dihasilkan sedikit.
*   Dijkstra: Jika hanya terdapat sedikit vertex yang saling terhubung atau jika titik awal dan akhir langsung terhubung, algoritma Dijkstra akan memiliki kinerja terbaik dengan waktu eksekusi yang cepat.

# **Average case**



*   TSP: Algoritma TSP memiliki kompleksitas faktorial O(n!), sehingga kinerjanya sangat dipengaruhi oleh jumlah vertex yang ada. Semakin banyak vertex, semakin lama waktu yang dibutuhkan untuk menghitung jalur terpendek.
*   Dijkstra: Algoritma Dijkstra memiliki kompleksitas O(|V|^2), dimana |V| adalah jumlah vertex. Pada kasus rata-rata, kinerja algoritma ini tergantung pada jumlah vertex dan banyaknya edge yang terhubung.
  
