# Lab7Web.
Nama: Nadine Amelia Putri 

Nim: 312410188

**Untuk mengaktifkan ekstentsi,dapat melalui XAMPP Control Panel, pada bagian Apache klik Config -> PHP.ini**
<img width="800" height="400" alt="Cuplikan layar 2026-03-30 103106" src="https://github.com/user-attachments/assets/011aaa26-f0ea-4f51-a699-5b3513cf5922" />


**Pada bagian extention, hilangkan tanda ; (titik koma) pada ekstensi yang akan diaktifkan.**
**Kemudian simpan kembali filenya dan restart Apache web server.**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 103452" src="https://github.com/user-attachments/assets/f0ea0196-23dd-42bc-8bf7-26c3ad58ac54" />


- **Unduh Codeigniter dari website https://codeigniter.com/download**
- **Extrak file zip Codeigniter ke direktori htdocs/lab11_ci.**
- **Ubah nama direktory framework-4.x.xx menjadi ci4.**
- **Buka browser dengan alamat http://localhost/lab11_ci/ci4/public/**
<img width="800" height="400" alt="Cuplikan layar 2026-03-30 103609" src="https://github.com/user-attachments/assets/b6742a60-3fd5-45f1-b9a4-125e023cc284" />

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 105724" src="https://github.com/user-attachments/assets/c1439802-b239-405b-b1e0-7fd707f15106" />

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 110005" src="https://github.com/user-attachments/assets/cf6ebec0-5b4e-4399-b83e-2ab3fe13f0f1" />

## Menjalankan CLI (Command Line Interface)
Codeigniter 4 menyediakan CLI untuk mempermudah proses development. Untuk mengakses
CLI buka terminal/command prompt. 

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 110347" src="https://github.com/user-attachments/assets/4c0ec1fd-38da-4ea8-938d-1d6f39bef09b" />

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 110453" src="https://github.com/user-attachments/assets/d938b37b-a4e4-42fd-add1-3ef0bf6c1c40" />


## Mengaktifkan Mode Debugging
Codeigniter 4 menyediakan fitur debugging untuk memudahkan developer untuk mengetahui
pesan error apabila terjadi kesalahan dalam membuat kode program.
Secara default fitur ini belum aktif. Ketika terjadi error pada aplikasi akan ditampilkan pesan
kesalahan seperti berikut.

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 133213" src="https://github.com/user-attachments/assets/c14a2ca7-33b6-4759-b07e-f1b41f7b8614" />

**Semua jenis error akan ditampilkan sama. Untuk memudahkan mengetahui jenis errornya,
maka perlu diaktifkan mode debugging dengan mengubah nilai konfigurasi pada environment
variable CI_ENVIRONMENT menjadi development.**
<img width="884" height="211" alt="image" src="https://github.com/user-attachments/assets/a972cb2f-127f-4692-a27f-95a9c89a9a32" />

**Ubah nama file env menjadi .env kemudian buka file tersebut dan ubah nilai variable
CI_ENVIRINMENT menjadi development**
<img width="800" height="400" alt="Cuplikan layar 2026-03-30 105757" src="https://github.com/user-attachments/assets/a90a77b5-1512-442f-80a5-1549d13d048c" />

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 105816" src="https://github.com/user-attachments/assets/58238284-052c-46c3-931f-cef523082c1e" />

**Contoh error yang terjadi. Untuk mencoba error tersebut, ubah kode pada file
app/Controller/Home.php hilangkan titik koma pada akhir kode.**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 140400" src="https://github.com/user-attachments/assets/cf99e39c-0669-4c0f-8f7a-eb550167c8fd" />

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 140410" src="https://github.com/user-attachments/assets/10ded210-ee0a-49ff-866e-0f39fd9e10f3" />


<img width="800" height="600" alt="Cuplikan layar 2026-03-30 140556" src="https://github.com/user-attachments/assets/b40fcd27-cb14-4f93-b205-94dbcff4a5c6" />


## Pada file tersebut kita dapat mendefinisikan route untuk aplikasi yang kita buat.
**Kode tersebut akan mengarahkan rute untuk halaman home.**

## Membuat Route Baru.
**Menambahkan kode berikut di dalam Routes.php**

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/7b2dfd32-5567-4995-a961-431e199ebe57" />


## Untuk mengetahui route yang ditambahkan sudah benar, buka CLI dan jalankan perintah berikut.
**```php spark routes```**

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/a84b58e5-6c1f-4d40-a8eb-18f13306f282" />

## Selanjutnya coba akses route yang telah dibuat dengan mengakses alamat url
**http://localhost:8080/about**

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 141418" src="https://github.com/user-attachments/assets/b5cccc21-33e9-4957-baf2-5109aedd815a" />

## Membuat Controller
Selanjutnya adalah membuat Controller Page. 

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/c2175608-d738-4899-a35d-617716c2ec9c" />

Selanjutnya refresh Kembali browser, maka akan ditampilkan hasilnya yaitu halaman sudah
dapat diakses.

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 142106" src="https://github.com/user-attachments/assets/d61e53e2-e263-4be0-9ab9-d20af0dbeb20" />

## Auto Routing
Secara default fitur autoroute pada Codeiginiter sudah aktif. Untuk mengubah status autoroute
dapat mengubah nilai variabelnya. Untuk menonaktifkan ubah nilai true menjadi false.


<img width="800" height="400" alt="Cuplikan layar 2026-03-30 143154" src="https://github.com/user-attachments/assets/67229d18-2f32-472b-a51e-4529ca374736" />

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 143923" src="https://github.com/user-attachments/assets/99416ef6-381d-4236-8bd7-dc0b07c64799" />

<img width="800" height="400" alt="Cuplikan layar 2026-03-30 144008" src="https://github.com/user-attachments/assets/d074821a-13eb-42ed-b64d-e91b50007a6a" />

<img width="800" height="600" alt="Cuplikan layar 2026-03-30 145721" src="https://github.com/user-attachments/assets/8e9c236c-8f6f-4cb3-95e8-7330961bfa54" />
