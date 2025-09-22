# Lab1Web.
Tugas Pemograman Web1 Pertemuan 2
   
    Nama: Burhan Isnain Nur Huda
    NIM: 312410226
    Kelas: TI.24.A.2
    Mata Kuliah: Pemograman Web1
    
#  Latihan HTML Dasar

Repository ini berisi latihan membuat halaman web sederhana menggunakan **HTML dasar**.  
Project ini dibuat sebagai bagian dari praktikum Pemrograman Web.  

#  Struktur File
- `lab1_tag_dasar.html` → Halaman utama, isinya perkenalan singkat dan navigasi ke halaman lain.  
- `lab1_halaman2.html` → Halaman kedua, isinya cerita lebih detail tentang **hobi saya (nge-gym, olahraga fisik, dll)**.  

#  Penjelasan
<img width="1915" height="680" alt="image" src="https://github.com/user-attachments/assets/282dcf25-b9ac-4b26-8cee-64ca550ce9cd" />

#  lab1_tag_dasar.html
Halaman ini bisa dibilang sebagai **pintu masuk**.  
 Ada judul `<h1>` buat nunjukin nama.  
 Paragraf perkenalan singkat tentang diri saya.  
 Logo kampus ditampilkan pakai `<img>`.  
 Navigasi `<nav>` buat pindah ke halaman 2.  
 Footer di bawah buat nandain hak cipta.  

#  lab1_halaman2.html
Halaman ini fokusnya **ngejelasin hobi lebih detail**.  
 Judul `<h1>` tentang hobi saya.  
 Subjudul `<h2>` untuk ngebagi konten: "Nge-Gym" sama "Olahraga Outdoor".  
 Ada paragraf cerita kenapa suka olahraga.  
 Gambar olahraga biar tampilannya lebih hidup.  
 Navigasi balik ke halaman utama.  
 Footer biar rapi.  

# Tujuan
 Melatih penggunaan **tag dasar HTML** kayak `<h1>`, `<p>`, `<img>`, `<nav>`, dan `<footer>`.  
 Belajar bikin struktur web sederhana dengan **multi-halaman**.  

#  Preview
Kalau dijalankan di browser:
1. Buka `lab1_tag_dasar.html` → bakal lihat halaman perkenalan.  
2. Klik menu navigasi → pindah ke `lab1_halaman2.html` buat lihat detail hobi.  

Jawaban Pertanyaan


```1.Lakukan perubahan pada kode sesuai dengan keinginan anda, amati perubahannya adakah error ketika terjadi kesalahan penulisan tag?```

Kalau kita ubah isi kode (misalnya mengganti teks, menambah paragraf, atau mengganti gambar) hasil di browser akan ikut berubah.
Tapi kalau ada kesalahan penulisan tag (misalnya <p> ditulis <pp>, atau lupa menutup tag), biasanya:
Browser tetap berusaha menampilkan halaman, tapi tampilannya bisa jadi berantakan.
Tidak muncul pesan error langsung, tapi struktur HTML jadi tidak sesuai aturan.

2.Apa perbedaan dari ```tag <p> dengan tag <br>,``` berikan penjelasannya!
yaitu ```<p>``` digunakan untuk membuat paragraf baru. Browser otomatis memberi jarak (spasi) sebelum dan sesudah paragraf.
```<br>``` digunakan untuk membuat baris baru (line break) tanpa jarak tambahan. Jadi teks langsung turun ke bawah tapi masih dalam paragraf yang sama.
     
    Contoh:  
    `<p>Ini paragraf pertama.</p>`
    `<p>Ini paragraf kedua.</p>`
    `Baris pertama <br> Baris kedua `

3.Apa perbedaan atribut `title` dan `alt` pada tag `<img>`?
`title` → teks yang muncul saat kursor diarahkan ke gambar (tooltip).  
`alt` → teks alternatif yang muncul kalau gambar gagal dimuat (misalnya file gambar hilang). Selain itu, `alt` juga dipakai oleh screen reader (aksesibilitas).  


    Contoh:  
    `<img src="gym.jpg" title="Latihan Gym" alt="Gambar orang sedang fitness"> ```

4.Untuk mengatur ukuran gambar, digunakan atribut `width dan height`. Agar tampilan gambar proporsional sebaiknya kedua atribut tersebut diisi semua atau tidak?

Sebaiknya cukup salah satu saja yang diisi `(biasanya width).`
Kalau `width dan height` diisi sembarangan, gambar bisa jadi gepeng atau melebar tidak sesuai proporsi aslinya.
Kalau hanya `width` diisi → browser otomatis menyesuaikan `height` agar tetap proporsional.

5.Pada link tambahkan atribut target dengan nilai atribut bervariasi `(_blank, _self, _top, _parent)`, apa yang terjadi pada masing-masing nilai atribut tersebut?

`_blank` yaitu untuk buka link di tab/jendela baru.

`_self` yaitu untuk buka link di halaman yang sama (default).

`_top` yaitu untuk buka link di jendela penuh, menghapus semua frame (kalau pakai frame).

`_parent` yaitu untuk buka link di halaman induk (kalau ada frame dalam frame).

Contoh:
``` html
<a href="https://www.google.com" target="_blank">Google (tab baru)</a>
<a href="lab1_tag_dasar.html" target="_self">Halaman Utama</a>
