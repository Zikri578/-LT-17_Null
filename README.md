# -LT-17_Null

`null` adalah nilai yang diberikan kepada variabel di JavaScript jika Anda ingin menunjukkan bahwa variabel tersebut tidak memiliki referensi objek apa pun. Ini juga merupakan tipe data di JavaScript. Nilai `null` digunakan untuk menunjukkan bahwa suatu objek atau variabel sengaja tidak memiliki nilai. Misalnya:

    let x = null;
    console.log(x); // Output: null

    const y = {};
    y.prop = null;
    console.log(y.prop); // Output: null

Pada contoh di atas, variabel x diberikan nilai `null`, sehingga saat kita coba untuk menampilkan nilainya, maka akan menghasilkan `null`. Kita juga mencoba untuk mengubah properti prop dari objek y menjadi `null`, sehingga saat kita coba untuk menampilkan nilainya, maka akan menghasilkan `null`.

Anda dapat mengecek apakah suatu variabel bernilai `null` dengan menggunakan operator pembandingan `===` atau `!==`. Misalnya:

    let x = null;
    if (x === null) {
      console.log('x is null');
    }

    if (x !== null) {
      console.log('x is not null');
    }

Sebagai perbandingan dengan `undefined` , jika variable di deklarasikan tetapi tidak di inisialisasi maka akan di tetapkan nilai `undefined`. Namun jika `null` di berikan ke variable, maka ini merupakan nilai yang di sengaja di berikan.

Anda dapat menggunakan operator pembandingan `===` atau `!==` untuk memeriksa apakah suatu variabel bernilai `null` atau tidak. Anda juga dapat menggunakan fungsi `typeof` untuk mengecek tipe data dari suatu variabel, tetapi fungsi ini akan mengembalikan string `object` jika variabel bernilai `null`. Namun, ini mungkin tidak menjadi cara yang baik untuk memeriksa apakah sebuah variable null atau tidak, sebaiknya gunakan operator pembandingan seperti yang telah dijelaskan sebelumnya. Misalnya:

    let x = null;
    console.log(typeof x); // Output: object

Sama seperti `undefined`, kita harus berhati-hati saat menggunakan null, karena jika kita mencoba untuk mengakses properti atau metode dari suatu objek yang bernilai null akan menghasilkan error. Misalnya:

    let x = null;
    console.log(x.prop); // Output: Uncaught TypeError: Cannot read property 'prop' of null

