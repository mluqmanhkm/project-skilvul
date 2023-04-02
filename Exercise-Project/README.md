# Exercise - Project

Simple program created with html and javascript

## Exercise Loop

1. Kita sudah mengetahui bahwa banyaknya user maksimal adalah 100.

Buat sebuah program yang menampilkan teks ‘User ke - 1 … User ke - 100’ pada setiap baris di halaman HTML.

Lakukan FOR LOOP pada Javascript.

```javascript
for (let user = 1; user <= 100; user++) {
  console.log("user ke " + user);
}
```

Penjelasan:

- menentukan nilai awal dengan mendeklarasikan variabel user = 1 karena nilai awal yang diinginkan saat berjalannya loop adalah 1
- mendefinisikan kondisi berjalannya, loop user <= 100 karena ingin menampilkan nilai sampai 100
- menambah niai awal sebanyak 1 dengan user++.
- console.log dengan menampilkan "user ke " ditambah dengan data user

jadi saat looping berjalan nilai 1 akan dicek di awal karena 1 kurang dari sama dengan 100 maka bernilai true dan akan ditampilkan di console "user ke 1", lalu karena user++ maka ditambah 1 menjadi 2 dan nilai dicek lagi seperti nilai sebelumnya sampai nilai tersebut sama dengan 100 barulah looping akan berhenti.
