# Super Cahsier Project

## Background Project
Andi adalah seorang pemilik supermarket besar di salah satu kota di Indonesia dan memiliki rencna untuk membuat sistem kasir self-service sehingga customer bisa langsung memasukkan item yang dibeli, jumlah item yang dibeli, dan harga item yang dibeli serta fitur lainnya.

## Feature Requirements
- Membuat ID transaksi customer
- Memasukkan nama item, jumlah item, dan harga barang menggunakan method add_item()
- Jika ada kesalahan dalam memasukkan nama item atau jumlah item atau harga item tetapi tidak ingin menghapus item tersebut, dapat menggunakan fungsi berikut
    - Update nama item dengan method update_nama_item()
    - Update jumlah item dengan method update_jumlah_item() 
    - Update harga item menggunakan method update_harga_baru()
- Jika batal membeli item belanjaan, customer bisa menghapus salah satu item dari nama item dengan method delet_item()
- Jika batal membeli dan ingin langsung menghapus semua transaksi atau reset transaksi bisa menggunakan method reset_transaction()
- Mengecek seluruh pesanan dengan method check_order()
- Checkout seluruh pesanan dengan menampilkan seluruh data yang dipesan beserta total harga dengan method checkout_order() 


## Flowchart 
![python cashier](https://user-images.githubusercontent.com/88957143/231932104-f83b1c53-4994-4d30-a616-4cb16f364b93.png)

## Penjelasan Method/ Function
- Class Transcation(), merupakan method untuk menaruh atau menampung semua fungsi untuk menjalankan transaksi.
![method1 1](https://user-images.githubusercontent.com/88957143/232258215-38a6b477-be5b-4012-97be-49fce5fadcc4.PNG)
- add_item, merupakan methode untuk menambahkan item yang akan dibeli.
![method 2](https://user-images.githubusercontent.com/88957143/232258460-ce2aface-1949-4168-a277-88e6aa63f842.PNG)
- update_nama_item, merupakan method untuk mengganti nama item tetapi tidak ingin mengganti item yang sudah ditambahkan.
![method 3](https://user-images.githubusercontent.com/88957143/232258759-8ac80580-d32b-4591-8967-97509ad2e12c.PNG)
- update_jumlah_item, merupakan method untuk mengganti jumlah item yang sudah ditambahkan dan tidak ingin mengganti jenis item tersebut.
![method 4](https://user-images.githubusercontent.com/88957143/232261649-20ee5b11-50bd-424c-b46e-15d600a7f164.PNG)
- update_harga_baru, merupakan method untuk mengganti harga item yang akan dibeli jika terjadi kesalahan input harga dan tidak ingin mengganti jenis item yang sudah ditambahkan.
![method 5](https://user-images.githubusercontent.com/88957143/232261706-0da499a3-89c8-4a51-898b-362ba6dd3f0d.PNG)
- delete_item, merupakan method untuk menghapus salah satu item yang tidak jadi dibeli tetapi sudah ditambahkan.
![method 6](https://user-images.githubusercontent.com/88957143/232261758-c7b888f7-e7db-43c3-8b38-3e45dc9e622e.PNG)
- reset_trasaction, merupakan method untuk menghapus seluruh item yang telah ditambahkan sekaligus.
![method 7](https://user-images.githubusercontent.com/88957143/232321756-3543e35c-9f37-49c9-b4e3-91f5e2011541.PNG)
- check_order, merupakan method untuk mengecek seluruh pesanan. baik nama item, jumlah, dan harga per item.
![method 8](https://user-images.githubusercontent.com/88957143/232322166-6117f350-1f6f-48d0-a43b-45f1f1811f2d.PNG)
- total_price, method yang menampilkan seluruh data yang dipesan beserta total harga yang harus dibayarkan.
![method 9](https://user-images.githubusercontent.com/88957143/232322482-cfa445b8-0221-452f-9c02-be99cd00fd13.PNG)

# Test Case
- Test 1
Customer ingin menambahkan dua item baru menggunakan add_item(). Item yang ditambahkan adalah sebagai berikut:
-- Nama Item: Ayam Goreng, qty: 2, harga: 20000
-- Nama Item: Pasta Gigi, qty: 3, harga: 15000
![test 1](https://user-images.githubusercontent.com/88957143/232323908-f6e6367f-7a79-456b-8f6a-a7c435a506f0.PNG)

- Test 2
Customer salah membeli salah satu item dari belanjaan yang sudah ditambahkan, maka Customer menggunakan method delete_item() untuk menghapus item. Item yang ingin dihapuskan adalah Pasta gigi.
![test 2](https://user-images.githubusercontent.com/88957143/232324857-576f334b-8708-432e-ac6b-9218cb3f9505.PNG)

- Test 3
Customer ingin menghapus semua pesanan yang dimasukkan daripada menghapus satu per satu menggunakan method resert_transaction.
![test 3](https://user-images.githubusercontent.com/88957143/232325136-6b511872-82ef-47b5-a506-99d3210ec05a.PNG)

- Test 4
Setelah customer belanja, akan menghitung semua total belanja yang harus dibayarkan menggunakan method total_price.
![test 4](https://user-images.githubusercontent.com/88957143/232325493-1d2a7587-ac43-4b64-92ae-1b397210b2f1.PNG)

## Kesimpulan dan Saran
Sistem kasir berjalan dengan semestinya dan sudah melewati beberapa test case yang sudah ditetapkan. Pengembangan lebih lanjut diperlukan agar program bisa berjalan lebih baik dan efisien.
