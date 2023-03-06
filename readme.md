# Apa yang dimaksud dengan multiple import/export javascript ES6?

Dalam JavaScript, istilah "import" dan "export" digunakan untuk menentukan bagaimana modul diatur dan dibagikan di berbagai bagian aplikasi.<br>
Pernyataan "Import" digunakan untuk memuat modul ke dalam file, sedangkan pernyataan "export" digunakan untuk mengekspos bagian modul untuk digunakan di file lain. multiple import/export mengacu pada kemampuan untuk mengimpor dan mengekspor beberapa item dalam satu pernyataan.<br>

## contoh "import" untuk memuat banyak item dari modul seperti ini:<br>

```javascript
import { item1, item2, item3 } from './myModule';
```

Dalam hal ini, item "item1", "item2", dan "item3" sedang diimpor dari file "myModule".<br>

## contoh "ekspor" untuk mengekspor beberapa item dari modul seperti ini

```javascript
export { item1, item2, item3 };
```

Dalam hal ini, item "item1", "item2", dan "item3" diekspor dari modul.<br><br>
Multiple import/export dapat membuat kode lebih ringkas dan lebih mudah dibaca dengan mengurangi jumlah baris kode yang diperlukan untuk mengimpor atau mengekspor beberapa item<br><br>

## Kapan bisa menggunakan banyak impor/ekspor javascript?

Multiple import/export dapat digunakan setiap kali ada banyak item dalam modul yang perlu diimpor atau diekspor. Ini sering terjadi ketika modul berisi kumpulan fungsi, kelas, atau konstanta terkait yang digunakan di berbagai bagian aplikasi.<br>
Misalnya, modul bernama "utils" yang berisi beberapa fungsi pembantu, serta beberapa konstanta dan kelas:<br>

```javascript
// utils.js

export const PI = 3.14159;

export function square(x) {
  return x * x;
}

export function cube(x) {
  return x * x * x;
}

export class Point {
  constructor(x, y) {
    this.x = x;
    this.y = y;
  }

  distance() {
    return Math.sqrt(this.x * this.x + this.y * this.y);
  }
}
```

Untuk menggunakan item ini di modul lain, bisa menggunakan beberapa pernyataan import seperti :<br>

```javascript
// main.js

import { PI, square, cube, Point } from './utils';

console.log(PI);
console.log(cube(3));

const p = new Point(3, 4);
console.log(p.distance());
```

Dalam contoh ini, menggunakan pernyataan import tunggal untuk mengimpor beberapa item dari modul "utils". Kami kemudian dapat menggunakan item ini dalam kode kami sesuai kebutuhan.<br>
Secara keseluruhan, menggunakan multiple import/export dapat membantu membuat kode Anda lebih modular, lebih mudah dibaca, dan lebih mudah dipelihara, terutama dalam aplikasi besar yang memiliki banyak modul dan file berbeda.
