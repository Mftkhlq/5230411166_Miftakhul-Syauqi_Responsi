Disini saya membuat aplikasi desktop sederhana untuk yang dimana  membutuhkan staf dalam mengelola produk dan mencatat transaksi penjualan. Aplikasi ini berbasis GUI dan menggunkan bahasa pemrograman python dan menngunakan library Tkinter untuk menampilkan GUI nya, Yang dimana GUI tersebut bisa diakses oleh staff.
Posisi staf disini dapat melakukan operasi CRUD (Create, Read, Update dan Delete), Dan juga bisa menambahkan transaksi baru serta bisa menghapusnya. 
  1.	Fitur pada Manajemen produk :
  Fitur yang ada di dalam aplikasi ini adalah :
      1.	Add = staf bisa menambahkan produk yang ingin ditambahkan, seperti  menambahkan Nama barang ingin ditambahkan  stok beserta harganya.
      2.	Update = staf juga bisa melalukan update pada produk yg ingin diubah seperti
           Harga barang atau pun stok barang
      3.	Delete = terakhir staf dapat melakukan delete/hapus barang yang diinginkan,mungkin bisa saja barang tersebut sudah tidak ada lagi di gudang
    	    
  2.	Fitur pada manajemen transaksi
    Fitur yang ada di dalam aplikasi ini adalah :
      1.	Tambah transaksi = misal ada customer ingin melakukan pembelian, maka staf dapat membuat transaksinya.
      2.	Hapus transaksi = staf juga dapat melakukan hapus transaksi semisal transaksi tersebut dibatalkan oleh customer, maka staff dapat melakukanya.
    	
Cara menjalankannya :
      1.	Admin/ staf melakukan penambahan barang di manajemen produk, selanjutnya staf  dapat mengubah dan menghapus barang tersebut
      2.	Staf juga dapat mengubah transaksi di bagian manajemen transaksi

      
Struktur tabel pada Database :

Tabel produk
CREATE TABLE `products` (
  `id` int(11) NOT NULL,
  `name` varchar(100) NOT NULL,
  `price` decimal(10,2) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

Tabel transaksi
CREATE TABLE `transactions` (
  `id` int(11) NOT NULL,
  `product_id` int(11) NOT NULL,
  `quantity` int(11) NOT NULL,
  `total_price` decimal(10,2) NOT NULL,
  `date` date NOT NULL
) 



