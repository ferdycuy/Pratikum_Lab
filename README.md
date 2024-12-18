# Praktikum 1: Dasar PHP, Array, dan Fungsi

## Pendahuluan
Praktikum ini bertujuan untuk memberikan pemahaman dasar tentang:
1. Konsep global aplikasi web dengan PHP.
2. Kerangka program PHP, tipe data, variabel, dan operator.
3. Sintaks dasar untuk alur program seperti kondisional dan perulangan.
4. Implementasi array dan fungsi dalam PHP.

---

## Latihan

### Latihan 1
**Kode:**
```php
<?php
$hello = "Hello World!";
$a_number = 4;
$anotherNumber = 8.9;
$bool = true;
?>
```
**Hasil dan Penjelasan:**
- Jika simbol `$` dihapus, program akan menghasilkan error karena PHP membutuhkan `$` untuk mendefinisikan variabel.

---

### Latihan 2
**Kode:**
```php
<?php
echo "<h1>Variable</h1></br>";
$angka = 99;
echo "Ini adalah angka = $angka </br>";
$angka_2 = $angka + 1;
echo "Ini hasilnya = $angka_2 </br>";
?>
```
**Hasil dan Penjelasan:**
- Menampilkan nilai variabel `$angka` dan hasil operasi penambahan.

---

### Latihan 3
**Kode:**
```php
<?php
$addition = 2 + 4;
$subtraction = 6 - 2;
$multiplication = 5 * 3;
$division = 15 / 3;
$modulus = 5 % 2;

echo "Penambahan: 2 + 4 = $addition <br />";
echo "Pengurangan: 6 - 2 = $subtraction <br />";
echo "Perkalian: 5 * 3 = $multiplication <br />";
echo "Pembagian: 15 / 3 = $division <br />";
echo "Modulus: 5 % 2 = $modulus";
?>
```
**Hasil dan Penjelasan:**
- Menampilkan hasil operasi matematika dasar.

---

### Latihan 4
**Kode:**
```php
<?php
$x = 4;
$x += 3; // Ganti dengan -=, *=, /=, %=, atau .= untuk uji coba
echo "Hasil dari operasi tersebut adalah = $x";
?>
```
**Hasil dan Penjelasan:**
- Operator `+=` menambah nilai variabel `$x` dengan angka lain. Variasi operator lainnya dapat digunakan untuk melihat efek yang berbeda.

---

### Latihan 5
**Kode:**
```php
<?php
$my_name = "anotherguy";
if ($my_name == "someguy") {
    echo "Your name is someguy!<br />";
}
echo "Welcome to my homepage!";
?>
```
**Hasil dan Penjelasan:**
- Jika `$my_name` tidak sesuai dengan kondisi `if`, hanya teks "Welcome to my homepage!" yang ditampilkan.

---

### Latihan 6
**Kode:**
```php
<?php
$destination = "Tokyo";
echo "Traveling to $destination<br />";
switch ($destination) {
    case "Las Vegas":
        echo "Bring an extra $500";
        break;
    case "Amsterdam":
        echo "Bring an open mind";
        break;
    case "Tokyo":
        echo "Bring lots of money";
        break;
    default:
        echo "Unknown destination";
}
?>
```
**Hasil dan Penjelasan:**
- `switch` menjalankan blok kode berdasarkan nilai dari `$destination`.

---

### Latihan 7
**Kode:**
```php
<?php
$brush_price = 5;
echo "<table border=\"1\" align=\"center\">";
echo "<tr><th>Quantity</th><th>Price</th></tr>";
for ($counter = 10; $counter <= 100; $counter += 10) {
    echo "<tr><td>$counter</td><td>" . ($brush_price * $counter) . "</td></tr>";
}
echo "</table>";
?>
```
**Hasil dan Penjelasan:**
- Membuat tabel perhitungan harga kuas dengan jumlah tertentu menggunakan perulangan `for`.

---

### Latihan 8
**Kode:**
```php
<?php
$vehicles = ["Mobil", "Sepeda", "Bus", "Becak", "Truk", "Andong", "Sepeda Motor"];
foreach ($vehicles as $vehicle) {
    echo "$vehicle<br />";
}
sort($vehicles);
echo "Sorted:<br />";
foreach ($vehicles as $vehicle) {
    echo "$vehicle<br />";
}
?>
```
**Hasil dan Penjelasan:**
- Menampilkan elemen array sebelum dan sesudah diurutkan dengan fungsi `sort()`.

---

### Latihan 10
#### Fungsi Fibonacci
**Kode:**
```php
<?php
function fibonacci($n) {
    if ($n <= 1) return $n;
    return fibonacci($n - 1) + fibonacci($n - 2);
}
echo "Fibonacci ke-5: " . fibonacci(5);
?>
```
**Hasil dan Penjelasan:**
- Menghitung bilangan Fibonacci ke-5 menggunakan fungsi rekursif.

#### Fungsi Pangkat
**Kode:**
```php
<?php
function power($x, $y) {
    return pow($x, $y);
}
echo "2 pangkat 3: " . power(2, 3);
?>
```
**Hasil dan Penjelasan:**
- Menghitung nilai pangkat dengan fungsi `pow`.

---

## Kesimpulan
Melalui praktikum ini, mahasiswa memahami:
- Dasar sintaks PHP untuk membuat program web dinamis.
- Penggunaan array dan fungsi untuk memproses data.
- Cara kerja kontrol alur dengan kondisional dan perulangan.
