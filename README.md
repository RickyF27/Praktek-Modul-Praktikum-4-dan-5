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

- EightPuzzleSearch

Pada class ini menggunakan EightPuzzleSpace supaya mendapatkan informasi tentang ruang pencarian dan kelas Node untuk mewakili simpul dalam pencarian. Class ini juga mengelola daftar terbuka, daftar tertutup serta menyediakan metode untuk mendapatkan simpul terbaik dari daftar terbuka (getBestNode), mendapatkan biaya sebelumnya dari simpul (getPreviousCost), mencetak jalur solusi (printPath), dan menjalankan algoritma pencarian (run).

- EightPuzzleSpace

Class ini bertugas untuk menghasilkan konfigurasi awal dan tujuan dari puzzle 8 angka, serta menghasilkan daftar kemungkinan langkah yang dapat diambil dari suatu keadaan puzzle dengan cara menyediakan metode untuk mendapatkan simpul awal (getRoot), mendapatkan tujuan (getGoal), dan mendapatkan daftar suksesor dari simpul tertentu (getSuccessors).

- Node

Class ini merepresentasikan simpul (node) dalam struktur data graf. Setiap simpul memiliki atribut state yang merupakan array integer berukuran 9, yang merepresentasikan keadaan dari puzzle 8 angka. Atribut lainnya termasuk biaya (cost) yang terkait dengan simpul tersebut, induk (parent) yang merupakan simpul yang merupakan pendahulu dari simpul saat ini, dan daftar suksesor (successors) yang merupakan daftar simpul anak dari simpul saat ini. Kelas ini juga memiliki metode untuk mengonversi ke string, memeriksa kesetaraan, dan mendapatkan jalur dari simpul ke akar.

2. Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 8. Kemudian tentukan langkah- langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1.

Jawaban :

Ubah initial dan goal pada program seperti berikut

