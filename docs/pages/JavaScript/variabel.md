# Variabel

Variabel adalah tempat untuk menyimpan data dalam program. Setiap variabel memiliki nama yang unik dan nilai yang dapat berubah-ubah selama program berjalan. Nilai variabel dapat berupa angka, string, objek, dan tipe data lainnya.

## Deklarasi Variabel

Bagaimana keywordi let, const, dan var Bekerja di JavaScript
di era JavaScript pra-ES6 yang lama, pengembang biasa mendeklarasikan variabel menggunakan kata kunci `var` atau tanpa kata kunci apa pun. 
Dengan ES6 (EcmaScript 2015), awal era modern dalam JavaScript, bahasa tersebut mendapatkan dua kata kunci baru untuk membantu kami mendeklarasikan variabel. Ini adalah `let` dan `const`.


- Cara Mendeklarasikan Variabel di JavaScript
Dalam JavaScript, kita dapat mendeklarasikan variabel dengan tiga cara berbeda seperti ini, kita bisa menggunakan kata kunci `var`, `let`, atau `const.`

```
// menggunakan var
var nama = "John Doe";

// menggunakan let
let usia = 25;

// menggunakan const
const PI = 3.14;
```

Ketiga kata kunci ini memiliki perbedaan dalam cara variabel tersebut bisa diubah dan diakses:

- `var`: variabel yang dideklarasikan dengan `var` bisa diakses dan diubah nilainya di mana saja di dalam fungsi tempat variabel tersebut dideklarasikan. Variabel yang dideklarasikan dengan `var` juga bisa diakses di luar blok tempat variabel tersebut dideklarasikan. Namun, jika variabel dideklarasikan di luar fungsi, variabel tersebut akan menjadi variabel global.

- `let`: variabel yang dideklarasikan dengan `let` memiliki cakupan blok yang lebih ketat daripada variabel yang dideklarasikan dengan `var`. Variabel yang dideklarasikan dengan `let` hanya bisa diakses dan diubah nilainya di dalam blok tempat variabel tersebut dideklarasikan.

- `const`: variabel yang dideklarasikan dengan `const` juga memiliki cakupan blok yang ketat seperti variabel yang dideklarasikan dengan `let`, tetapi nilainya tidak bisa diubah setelah dideklarasikan. Variabel yang dideklarasikan dengan `const `bersifat konstan dan nilainya tidak bisa diubah di dalam blok tempat variabel tersebut dideklarasikan.

- Urutan aksesibilitas dalam scope dimulai dari yang terendah :
    - `var` : The functional scope level
    - `let`: The block scope level
    - `const` : The block scope level

Gambar di bawah menunjukkan mindmap dari ketiga kata kunci ini dengan mengacu pada scope yang berbeda.
![Gambar1](/assets/img/gambar1.png)

