# Fungsi pada JavaScript
Fungsi pada JavaScript adalah sebuah blok kode yang bisa digunakan kembali (reusable) yang melakukan tugas tertentu. Fungsi pada JavaScript sangat penting karena memungkinkan kita untuk mengorganisasi kode dan membuatnya lebih mudah dipahami, serta mengurangi duplikasi kode.

## Mendefinisikan Fungsi
Anda bisa mendefinisikan sebuah fungsi pada JavaScript dengan menggunakan kata kunci `function` diikuti dengan nama fungsi dan parameter (jika ada), kemudian diikuti dengan blok kode yang akan dijalankan ketika fungsi tersebut dipanggil.

Contoh: 
```
function tambah(a, b) {
  return a + b;
}
```
Di contoh di atas, `tambah` adalah nama fungsi, dan `a` dan `b` adalah parameter yang akan digunakan oleh fungsi tersebut. Blok kode yang dijalankan oleh fungsi adalah `return a + b`, yang akan mengembalikan hasil penjumlahan dari `a` dan `b`.

## Memanggil Fungsi
Untuk memanggil sebuah fungsi, cukup tuliskan nama fungsi diikuti dengan tanda kurung `()` dan argumen (jika ada) di dalam tanda kurung tersebut.

Contoh:
```
let hasil = tambah(3, 4);
console.log(hasil); // output: 7
```
Di contoh di atas, kita memanggil fungsi `tambah` dengan mengirimkan nilai `3` dan `4` sebagai argumen. Hasil dari penjumlahan tersebut kemudian disimpan di dalam variabel `hasil`, yang kemudian di-print ke console.

## Fungsi Tanpa Parameter
Fungsi pada JavaScript juga bisa didefinisikan tanpa parameter. Dalam hal ini, tanda kurung `()` tetap harus dituliskan setelah nama fungsi.

Contoh:
```
function halo() {
  console.log("Halo!");
}

halo(); // output: "Halo!"
```
Di contoh di atas, fungsi `halo` didefinisikan tanpa parameter. Ketika fungsi tersebut dipanggil, blok kode di dalamnya akan dijalankan dan `"Halo!"` akan di-print ke console.

## Fungsi Tanpa Nilai Kembali (Void)
Fungsi pada JavaScript bisa saja tidak mengembalikan nilai apapun. Dalam hal ini, nilai kembali dari fungsi tersebut adalah `undefined`.

Contoh:
```
function sapa(nama) {
  console.log("Halo, " + nama + "!");
}

let hasil = sapa("John"); // output: "Halo, John!"
console.log(hasil); // output: undefined
```
Di contoh di atas, fungsi `sapa` hanya menge-print pesan ke console dan tidak mengembalikan nilai apapun. Ketika kita mencoba menyimpan hasil pemanggilan fungsi ke dalam variabel `hasil`, nilai dari variabel tersebut adalah `undefined`.

## Fungsi Anonim
Selain mendefinisikan fungsi dengan nama, kita juga bisa mendefinisikan fungsi tanpa nama yang disebut fungsi anonim. Fungsi anonim biasanya digunakan sebagai argumen dari fungsi lain, atau disimpan di dalam variabel.

Contoh:
```
let jumlah = function(a, b) {
  return a + b;
};

console.log(jumlah(2, 3)); // output
```