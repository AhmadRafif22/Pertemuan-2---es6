# SPREAD OPERATOR
## Pengertian

Spread Operator dilambangkan dengan tiga titik "..." dan digunakan untuk menyebarkan atau memperluas elemen objek yang dapat diubah seperti array, string atau object

1. Spred Operator => Berfungsi memasukkan beberapa argument yang beerbentuk data array dalam fungsi, atau memasukkan nilai array berbentuk data array kedalam fungsi/ memasukkan data array ke dalam array lainnya
2. Inti dari spread operator yaitu sebagai Pelebur array menjadi beberapa elemen yang berbeda fitur 
4. Spread operator ====> Memecah (expend / unpack) menjadi single element
5. Yang awalnya berasal dari Iterabel (yang awalnya banyak elemen) kemudian menjadi single elemen (mis: Array, String dan Object) 

## Penggunaan Dengan Array
Salah satu penggunanan umum dari Spread Operator adalah menggabungkan array 
Misalnya, kalian dapat menggunakannya untuk membuat larik baru dengan menggabungkan dua atau lebih larik yang ada

<b> Contoh penggunanan: </b>
<b>1. Spread Operator untuk memecah iterables menjadi single element </b>
* Disini kita sudah mempunyai (index.html)
* Dan memiliki script seperti biasa
Yaitu :
Jika codingan seperti dibawah maka yang akan tampil adalah array

<image src= "Image\1.png">

Hasil

<image src= "Image\2.png">

Tapi kalau saya tambah fungsi Spread Operator "..." Maka :

<image src= "Image\3.png">

Hasil 

<image src= "Image\4.png">

<b>2. Spread Operator juga dapa menggabungkan anatara 2 array</b>
* Jika terdapat 2 array misal ada array mhs dan dosen
* Kemudian dapat di gabung antara 2 array diatas 
Yaitu :

<image src= "Image\5.png">

Hasil 

<image src= "Image\6.png">

<b>3. Spread Operator juga dapat menggabungkan array ditengah </b>

<image src= "Image\7.png">

Hasil 

<image src= "Image\8.png">

<b>4. Spread Operator dapat menyalin Array atau Object</b>
* Jika yang di console hanya array ke 1 

<image src= "Image\9.png">

Hasil 

<image src= "Image\10.png">

* Jika yang di console ingin array ke 2

<image src= "Image\11.png">

Hasil 

<image src= "Image\12.png">

## Penggunaan Dengan Objek
Saat digunakan dengan objek, operator spread dapat digunakan untuk:

1. Buat objek baru dengan properti dari objek yang sudah ada:{...obj}
2. Tambahkan atau timpa properti ke objek yang sudah ada:{...obj, newProp: value}
3. Menggabungkan dua atau lebih objek:{...obj1, ...obj2}

## Operator Spread
Operator spread adalah alat yang ampuh dalam JavaScript yang dapat menyederhanakan kode Anda dan membuatnya lebih mudah untuk bekerja dengan array, string, dan objek