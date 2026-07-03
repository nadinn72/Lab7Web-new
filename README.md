# Lab7Web.
Nama: Nadine Amelia Putri 

Nim: 312410188

# Praktikum 1 

## 1. Konfigurasi Ekstensi PHP
**- Buka XAMPP Control Panel → Apache → Config → PHP.ini**

**- Aktifkan ekstensi: php-json, php-mysqlnd, php-xml, php-intl, libcurl**

**- Hapus tanda ; di depan nama ekstensi, simpan, lalu restart Apache.**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 103106" src="https://github.com/user-attachments/assets/011aaa26-f0ea-4f51-a699-5b3513cf5922" />

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 103452" src="https://github.com/user-attachments/assets/f0ea0196-23dd-42bc-8bf7-26c3ad58ac54" />


## 2. Instalasi Codeigniter 4
**- Unduh dari https://codeigniter.com/download**

**- Ekstrak ke htdocs/lab11_ci/**

**- Ubah nama folder framework-4.x.xx menjadi ci4**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 103609" src="https://github.com/user-attachments/assets/b6742a60-3fd5-45f1-b9a4-125e023cc284" />

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 105724" src="https://github.com/user-attachments/assets/c1439802-b239-405b-b1e0-7fd707f15106" />

**- Akses http://localhost/lab11_ci/ci4/public/**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 110005" src="https://github.com/user-attachments/assets/cf6ebec0-5b4e-4399-b83e-2ab3fe13f0f1" />

## 3. Menjalankan CLI (Command Line Interface)
**- Codeigniter 4 menyediakan CLI untuk mempermudah proses development. Untuk mengakses
CLI buka terminal/command prompt.**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 110347" src="https://github.com/user-attachments/assets/4c0ec1fd-38da-4ea8-938d-1d6f39bef09b" />

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 110453" src="https://github.com/user-attachments/assets/d938b37b-a4e4-42fd-add1-3ef0bf6c1c40" />


## 4. Mengaktifkan Mode Debugging
**- Codeigniter 4 menyediakan fitur debugging untuk memudahkan developer untuk mengetahui
pesan error apabila terjadi kesalahan dalam membuat kode program.**

**- Secara default fitur ini belum aktif. Ketika terjadi error pada aplikasi akan ditampilkan pesan
kesalahan seperti berikut.**


<img width="800" height="400" alt="Cuplikan layar 2026-03-30 133213" src="https://github.com/user-attachments/assets/c14a2ca7-33b6-4759-b07e-f1b41f7b8614" />

**- Semua jenis error akan ditampilkan sama. Untuk memudahkan mengetahui jenis errornya,
maka perlu diaktifkan mode debugging dengan mengubah nilai konfigurasi pada environment
variable CI_ENVIRONMENT menjadi development.**


<img width="884" height="211" alt="image" src="https://github.com/user-attachments/assets/a972cb2f-127f-4692-a27f-95a9c89a9a32" />


**- Ubah nama file env menjadi .env**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 105757" src="https://github.com/user-attachments/assets/a90a77b5-1512-442f-80a5-1549d13d048c" />


<img width="800" height="400" alt="Cuplikan layar 2026-03-30 105816" src="https://github.com/user-attachments/assets/58238284-052c-46c3-931f-cef523082c1e" />

**- Contoh error yang terjadi. Untuk mencoba error tersebut, ubah kode pada file
app/Controller/Home.php hilangkan titik koma pada akhir kode.**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 140400" src="https://github.com/user-attachments/assets/cf99e39c-0669-4c0f-8f7a-eb550167c8fd" />


<img width="800" height="400" alt="Cuplikan layar 2026-03-30 140410" src="https://github.com/user-attachments/assets/10ded210-ee0a-49ff-866e-0f39fd9e10f3" />

**- berikut adalah contoh error yang terjadi**

<img width="800" height="600" alt="Cuplikan layar 2026-03-30 140556" src="https://github.com/user-attachments/assets/b40fcd27-cb14-4f93-b205-94dbcff4a5c6" />

## 5. Menambahkan Route Baru
**- Buka app/config/Routes.php**

**- Tambahkan kode:**

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/7b2dfd32-5567-4995-a961-431e199ebe57" />


## 6. Cek Route dengan CLI
**- Buka terminal/CMD, arahkan ke C:\xampp\htdocs\lab11_ci\ci4**

**- Jalankan: php spark routes**

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/a84b58e5-6c1f-4d40-a8eb-18f13306f282" />

**- Selanjutnya coba akses route yang telah dibuat dengan mengakses alamat url**
```
**http://localhost:8080/about**
```

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 141418" src="https://github.com/user-attachments/assets/b5cccc21-33e9-4957-baf2-5109aedd815a" />

## 7. Membuat Controller
**- Selanjutnya adalah membuat Controller Page.** 

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/c2175608-d738-4899-a35d-617716c2ec9c" />

**- Selanjutnya refresh Kembali browser, maka akan ditampilkan hasilnya yaitu halaman sudah
dapat diakses.**


<img width="800" height="400" alt="Cuplikan layar 2026-03-30 142106" src="https://github.com/user-attachments/assets/d61e53e2-e263-4be0-9ab9-d20af0dbeb20" />

## 8. Auto Routing
**Secara default fitur autoroute pada Codeiginiter sudah aktif. Untuk mengubah status autoroute
dapat mengubah nilai variabelnya. Untuk menonaktifkan ubah nilai true menjadi false.**

``` $routes->setAutoRoute(true); ```

**- Tambahkan method baru pada Controller Page seperti berikut.**

**- Method ini belum ada pada routing, sehingga cara mengaksesnya dengan menggunakan
alamat: http://localhost:8080/page/tos**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 143154" src="https://github.com/user-attachments/assets/67229d18-2f32-472b-a51e-4529ca374736" />

## 9. Membuat View dan Layout
**- Selanjutnya adalam membuat view untuk tampilan web agar lebih menarik.**

**- Buat file barudengan nama about.php pada direktori view (app/view/about.php)**

**- Ubah method about pada class Controller Page**

**- Kemudian lakukan refresh pada halaman tersebut**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 143923" src="https://github.com/user-attachments/assets/99416ef6-381d-4236-8bd7-dc0b07c64799" />

## 10. Menambahkan CSS Layout (dari praktikum 4)
**- Pada dasarnya layout web dengan css dapat diimplamentasikan dengan mudah pada
codeigniter.**

**- Yang perlu diketahui adalah, pada Codeigniter 4 file yang menyimpan asset css
dan javascript terletak pada direktori public.**

**- Copy file style.css dari praktikum 4 ke public/**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 144008" src="https://github.com/user-attachments/assets/d074821a-13eb-42ed-b64d-e91b50007a6a" />


## 11. Menggabungkan View dengan Layout
**- Buat folder app/Views/template/**

**- Buat header.php dan footer.php**

**- Refresh halaman about → tampilan jadi lebih rapi dengan CSS:**
<img width="800" height="600" alt="Cuplikan layar 2026-03-30 145721" src="https://github.com/user-attachments/assets/8e9c236c-8f6f-4cb3-95e8-7330961bfa54" />


# Praktikum 2

## 1. Membuat Database dan Tabel
**- Jalankan MySQL melalui XAMPP Control Panel (Start MySQL)**

**- Buka phpMyAdmin atau CLI MySQL**

**- Buat database:**
```CREATE DATABASE lab_ci4;```

<img width="200" height="150" alt="image" src="https://github.com/user-attachments/assets/b8d93b53-12a4-4ff9-88ae-e83f3693871d" />

**- Buat tabel artikel:**
<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/a34af13e-6dc6-497d-9786-957d81bd2093" />


## 2. Konfigurasi Database di .env
**- Selanjutnya membuat konfigurasi untuk menghubungkan dengan database server.**

**- Konfigurasi dapat dilakukan dengan du acara, yaitu pada file app/config/database.php atau menggunakan file .env.**

**- Pada praktikum ini kita gunakan konfigurasi pada file .env pada root proyek CI4 (C:\xampp\htdocs\lab11_ci\ci4)**

**- Pada Tahapan ini berperan penting agar aplikasi bisa terhubung ke database.**

## 3. Membuat Model Artikel
**- Buat file app/Models/ArtikelModel.php**

**- Model ini akan digunakan untuk mengambil, menyimpan, mengupdate, dan menghapus data dari tabel artikel**

## 4. Membuat Controller Artikel
**- Buat file app/Controllers/Artikel.php**

**- Method index(): Memanggil model, mengambil semua data artikel dengan findAll(), lalu mengirim ke view artikel/index.**

## 5. Membuat View Index Artikel
**- Buat folder app/Views/artikel/**

**- Buat file index.php di dalam folder tersebut**

**- Buat folder template untuk header dan footer**

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/58223988-7aa8-4fd2-a8de-3cc3ca8678d2" />


## 6. Menambahkan Data Awal ke Database
**- Jalankan SQL melalui phpMyAdmin atau CLI:**
**Akses** ``http://localhost:8080/artikel``

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/b44b36ee-45b4-437f-81bb-c21496181769" />

## 7. Menambahkan Method view di Controller
**- Tambahkan kode di Artikel.php**

## 8. Membuat View Detail
**- Buat file app/Views/artikel/detail.php, untuk menghasilkan berikut**

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/214570c9-b475-4be5-93b0-0cf928a73e0f" />

## 9. Menambahkan Routing untuk Detail
**- Buka app/config/Routes.php**

**- Klik judul artikel di halaman daftar, seharusnya menampilkan detail.**

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/a9707b64-909e-4145-a897-bc28d054505f" />


## Membuat Menu Admin (CRUD)
## 10. Menambahkan Method admin_index
## 11. Membuat View Admin Index
**- Buat file app/Views/artikel/admin_index.php**
**- Tambahkan template admin_header dan admin_footer**

## 12. Routing untuk Group Admin
**- Tambahkan code di Routes.php**
**Akses** ``http://localhost:8080/admin/artikel``

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/becb523b-d0e5-46fa-a938-b922b435fae8" />


## 13. Menambah Data (Method add)
**- Menambahkan code di Artikel.php**

**- Buat view form_add.php di app/Views/artikel/:**

**- Coba tambah artikel baru,**

<img width="800" height="400" alt="Cuplikan layar 2026-05-22 120511" src="https://github.com/user-attachments/assets/d06cd669-ae29-43c4-8675-ca27139e1cae" />

**- lalu cek di halaman admin dan di halaman depan.**

<img width="800" height="400" alt="Cuplikan layar 2026-05-22 120547" src="https://github.com/user-attachments/assets/354c2bee-fbfb-4265-be98-76ba2bc460cf" />


## 14. Mengubah Data (Method edit)
**- Menambahkan code di Artikel.php**

**- Buat view form_edit.php:**

**Uji coba ubah data,**

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/d388446c-b557-4bb7-a376-06d75a158a33" />

**- Memastikan bahwa berhasil mengubah data**

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/3b4a6f04-ced7-4613-9c2e-e6b8eaec0138" />

## 15. Menghapus Data (Method delete)
**- Menambahkan code di Artikel.php**

**- Coba klik tombol Hapus pada halaman admin, konfirmasi, lalu data terhapus.**

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/b66bfb60-0218-4333-b45d-bbdb2262897d" />

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/58efc6ea-6a1f-4094-bfc5-ca11b8f1eba8" />


# Praktikum 3

## 1 Membuat Layout Utama
**Buat folder layout di dalam app/Views/**

**Buat file main.php di dalam folder layout dengan kode berikut:**

**Layout ini akan digunakan untuk semua halaman agar tampilan konsisten (header, nav, sidebar, footer).**

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title><?= $title ?? 'My Website' ?></title>
    <link rel="stylesheet" href="<?= base_url('/style.css');?>">
</head>
<body>
    <div id="container">
        <header>
            <h1>Layout Sederhana</h1>
    </header>
    <nav>
        <a href="<?= base_url('/');?>" class="active">Home</a>
        <a href="<?= base_url('/artikel');?>">Artikel</a>
        <a href="<?= base_url('/about');?>">About</a>
        <a href="<?= base_url('/contact');?>">Kontak</a>
    </nav>
    <section id="wrapper">
        <section id="main">
                <?= $this->renderSection('content') ?>
            </section>
            <aside id="sidebar">
                <?= view_cell('App\\Cells\\ArtikelTerkini::render') ?>
                <div class="widget-box">
                    <h3 class="title">Widget Header</h3>
                    <ul>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                    </ul>
                </div>
                <div class="widget-box">
                    <h3 class="title">Widget Text</h3>
                    <p>Vestibulum lorem elit, iaculis in nisl volutpat,
                    malesuada tincidunt arcu. Proin in leo fringilla,
                    vestibulum mi porta,
                    faucibus felis. Integer pharetra est nunc, nec pretium
                    nunc pretium ac.</p>
                </div>          
            </aside>
        </section>
        <footer>
            <p>&copy; 2026 - Universitas Pelita Bangsa</p>
        </footer>
    </div>
</body>
</html>
```

## 2. Modifikasi File View
**Ubah app/Views/home.php agar sesuai dengan layout baru:**

**Sesuaikan juga untuk halaman lainnya yang ingin menggunakan format layout yang baru.**

```
<?= $this->extend('layout/main') ?>
<?= $this->section('content') ?>
<h1><?= $title; ?></h1>
<hr>
<p><?= $content; ?></p>
<?= $this->endSection() ?>
```

## 3. Menampilkan Data Dinamis dengan View Cell
**View Cell adalah fitur yang memungkinkan pemanggilan tampilan dalam bentuk komponen
yang dapat digunakan ulang. Cocok digunakan untuk elemen-elemen yang sering muncul di
berbagai halaman seperti sidebar, widget, atau menu navigasi.**

## a. Membuat Class View Cell
**Buat folder Cells di dalam app/**

**Buat file ArtikelTerkini.php di dalam app/Cells/ dengan kode berikut:**

```
<?php

namespace App\Cells;

use CodeIgniter\View\Cells\Cell;
use App\Models\ArtikelModel;

class ArtikelTerkini extends Cell
{
    protected $kategori = null;
    protected $limit = 5;

    public function mount($kategori = null, $limit = 5)
    {
        $this->kategori = $kategori;
        $this->limit = $limit;
    }

    public function render()
    {
        $model = new ArtikelModel();
        
        $query = $model->orderBy('created_at', 'DESC');
        
        // Filter berdasarkan kategori (bisa dikembangkan dengan menambah kolom kategori)
        if ($this->kategori) {
            $query->like('judul', $this->kategori);
        }
        
        $artikel = $query->findAll($this->limit);
        
        return view('components/artikel_terkini', [
            'artikel' => $artikel,
            'kategori' => $this->kategori
        ]);
    }
}
```

## b. Membuat View untuk View Cell
**Buat folder components di dalam app/Views/**

**Buat file artikel_terkini.php di dalam app/Views/components/ dengan kode berikut:**

```
<div class="widget-box">
    <h3 class="title">
        Artikel Terkini 
        <?= $kategori ? "<small>($kategori)</small>" : '' ?>
    </h3>
    <ul>
        <?php if (!empty($artikel)): ?>
            <?php foreach ($artikel as $row): ?>
                <li>
                    <a href="<?= base_url('/artikel/' . $row['slug']); ?>">
                        <?= esc($row['judul']); ?>
                    </a>
                    <br>
                    <small><?= date('d/m/Y', strtotime($row['created_at'])); ?></small>
                </li>
            <?php endforeach; ?>
        <?php else: ?>
            <li>Belum ada artikel</li>
        <?php endif; ?>
    </ul>
</div>
```

# Pertanyaan dan Tugas Praktikum 3

## A. Apa manfaat utama dari penggunaan View Layout dalam pengembangan aplikasi?

**Manfaat utama View Layout:**

- Konsistensi Tampilan - Seluruh halaman memiliki struktur header, footer, dan sidebar yang sama

- Efisiensi Kode - Tidak perlu menulis ulang kode template yang sama di setiap halaman

- Kemudahan Maintenance - Perubahan pada layout cukup dilakukan di satu file

- Modularitas - Memisahkan konten utama dari struktur template

- Reusability - Komponen layout dapat digunakan kembali di berbagai halaman

- DRY Principle (Don't Repeat Yourself) - Menghindari duplikasi kode

## B. Jelaskan perbedaan antara View Cell dan View biasa

**View Biasa**

View biasa adalah tampilan untuk halaman utuh, seperti halaman home, artikel, atau about. Semua data dan logika disiapkan oleh Controller. View ini tidak bisa berdiri sendiri karena bergantung pada Controller. Jika ingin dipakai ulang, harus di-include secara manual. Cocok untuk halaman yang utuh dan sederhana.

**View Cell**

View cell adalah komponen kecil yang mandiri, seperti sidebar, widget, atau menu dinamis. Dia bisa memproses datanya sendiri tanpa bantuan Controller. Cukup panggil dengan fungsi view_cell() kapan saja dan di mana saja. View cell mudah dipindahkan antar proyek karena semua logika sudah terbungkus dalam kelas Cell sendiri.

## C. Cara mengubah View Cell agar hanya menampilkan post dengan kategori tertentu

**Sudah diimplementasikan pada class ArtikelTerkini di atas. Berikut contoh penggunaannya:**

```
php
// Memanggil View Cell dengan filter kategori tertentu
<?= view_cell('App\\Cells\\ArtikelTerkini::render', ['kategori' => 'teknologi']) ?>
<?= view_cell('App\\Cells\\ArtikelTerkini::render', ['kategori' => 'pendidikan']) ?>

// Tanpa filter (menampilkan semua)

<?= view_cell('App\\Cells\\ArtikelTerkini::render') ?>
```

**Penjelasan implementasi:**

- Menambahkan properti $kategori pada class Cell

- Method mount($kategori = null) untuk menerima parameter

- Query menggunakan where('kategori', $this->kategori) jika parameter diberikan


# Praktikum 4

## 1.  Membuat Tabel User
Membuat tabel baru bernama user di dalam database.
Struktur tabel terdiri dari:
id : sebagai primary key dan auto increment
username : untuk menyimpan nama pengguna
useremail : untuk menyimpan alamat email
userpassword : untuk menyimpan password yang akan di-hash
Tabel ini berfungsi sebagai tempat penyimpanan data akun pengguna yang akan melakukan login.

<img width="1622" height="452" alt="Cuplikan layar 2026-04-01 100813" src="https://github.com/user-attachments/assets/db0838ec-1ccb-43f4-9415-4c95741c66d3" />

## 2. Membuat Model User
Membuat file model dengan nama UserModel di dalam direktori app/Models.
Model ini menghubungkan aplikasi dengan tabel user di database.
Mendefinisikan tabel yang digunakan, primary key, dan field-field yang boleh diisi (username, useremail, userpassword).
Model ini akan digunakan untuk melakukan operasi database seperti mengambil data pengguna berdasarkan email.

## 3. Membuat Controller User
Membuat controller baru bernama User di dalam direktori app/Controllers.
Di dalam controller ini terdapat dua method utama:

**a. Method index()**

Berfungsi untuk menampilkan daftar seluruh pengguna yang terdaftar.
Mengambil semua data user dari database melalui model.
Menampilkan data tersebut ke dalam view.

**b. Method login()**

Berfungsi untuk menangani proses login.
Jika belum ada data yang dikirim (email kosong), maka akan menampilkan form login.
Jika email sudah diisi, sistem akan melakukan pencarian data pengguna berdasarkan email yang dimasukkan.
Jika email ditemukan, sistem akan memeriksa kecocokan password menggunakan fungsi verifikasi hash.
Jika password cocok, sistem akan menyimpan data sesi (user id, username, email, dan status logged_in) dan mengarahkan ke halaman admin.
Jika password salah, akan muncul pesan error "Password salah".
Jika email tidak ditemukan, akan muncul pesan error "Email tidak terdaftar".
Pesan error ditampilkan menggunakan flash message.


## 4. Membuat View Login
Membuat direktori baru bernama user di dalam app/views.
Membuat file login.php sebagai halaman login.
Halaman login berisi:
Form dengan dua input: email dan password.
Tombol login untuk mengirimkan data.
Area untuk menampilkan flash message jika terjadi error.
Tampilan menggunakan CSS sederhana yang sudah disediakan.

## 5. Membuat Database Seeder
Membuat seeder dengan nama UserSeeder melalui command line (CLI).
Seeder berfungsi untuk mengisi data dummy ke dalam database.
Data yang dimasukkan adalah satu akun contoh:
Username: admin
Email: admin@email.com
Password: admin123 (akan di-hash sebelum disimpan)
Menjalankan seeder melalui CLI agar data langsung masuk ke tabel user di database.

## 6. Uji Coba Login
Membuka halaman login melalui browser (http://localhost:8080/user/login).
Mencoba login dengan akun yang sudah dibuat melalui seeder.
Jika berhasil, akan diarahkan ke halaman admin.
Jika gagal, akan muncul pesan error sesuai penyebabnya (password salah atau email tidak terdaftar).

<img width="800" height="400" alt="Cuplikan layar 2026-06-11 143029" src="https://github.com/user-attachments/assets/2963e77b-0f6d-4030-8cfc-7a450b1f16ba" />

8. Menambahkan Auth Filter
Membuat file filter baru bernama Auth di dalam direktori app/Filters.
Filter ini berfungsi untuk melakukan pengecekan sebelum mengakses halaman tertentu.

9. Percobaan Akses Menu Admin
Membuka url halaman admin (http://localhost:8080/admin/artikel) secara langsung tanpa login terlebih dahulu.
Karena filter Auth sudah aktif, maka secara otomatis akan diarahkan ke halaman login.
Setelah login berhasil, baru bisa mengakses halaman admin tersebut.

<img width="800" height="400" alt="Cuplikan layar 2026-06-11 143237" src="https://github.com/user-attachments/assets/6c222b87-662f-4fb7-af38-b7a95e2aabda" />

11. Fungsi Logout
Menambahkan method logout pada controller User.
Fungsi logout bekerja dengan:
Menghapus semua data sesi yang tersimpan (session destroy).
Mengarahkan pengguna kembali ke halaman login.
Dengan demikian, setelah logout, pengguna tidak bisa mengakses halaman admin lagi sampai login ulang.

<img width="800" height="400" alt="Cuplikan layar 2026-06-11 143237" src="https://github.com/user-attachments/assets/6832b94f-bd8a-44c3-948a-fa16a1f5832b" />




Berikut adalah praktikum 5-14

https://github.com/nadinn72/Lab11Web_VueJS.git





