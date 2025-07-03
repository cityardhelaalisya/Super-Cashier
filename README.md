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
  
**Functions**<br>
Berikut ini adalah Class dan Method yang terdapat di Aplikasi Self-Service Kasir:  
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
Code:  
![test case 1](https://github.com/user-attachments/assets/18b0136e-9650-4857-b28f-bc477dd2bebd)  
Output:  
![output test case 1](https://github.com/user-attachments/assets/646b4a56-6787-4211-b5d3-71e71ac79f44)
  
Test Case 2:  
Customer ingin menghapus item dikarenakan salah membeli salah satu item. Maka customer menggunakan method delete_item() untuk menghapus item yaitu Pasta Gigi.  
Code:<br>
![test case 2](https://github.com/user-attachments/assets/4fad977f-362d-4ff7-9871-ce815c0c0715)

Ouput:  
![output test case 2](https://github.com/user-attachments/assets/df26f9b4-61fd-4783-abca-7a57a0425cc0)

Test Case 3:  
Customer melakukan kesalahan dalam memasukan item lagi sehingga customer memilih untuk menghapus seluruh item belanjaannya daripada menghapusnya satu persatu. Kali ini, customer menggunakan method reset_transaction().  
Code:<br>
![test case 3](https://github.com/user-attachments/assets/56977625-ec77-48e1-8744-ee18a7c5ba71)

Output:  
![output test case 3](https://github.com/user-attachments/assets/67a5efbc-0cd0-4bb3-973a-639ca39d9dbf)

Test Case 4:  
Setelah customer selesai berbelanja, total harga belanja akan dihutung dengan method total_price() dan akan mendapatkan diskon sesuai ketentuan.  
Code:<br>
![test case 4](https://github.com/user-attachments/assets/ec8d041e-0f6c-4f8c-8859-d659fb248ab1)

Output:  
![output test case 4](https://github.com/user-attachments/assets/f966c798-3055-4b20-b3f4-010611276658)

**Kesimpulan**  
Program self-service kasir sudah berjalan dengan lancar dan bisa digunakan oleh customer mempermudah proses transaksi. Untuk pengembangan lebih lanjut, program ini bisa diupgrade dengan menambahkan beberapa fitur baru seperti opsi pengiriman untuk customer yang berada di luar daerah supermarket sehingga mereke bisa berbelanja dengan mudah.

