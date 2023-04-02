Exercise - Project

1. Kita sudah mengetahui bahwa banyaknya user maksimal adalah 100.
Buat sebuah program yang menampilkan teks ‘User ke - 1 … User ke - 100’ pada setiap baris di halaman HTML.
Lakukan FOR LOOP pada Javascript.

for (let user=1; user <=100; user++){ 
    console.log('user ke ' + user);
}
Penjelasan: 
- membuat perulangan menggunakan for
- menentukan nilai awal dengan mendeklarasikan variabel user = 1 karena nilai awal yang diinginkan saat berjalannya loop adalah 1
- mendefinisikan kondisi berjalannya loop user <= 100 karena ingin menampilkan nilai sampai 100
- menambah niai awal sebanyak 1 dengan user++.  
- console.log dengan menampilkan user ke ditambah dengan data user
jadi saat looping berjalan nilai 1 akan dicek di awal karena 1 kurang dari sama dengan 100 maka bernilai true dan ditampilkan di console user ke 1, lalu karena user++ maka ditambah 1 menjadi 2 dan nilai dicek lagi seperti nilai sebelumnya sampai nilai tersebut sama dengan 100 barulah looping akan berhenti.    

2. Lakukan pengulangan menggunakan FOR LOOP untuk melakukan penambahan nilai sebanyak 10 kali.
Nilai awal = 0
Pengulangan = 10 kali
Nilai awal ditambah 2 setiap pengulangan
Tampilan hasil penambahan pada setiap pengulangan

for(let awal=0; awal<=10; awal +=2){
    console.log('perulangan ke ' + awal);
}
Penjelasan: 
- membuat perulangan menggunakan for
- menentukan nilai awal dengan mendeklarasikan variabel awal = 0 karena nilai awal yang diinginkan saat berjalannya loop adalah 0
- mendefinisikan kondisi berjalannya loop awal <= 10 karena ingin menampilkan nilai sampai 10
- menambah niai awal sebanyak 2 dengan awal+=2. 
- console.log dengan menampilkan perulangan ke ditambah dengan data awal
jadi saat looping berjalan nilai 0 akan dicek di awal karena 0 kurang dari sama dengan 10 maka bernilai true dan ditampilkan di console perulangan ke 0, lalu karena user+=2 maka ditambah 2 menjadi 2 dan nilai dicek lagi seperti nilai sebelumnya sampai nilai tersebut sama dengan 10 barulah looping akan berhenti. 

3.  Lakukan pengulangan dengan FOR LOOP yang melakukan iterasi dari 0..20.
Setiap iterasi/pengulangan lakukan pengecekan apakah nilai tersebut ganjil atau genap.
Tampilkan keterangan ganjil dan genap pada sebuah nilai setiap pengulangan

for(let i=0; i<=20; i++){
    if(i%2){
        console.log(i+ ' ganjil')
    }else{
        console.log(i+ ' genap')
    }
}
Penjelasan: 
- membuat perulangan menggunakan for
- menentukan nilai awal dengan mendeklarasikan variabel i = 0 karena nilai awal yang diinginkan saat berjalannya loop adalah 0
- mendefinisikan kondisi berjalannya loop i <= 20 karena ingin menampilkan nilai sampai 20 
- menambah niai i sebanyak 1 dengan i++. 
- membuat if else di dalam for dengan if(1%2) karena jika if memiliki sisa saat dibagi 2 maka akan console.log menampilkan ganjil, jika tidak maka menampilkan genap 
jadi saat looping berjalan nilai 0 akan dicek di awal karena 0 kurang dari sama dengan 20 maka bernilai true maka akan masuk ke pengkondisian if else karena o dibagi 2 = 0 dan tidak sisa maka akan menamplkan 0 genap lalu karena i++ maka ditambah 1 menjadi 1 dan nilai dicek lagi seperti nilai sebelumnya sampai nilai tersebut sama dengan 20 barulah looping akan berhenti.

4. Tampilkan sebuah Konfirmasi Pop Up kepada user menggunakan confirm();
Berikan teks ‘Apakah anda mau mengulang’ pada box confirm
Jika user memilih ‘OK’ maka program akan terus menampilan pop up yang sama
Jika user memilih ‘Cancel’ maka program akan menampilkan teks ‘Perulangan sudah dilakukan sebanyak …(jumlah klik OK yang dilakukan user)
      function myFunction() {
        let i = true;
        let click = 0;
        while (i) {
          i = confirm("Apakah anda mau mengulang?");
          if (i === true) {
            click = click + 1;
          }
        }
        alert("Perulangan sudah dilakukan sebanyak " + click + " kali");
      }
- membuat html lalu menambahkan h1 dan button dengan properti onclick dengan mengambil function myfunction
- membuat function
- mendeklarasikan variabel i=true dan click=0
- menggunakan perulangan while(i) jadi ketika while i karena i = true maka i akan menampilkan confirm() 
- menambahkan if (i=== true) karea i=true maka true === true maka jalankan perintah click = click+ 1 untuk menghitung jumlah klik saat menekan tombol ok begitu seterusnya hingga user menekan tombol cancel. saat menekan cancel akan menampilkan alert jumlah perulangan saat menekan tombol ok

5. Buat sebuah program kuis.
Tampilkan prompt() untuk meminta inputan dari user. Tampilan teks ‘Sebutkan kepanjangan dari nama IB (Impact Byte)?’
Lakukan pengecekan apakah jawaban dari user sudah benar
Jika benar, tampilkan alert ‘Selamat jawaban kamu benar’
Jika salah, lakukan pengulangan untuk menampilkan prompt() yg sama hingga jawaban dari user benar
      function myFunction() {
        let i = 1;
        while (i > 0) {
          let q = prompt("Sebutkan kepanjangan dari nama IB? (Impact Byte)");
          if (q == "Impact Byte") {
            alert("jawaban benar");
            break;
          }
          i++;
        }
      }