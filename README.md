# Super-Cashier  

**Latar Belakang Masalah**  
Supermarket memerlukan Self-Service Kasir yang mempermudah customer untuk memasukkan item yang dibeli, jumlah item yang dibeli, dan harga item yang dibeli dan fitur lainnya.  
Oleh karena itu, self-service kasir akan dibuat dengan beberapa fitur di bawah ini agar aplikasi self-service kasir dapat berjalan lancar.  

**Requirements**  
Berikut ini adalah beberapa fitur yang akan ditemukan di Aplikasi Self-Service Kasir:  
1. Transaction(): untuk membuat ID customer serta memulai proses transaksi
2. add_item(): untuk menambahkan rincian produk yang  dibeli seperti nama, jumlah, dan harga
3. update_item() : untuk memperbarui data-data produk yang dibeli
4. delete_item(): untuk menghapus salah satu data produk yang sudah ditambahkan  
5. reset_transaction(): untuk menghapus semua produk yang ditambahkan
6. check_order(): untuk mengecek kembali produk yang sudah dibeli dan akan mengeluarkan output benar atau tidaknya pesanan
7. total_price(): untuk menghitung total belanjaan customer. Terdapat diskon jika memenuhi ketentuan sebagai berikut:
   a. Diskon 5%, jika total belanja di atas Rp. 200.000,-  
   b. Diskon 8%, jika total belanja di atas Rp. 300.000,-  
   c. Diskon 10%, jika total belanja di atas Rp. 500.000,-


**Flowchart**  
![flowchart super cashier drawio](https://github.com/user-attachments/assets/b96ca1db-3ea1-4f36-88f3-ab247f76c818)
  
**Functions**
Berikut ini adalah beberapa function yang terdapat di Aplikasi Self-Service Kasir:  
1. Transaction(): Class object yang digunakan untuk menjalankan proses transaksi  
2. add_item(): memerlukan input berupa nama, jumlah, dan harga  
3. update_item() : Dengan fitur ini, customer dapat mengubah nama produk di update_item_name(nama item, nama item terbaru), jumlah produk di update_item_qty(nama item, jumlah item), harga produk di update_item_price(nama item, harga item)  
4. delete_item(): memerlukan input nama item untuk menjalankan fungsinya  
5. reset_transaction(): tidak memerlukan input  
6. check_order(): tidak memerlukan input dan output akan terbagi menjadi dua. "Pemesanan sudah benar" jika tidak ada kesalahan input dan "Terdapat kesalahan input data" jika inputan ada yang salah  
7. total_price(): tidak memerlukan inputan dan akan menghitung total harga beserta diskon jika sudah memenuhi syarat yang diperlukan


**Test Case**  
Berikut ini adalah test case yang sudah dilakukan:  
Test Case 1:  
Customer ingin menambahkan dua item baru menggunakan method add_item(). Item yang ditambahkan adalah sebagai berikut:  
a. Nama item: Ayam Goreng, Qty: 2, Harga: 20000  
b. Nama item: Pasta Gigi, Qty: 3, Harga: 15000  
Output:  

Test Case 2:  
Customer ingin menghapus item dikarenakan salah membeli salah satu item. Maka customer menggunakan method delete_item() untuk menghapus item yaitu Pasta Gigi.  
Ouput:  

Test Case 3:  
Customer melakukan kesalahan dalam memasukan item lagi sehingga customer memilih untuk menghapus seluruh item belanjaannya daripada menghapusnya satu persatu. Kali ini, customer menggunakan method reset_transaction().  
Output:  

Test Case 4:  
Setelah customer selesai berbelanja, total harga belanja akan dihutung dengan method total_price() dan akan mendapatkan diskon sesuai ketentuan.  
Output:  

**Kesimpulan**  
Program self-service kasir sudah berjalan dengan lancar dan bisa digunakan oleh customer mempermudah proses transaksi. Untuk pengembangan lebih lanjut, program ini bisa diupgrade dengan menambahkan beberapa fitur baru seperti opsi pengiriman untuk customer yang berada di luar daerah supermarket sehingga mereke bisa berbelanja dengan mudah.

