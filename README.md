# Fundamental SQL Using INNER JOIN and UNION
Tugas Praktek
Cobalah ketik query pada code editor untuk melihat keseluruhan isi dari kolom tabel ms_item_kategori dan ms_item_warna.

select * from ms_item_kategori;
select * from ms_item_warna;

+-----------+----------+
| nama_item | kategori |
+-----------+----------+
| bayam     | sayuran  |
| belimbing | buah     |
| duku      | buah     |
| durian    | buah     |
| gandum    | buah     |
| jamur     | sayuran  |
| jambu air | buah     |
| jeruk     | buah     |
+-----------+----------+
+-------------+--------------+
| nama_barang | warna        |
+-------------+--------------+
| apel        | merah        |
| bayam       | hijau        |
| daun bawang | hijau        |
| duku        | kuning pekat |
| durian      | kuning       |
| gandum      | coklat       |
| jambu air   | merah        |
| jeruk       | oranye       |
+-------------+--------------+

Menggabungkan Tabel dengan Key Columns
Saatnya  mempraktekkan penggabungan tabel ms_item_kategori dan ms_item_warna menggunakan key columns.

select * from ms_item_kategori,ms_item_warna
where nama_barang = nama_item;

+-----------+----------+-------------+--------------+
| nama_item | kategori | nama_barang | warna        |
+-----------+----------+-------------+--------------+
| bayam     | sayuran  | bayam       | hijau        |
| duku      | buah     | duku        | kuning pekat |
| durian    | buah     | durian      | kuning       |
| gandum    | buah     | gandum      | coklat       |
| jambu air | buah     | jambu air   | merah        |
| jeruk     | buah     | jeruk       | oranye       |
+-----------+----------+-------------+--------------+

