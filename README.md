# Praktek-Modul-Praktikum-4

1. Tentukan bagaimana algoritma BFS di atas dapat menentukan node ke 8, 6, dan 7.
   
Jawaban : Algoritma BFS akan mulai memasukkan node 3 kedalam antrian dikarenakan node 3 memiliki kedalaman 0, setelah diperiksa dan tidak mendapatkan node 8, 6, dan 7 maka pencarian akan dilanjutkan ke node 4 dan 2 dikarenakan node 4 dan 2 ini memiliki kedalaman 1 dan langsung terhubung kepada node 3, dan setelah diperiksa tidak mendapatkan node 8, 6 dan 7 maka pencarian akan dilanjutkan ke node 5, 6 dan 1 dimana pada node ini berada pada kedalaman 2 dan ditemukan hasil node 6 namuun untuk node 7 dan 8 belum ditemukan sehingga setelah memeriksa node 1 maka dilanjutkan pencarian ke node 7 dan 8 dimana node ini berada pada kedalaman 3 dan mendapatkan node 7 dan 8 sehingga node 8, 6, dan 7 telah ditemukan. Dalam pencarian menggunakan algoritma BFS ini pencrian dilakukan dari kiri ke kanan dan ketika tidak didapatkan hasil maka pencarian akan terus berjalan dari kiri ke kanan namun dengan tingkat kedalaman yang semakin tinggi sampai hasil ditemukan.


2.  Ubahlah method static void main sehingga bentuk tree seperti Gambar 4.4 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node 5. 

Jawaban :

untuk membuat gambar seperti pada tabel 4.4 kita harus mengganti bagian node pada code dimana untuk node yang digunakan adalah node 0 sampai node 6, kemudian kita juga harus mengatur node mana saja yang terhubung satu sama lain serta menentukan node mana yang harus berada pada kedalaman 0 seperti pada gambar dibawah ini.

![image](https://github.com/RickyF27/Praktek-Modul-Praktikum-4-dan-5/assets/149030301/c2f7ed8b-b7a8-4ed8-8c4f-7a379e6f5007)

Algoritma BFS akan mulai memasukkan node 0 kedalam antrian dikarenakan node 0 memiliki kedalaman 0, setelah diperiksa dan tidak mendapatkan node 5 maka pencarian akan dilanjutkan ke node 1 dan 2 dikarenakan node 1 dan 2 ini memiliki kedalaman 1 dan langsung terhubung kepada node 0, dan setelah diperiksa tidak mendapatkan node 5 maka pencarian akan dilanjutkan ke node 3, 4, 5, dan 6 dimana pada node ini berada pada kedalaman 2 dan ditemukan hasil node 5. Setelah menemukan node 5 proses akan terus berlanjut sampai semua node yang terhubung dengan node awal telah diperiksa. Dengan demikian, pada akhir proses BFS, node 5 akan ditemukan dan diproses sesuai dengan aturan algoritma BFS.


3.  Ubahlah method static void main sehingga bentuk tree seperti Gambar 4.5 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node 9.

Jawaban :

untuk membuat gambar seperti pada tabel 4.5 kita harus mengganti bagian node pada code dimana untuk node yang digunakan adalah node 1 sampai node 12, kemudian kita juga harus mengatur node mana saja yang terhubung satu sama lain serta menentukan node mana yang harus berada pada kedalaman 0 seperti pada gambar dibawah ini.

![image](https://github.com/RickyF27/Praktek-Modul-Praktikum-4-dan-5/assets/149030301/781408a0-45b8-4c66-9cdd-b085c4935385)

![image](https://github.com/RickyF27/Praktek-Modul-Praktikum-4-dan-5/assets/149030301/51f76516-78df-4e93-b030-53557c85b08f)

Algoritma BFS akan mulai memasukkan node 1 kedalam antrian dikarenakan node 1 memiliki kedalaman 0, setelah diperiksa dan tidak mendapatkan node 9 maka pencarian akan dilanjutkan ke node 2, 3 dan 4 dikarenakan node 2, 3 dan 4 ini memiliki kedalaman 1 dan langsung terhubung kepada node 1, dan setelah diperiksa tidak mendapatkan node 9 maka pencarian akan dilanjutkan ke node 5, 6, 7, dan 8 dimana pada node ini berada pada kedalaman 2 dan setelahh diperiksa tidak ditemukan hasil node 9 maka pencarian akan dilanjutkan ke node 9, 10, 11, dan 12 dimana pada node ini berada pada kedalaman 3 dan setelahh diperiksa ditemukan node 9. Setelah menemukan node 9 proses akan terus berlanjut sampai semua node yang terhubung dengan node awal telah diperiksa. Dengan demikian, pada akhir proses BFS, node 9 akan ditemukan dan diproses sesuai dengan aturan algoritma BFS.


4. Ubahlah kode program di atas sehingga bentuk tree seperti Gambar 6 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node C

Jawaban :

Untuk membuat gambar tree yang berisikan huruf kita harus mengganti code pada bagian public static class node dimana pada awalnya code bertuliskan int data menjadi string data, kemudian pada nodenya kita tambahkan dengan " " untuk mendefinisikan hurus tersebut, selain itu kita juga harus menyusun huruf mana saja yang terhubung satu sama lain serta menentukan huruf mana yang berada paling atas.

![image](https://github.com/RickyF27/Praktek-Modul-Praktikum-4-dan-5/assets/149030301/c57b5564-41dd-48dd-88dc-83f3195dd16b)

![image](https://github.com/RickyF27/Praktek-Modul-Praktikum-4-dan-5/assets/149030301/e1421a06-107c-4100-8776-c9ed1d733489) 

![image](https://github.com/RickyF27/Praktek-Modul-Praktikum-4-dan-5/assets/149030301/dc223528-24ad-4b2d-b1d1-6dc8b931fe05)

Untuk menemukan node 3 (C) algoritma BFS pertama-tama dimulai dengan memasukkan node 6 (F) ke dalam antrian, setelahh diperiksa dan tidak mendapatkan node 3(C) maka pencarian akan dilanjutkan ke node 2 (B), dan node 7 (G) yang terhubung langsung dengan node 6 atau node yang memiliki tingkat kedalaman 1. Setelah dilakukan pencarian dan tidak ditemukan hasil maka pencarian akan berlanjut ke node yang memiliki tingkat kedalaman 2 dimulai dari memeriksa node 1 (A), node 4 (D), dan node 9 (I). Apabila masih belum didapatkan node 3 (C) maka pencarian akan terus berlanjut ke tingkat kedalaman yang semakin tinggi yaitu kedalam 3 yang dimulai dari node 3 (C), dan pada node 3 (C) ini ditemukanlah hasil yang diinginkan, namun Setelah menemukan node 3 (C) proses akan terus berlanjut sampai semua node yang terhubung dengan node awal telah diperiksa. Dengan demikian, pada akhir proses BFS, node 3 (C) akan ditemukan dan diproses sesuai dengan aturan algoritma BFS.

 # Praktek-Modul-Praktikum-5

 1. Pelajari class EightPuzzleSearch, EightPuzzleSpace, dan Node.

Jawaban :

