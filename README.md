# Lab1web
*Nama    : Amelia Nurmala Dewi*

*NIM     : 312410199*

*Kelas   : TI.24.A2*


## Praktikum 1: HTML Dasar

### A. Langkah 1: Membuat Struktur Dasar HTML
<img width="793" height="605" alt="Screenshot (260)" src="https://github.com/user-attachments/assets/6118c299-3cb9-46c2-92e6-1279b87c0d58" />

Pertama saya membuat file `lab1_tag_dasar.html` dengan struktur dasar HTML.  
Di dalamnya saya menambahkan identitas berupa **Nama, Kelas, dan NIM**.  

### B. Langkah 2: Menambahkan Navigasi (Menu Link)
<img width="795" height="600" alt="Screenshot (261)" src="https://github.com/user-attachments/assets/d20c9634-4fd0-4bed-b7be-72d5763fb72a" />

Selanjutnya saya menambahkan tag `<nav>` untuk membuat navigasi berisi link ke:
- `lab1_tag_dasar.html` → Dasar HTML  
- `lab1_halaman2.html` → Halaman 2  
- Website eksternal → Google  

Saya juga menambahkan garis pemisah `<hr>` di bawah link.  

### C. Langkah 3: Membuat Judul dan Paragraf
<img width="796" height="603" alt="Screenshot (262)" src="https://github.com/user-attachments/assets/174349bd-5317-4edb-8b84-7f6ee31ed08c" />

Kemudian saya menambahkan heading `<h1>` dengan teks **Belajar Dasar HTML**.  
Saya juga membuat paragraf yang berisi kalimat penjelasan. Pada paragraf ini saya memberikan format teks:  
- Stabilo kuning menggunakan `<span style="background-color:yellow;">HTML dasar</span>`  
- Huruf miring dengan `<span style="font-style:italic;">Teknik Informatika</span>`  
- Garis bawah dengan `<span style="text-decoration:underline;">Universitas Pelita Bangsa</span>`  

### D. Langkah 4: Menambahkan Sub Judul dan Paragraf Kedua
<img width="800" height="602" alt="Screenshot (263)" src="https://github.com/user-attachments/assets/4f615b4b-4afd-4693-bf97-4798ab559cdb" />

Berikutnya saya membuat sub judul dengan tag `<h2>` berisi **Paragraf pada HTML**.  
Lalu saya menambahkan paragraf baru sebagai contoh penggunaan tag `<p>`.  

### E. Langkah 5: Menambahkan Gambar
<img width="797" height="677" alt="Screenshot (254)" src="https://github.com/user-attachments/assets/b1e3aec5-0ede-48c7-b843-4b9904e832ce" />

Terakhir saya menambahkan heading `<h3>` berisi **Logo Universitas Pelita Bangsa**.  
Kemudian saya menambahkan gambar logo UPB menggunakan tag `<img src="logo_upb.png" width="200">`.  

---


## Jawaban Pertanyaan

### 1. Lakukan perubahan pada kode sesuai dengan keinginan anda, amati perubahannya. Adakah error ketika terjadi kesalahan penulisan tag?
Jawab :

Jika ada kesalahan penulisan tag HTML (misalnya `<p>` ditulis `<pp>`), browser tidak akan menampilkan error secara langsung, tetapi elemen tidak akan berfungsi sebagaimana mestinya.  
* Contoh: `<pp>Ini teks</pp>` hanya ditampilkan sebagai teks biasa, bukan paragraf.  
* HTML bersifat toleran (forgiving), jadi tidak muncul pesan error, tetapi hasil tampilan bisa tidak sesuai harapan.

---

### 2. Apa perbedaan dari tag `<p>` dengan tag `<br>`?
Jawab :

- `<p>` digunakan untuk membuat paragraf baru. Saat digunakan, otomatis memberi jarak (spasi) antar paragraf.  
- `<br>` digunakan untuk pindah baris di dalam paragraf tanpa memberi jarak tambahan.

**Contoh:**
```html
<p>Ini paragraf pertama.</p>
<p>Ini paragraf kedua.</p>
```
Hasil: ada jarak antar paragraf.

```html
Ini baris pertama.<br>
Ini baris kedua.
```
Hasil: hanya pindah baris, tanpa jarak tambahan.

---

### 3. Apa perbedaan atribut `title` dan `alt` pada tag `<img>`?
Jawab :

* `alt` adalah teks alternatif yang muncul jika gambar gagal dimuat, dan juga digunakan oleh screen reader.
* `title` adalah teks yang muncul sebagai tooltip saat kursor diarahkan ke gambar.

**Contoh:**

```html
<img src="logo.png" alt="Logo Universitas Pelita Bangsa" title="Ini logo UPB">
```

Jika gambar gagal dimuat: muncul teks "Logo Universitas Pelita Bangsa".
Jika gambar tampil dan diarahkan kursor: muncul tooltip "Ini logo UPB".

---

### 4. Untuk mengatur ukuran gambar, digunakan atribut `width` dan `height`. Agar tampilan gambar proporsional sebaiknya kedua atribut tersebut diisi semua atau tidak?
Jawab :

Tidak harus diisi semua.

* Jika hanya salah satu atribut diisi (misalnya `width`), maka browser otomatis menyesuaikan yang lain agar proporsional.
* Jika keduanya diisi dengan nilai yang tidak sesuai rasio asli gambar, maka gambar bisa tampak gepeng atau melebar.

Jadi sebaiknya cukup isi salah satu (biasanya `width`) agar gambar tetap proporsional.

---

### 5. Pada link tambahkan atribut `target` dengan nilai bervariasi (`_blank`, `_self`, `_top`, `_parent`). Apa yang terjadi pada masing-masing nilai atribut tersebut?
Jawab :

* `target="_blank"` → membuka link di tab/jendela baru.
* `target="_self"` → membuka link di tab/jendela yang sama (default).
* `target="_top"` → membuka link di jendela penuh, keluar dari semua frame.
* `target="_parent"` → membuka link di frame induk (jika halaman menggunakan frame).

**Contoh kode:**

```html
<a href="http://google.com" target="_blank">Buka di Tab Baru</a>
<a href="http://google.com" target="_self">Buka di Tab Sama</a>
<a href="http://google.com" target="_top">Buka di Jendela Penuh</a>
<a href="http://google.com" target="_parent">Buka di Frame Induk</a>
```