![image](https://github.com/RickyF27/Praktek-Modul-Praktikum-4-dan-5/assets/149030301/df2460a2-2627-4264-ac0f-c531dbcd2eeb)

Dalam kode Eight Puzzle yang telah diberikan, langkah-langkah untuk mencapai keadaan tujuan dari keadaan awal dapat ditemukan dalam class EightPuzzleSearch. Class ini bertanggung jawab untuk mencari solusi dengan menggunakan algoritma pencarian A* dan memungkinkan pengguna untuk memilih heuristic yang akan digunakan baik itu h1 atau h2. Proses pencarian solusi melibatkan beberapa tahap berikut:

- Inisialisasikan keadaan awal dan keadaan tujuan.

- Buat node awal (root) menggunakan keadaan awal.

- Masukkan node awal ke dalam daftar open, ketika daftar open belum kosong lakukan langkah-langkah berikut:
  
     a. Pilih node dengan biaya terendah..

     b. Tambahkan node terpilih ke dalam daftar closed untuk menghindari pengulangan.

     c. Ketika node terpilih sama dengan keadaan tujuan, maka solusi telah ditemukan, dan proses berakhir.

     d. Dapatkan semua node penerus dari node terpilih.

     e. Untuk setiap node penerus, hitung biaya baru berdasarkan heuristic, panjang path, dan biaya sebelumnya.

     f. Jika node penerus belum pernah ada di daftar open atau memiliki biaya lebih rendah, tambahkan node penerus ke daftar open dengan biaya yang telah diperbarui.
  
Tahapan ini akan terus diulang sampai solusi ditemukan atau semua kemungkinan solusi dieksplorasi. Hasil akhir dari pencarian akan mencetak langkah-langkah solusi ke dalam output. Penting untuk dicatat bahwa class EightPuzzleSearch, EightPuzzleSpace, dan Node bekerja sama untuk mencari dan mengeksekusi solusi Eight Puzzle. Class EightPuzzleSearch mengatur logika pencarian, EightPuzzleSpace memberikan informasi tentang keadaan awal dan keadaan tujuan, serta menghasilkan node-node awal, sementara class Node digunakan untuk merepresentasikan setiap keadaan dalam permainan Eight Puzzle dan menyimpan informasi penting tentang keadaan tersebut, biayanya, dan node induknya.

Pada percobaan kedua, diperlukan 13 langkah untuk mencapai keadaan tujuan yang diinginkan, sedangkan pada percobaan pertama hanya memerlukan 6 langkah. Perbedaan ini disebabkan oleh perbedaan jarak yang lebih jauh dari keadaan awal ke keadaan tujuan pada puzzle di percobaan kedua, dibandingkan dengan percobaan pertama, atau karena kekacauan posisi yang lebih rumit pada percobaan kedua daripada percobaan pertama. Oleh karena itu, untuk mencapai keadaan tujuan yang diinginkan pada percobaan kedua, memerlukan langkah yang lebih banyak.

3. Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.9. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1 dan 2.

jawaban :

Ubah initial dan goal pada program seperti berikut

![image](https://github.com/RickyF27/Praktek-Modul-Praktikum-4-dan-5/assets/149030301/ba63605c-d780-4dbd-9a8b-cedc84debc38)

langkah-langkah untuk mencapai goal state adalah.

- Kondisi Awal (Root): {1, 5, 3, 4, 6, 8, 2, 7, 0}.

- Kondisi Goal: {7, 6, 5, 8, 0, 4, 1, 2, 3}.

- Jalannya Algoritma:

  a. Algoritma A* dimulai dengan kondisi awal (Root).

  b. Algoritma memeriksa semua kemungkinan langkah dari kondisi awal, mempertimbangkan posisi kotak kosong, dan menggunakan salah satu heuristik untuk menghitung biaya.

  c. Algoritma mencari jalur paling efisien menuju keadaan tujuan dengan mempertimbangkan biaya total.

  d. Algoritma memilih berdasarkan prioritas biaya terendah, yang ditentukan oleh heuristik yang digunakan.

  e. Algoritma terus berjalan hingga mencapai keadaan tujuan.

Pada percobaan ketiga, diperlukan 20 langkah untuk mencapai keadaan tujuan yang diinginkan, sementara pada percobaan pertama hanya memerlukan 6 langkah, dan pada percobaan kedua memerlukan 13 langkah untuk mencapai keadaan tujuan yang diinginkan. Perbedaan ini disebabkan oleh fakta bahwa teka-teki pada percobaan ketiga memiliki jarak yang lebih jauh dari keadaan awal hingga keadaan tujuan dibandingkan dengan percobaan pertama dan kedua.

4. Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.10. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1, 2, dan 3.

jawaban :

Ubah initial dan goal pada program seperti berikut

![image](https://github.com/RickyF27/Praktek-Modul-Praktikum-4-dan-5/assets/149030301/2a261c14-750e-47e9-8026-17900363f822)

Langkah-langkah untuk mencapai goal state adalah.

- Kondisi Awal (Root): {1, 2, 3, 4, 5, 6, 7, 8, 0}

- Kondisi Goal: {1, 2, 3, 4, 0, 5, 6, 7, 8}

- Alur Algoritma:

  a. Algoritma A* dimulai dengan kondisi awal (Root).

  b. Algoritma mencari langkah-langkah untuk mencapai keadaan akhir (Goal).

  c. Algoritma menggunakan salah satu heuristik untuk menghitung biaya setiap langkah.

  d. Algoritma memilih langkah-langkah yang memiliki biaya terendah berdasarkan heuristik yang dipilih.

  e. Algoritma terus berjalan hingga mencapai keadaan akhir (Goal).

Dalam percobaan ini, diketahui bahwa pada awalnya, root dari keempat percobaan menunjukkan perbedaan yang signifikan. Root di percobaan ketiga memiliki urutan angka yang lebih kompleks dibanding dengan root pada percobaan lainnya. Selain itu, solusi dari setiap percobaan juga menunjukkan perbedaan. Dalam percobaan pertama, solusinya adalah 1 6 5 8 0 4 2 7 3, sementara dalam percobaan kedua, solusinya adalah 1 2 3 4 5 6 7 8 0. Di sisi lain, dalam percobaan ketiga, solusinya adalah 7 6 5 8 0 4 1 2 3. Secara keseluruhan, walaupun keempat percobaan berhasil mencapai solusi, namun perbedaan pada root dan solusi menandakan bahwa program dimulai dari kondisi awal yang berbeda dan mencapai tujuan yang berbeda.

5. Ubahlah initial dan goal state dari program dan class-class di atas sehingga bentuk initial dan goal statenya Gambar 5.11. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state.

jawaban :

Ubah initial dan goal pada program seperti berikut

![image](https://github.com/RickyF27/Praktek-Modul-Praktikum-4-dan-5/assets/149030301/800a26b3-f18e-4c60-a478-6846778de4df)

langkah-langkah untuk mencapai goal state adalah.

- Mulailah dengan menginisialisasi node awal menggunakan keadaan awal dari puzzle.

- Persiapkan dua daftar: open list dan closed list. Letakkan node awal di dalam open list.
  
- Lakukan langkah-langkah berikut selama open list masih memiliki elemen di dalamnya:
  
  a. Pilih node dengan biaya terendah dari open list.
  
  b. Jika node yang dipilih adalah keadaan akhir (goal state), maka itu berarti puzzle telah selesai dan proses pencarian berakhir.
  
  c. Hasilkan semua node turunan dari node saat ini.
  
  d. Untuk setiap node turunan, hitung biaya f dan panjang jalur dari node awal hingga node saat ini.
  
  e. Jika node turunan sudah ada dalam open list dan biaya f yang baru lebih rendah, perbarui biaya node tersebut.
  
  f. Jika node turunan sudah ada dalam closed list dan biaya f yang baru lebih rendah, perbarui biaya node tersebut, dan pindahkan node dari closed list ke dalam open list.
  
  g. Jika node turunan belum ada dalam kedua daftar, tambahkan node tersebut ke dalam open list.
  
  h. Tandai node saat ini sebagai telah dieksplorasi dengan memindahkannya dari open list ke dalam closed list.

Algoritma mencoba berbagai kombinasi perpindahan ubin untuk menemukan jalur yang paling efisien menuju goal state. Pada percobaan ini untuk mencapai nilai goal state diperluhkan langkah yang sangat panjang, dikarenakan posisi pada root state dan goal state sangat jauh, hal ini juga disebabkan karena posisi node yang sangat teracak.
