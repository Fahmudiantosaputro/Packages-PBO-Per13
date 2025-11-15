## 1.	Pendahuluan
   
Pada aplikasi berbasis desktop, fitur autentikasi merupakan bagian penting untuk menjaga keamanan akses pengguna. Implementasi Form Login dalam Java NetBeans biasanya melibatkan beberapa komponen seperti penyimpanan data akun (database), form antarmuka (Java Swing), serta logika validasi username dan password.
Dalam proyek ini, dibuat sebuah sistem autentikasi yang terdiri dari beberapa fitur utama: Login, Daftar Akun, Input Password, Lupa Sandi, dan Konfirmasi Sandi Baru. Seluruh proses dirancang menggunakan Java Swing pada NetBeans, serta menggunakan database sebagai penyimpanan data permanen.

## 2.	Tujuan
   
•	Membuat form login interaktif menggunakan Java Swing.
•	Menerapkan proses autentikasi dasar: login, daftar akun, dan manajemen kata sandi.
•	Mengimplementasikan validasi password yang aman (panjang minimal, kombinasi karakter).
•	Mengembangkan fitur Lupa Sandi yang melibatkan verifikasi data pengguna.
•	Menyimpan data pengguna menggunakan database sehingga proses autentikasi bersifat permanen.
•	Melatih integrasi antara logika OOP, GUI, dan database dalam satu sistem.
•	Menggunakan JOptionPane, JTextField, dan JPasswordField untuk menangani input pengguna.

## 3.	Tugas
Proyek ini dibuat untuk memenuhi tugas mata kuliah Pemrograman Berbasis Objek (Java), dengan fokus pada pembuatan sistem autentikasi sederhana. Aplikasi mencakup:
Komponen Utama:
1.	Form Login
Menyediakan input Username dan Password serta tombol Login, Daftar, Reset Pass, Ubah Pass dan Dassboart/Beranda.

3.	Form Registrasi (Daftar Akun)
Menambahkan pengguna baru ke database dengan input:
a)	Username
b)	Password
c)	Konfirmasi Password
4.	Form Lupa Sandi
Verifikasi pengguna berdasarkan email/username untuk reset password.

6.	Form Reset Password
Memasukkan password baru dan melakukan konfirmasi password sebelum disimpan.

7.	Koneksi Database
Menggunakan JDBC/JPA untuk menyimpan dan membaca data akun secara permanen.
Seluruh komponen ini dihubungkan dalam satu aplikasi autentikasi dasar menggunakan Java Swing.

## IMPLEMENTASI FORM LOGIN DENGAN FITUR AUTENTIKASI BERBASIS JAVA NETBEANS (SWING)

1.	Langkah pertama membuat database tujuan nya untuk menyimpan data dan mengkoneksikan ke project Login yang kita buat.

<img width="817" height="251" alt="image" src="https://github.com/user-attachments/assets/5b8d3a87-4d23-44eb-8cb3-3bb5d6316b6a" />
 
2.	Langkah  kedua membuat source packages baru di NeatBeasn, Misalnya PertemuanKetigabelas.java. Selanjutnya membuat class
3.	dengan categori java with ANT dan pilih project Application bertujuan untuk menampung class Login dan lain lain. Kemudian
4.	tambahkan liberies yang harus diterapkan, membbuat entity database presistence.

a.	

<img width="832" height="570" alt="image" src="https://github.com/user-attachments/assets/8928a1b6-4736-40c3-822a-5cd8dfbb4af6" />

b.	

<img width="372" height="305" alt="image" src="https://github.com/user-attachments/assets/9bdbd3c3-c74c-4477-8b0c-d8713e949ab2" />
<img width="435" height="307" alt="image" src="https://github.com/user-attachments/assets/6e00fba3-30bb-47d3-b606-92625a9cfc0b" />

Pilih NEW, Lalu Entity class from DB, serta koneksikan database ke DB yang sudah dibuat diPgAdmin teman-teman. Kemudian tinggal next, 
next terakhir finish.

3.	Langkah ketiga membuat JFrame From untuk class login, reset pass, ubah pass, lalu daftar serta beranda.

<img width="368" height="303" alt="image" src="https://github.com/user-attachments/assets/16286060-0bbc-4099-be41-d6b9139100bb" />
<img width="441" height="302" alt="image" src="https://github.com/user-attachments/assets/cec135aa-09d9-4026-94e5-aaca8c28ca4f" />

4.	Langkah keempat, membuat desain GUI sesuai class yang ada. Jadi desain GUI dibawah itu menggunakan PALLET : PANEL, LABEL, TEXT FIELD,
5.	PASSWORD FIELD, DAN BOTTOM.

<img width="378" height="340" alt="image" src="https://github.com/user-attachments/assets/25804a58-ddca-4409-9b3a-0aabb1ac223a" />
<img width="408" height="339" alt="image" src="https://github.com/user-attachments/assets/b7d561dd-7517-407c-904e-8465a85d5059" />
<img width="382" height="319" alt="image" src="https://github.com/user-attachments/assets/cbfb17c0-64ff-46bc-9c8f-6c2076162135" />
<img width="404" height="317" alt="image" src="https://github.com/user-attachments/assets/4315a0f0-efb0-432a-9381-52304ca68b4a" />


6.	Langkah kelima, membuat logika dengan melengkapi code di sourcenya :
Code class FromLogin.java 
 
<img width="772" height="697" alt="image" src="https://github.com/user-attachments/assets/0f2948ed-8a00-4685-b964-74343d51e161" />

Code class FromDaftar.java
 
<img width="799" height="504" alt="image" src="https://github.com/user-attachments/assets/e62846ca-65d0-4093-b669-ebc71ecc6c09" />
<img width="748" height="246" alt="image" src="https://github.com/user-attachments/assets/4aca3724-7ec3-4b0d-a413-d30c9c938651" />

Code FromResetSandi.java
 
<img width="673" height="631" alt="image" src="https://github.com/user-attachments/assets/67777821-4ecb-41db-a35d-7d9f0c83784d" />

Code FromLupaSandi.java

 <img width="684" height="656" alt="image" src="https://github.com/user-attachments/assets/181635e0-9ef5-47fa-bc55-7818a95c4ca2" />

6.	Langkah keenam, mencoba project/Output project.

<img width="385" height="390" alt="image" src="https://github.com/user-attachments/assets/1015a847-eab7-4b9b-a24c-633ab99a0a70" />
<img width="385" height="390" alt="image" src="https://github.com/user-attachments/assets/a5c18393-96e5-4b31-8c9d-671484970b05" />

-	Melakukan pengisian username dan password untuk login, apabila username dan password belum terdaftar maka akan ada peringatan user
-	dan pass salah, dan sebaliknya ketika sudah terdaftar makan akan otomatis status login berhasil dan dialihkan ke beranda atau halaman selanjutnya.

<img width="381" height="362" alt="image" src="https://github.com/user-attachments/assets/ba906a16-c59e-4913-aa8d-92e6f4a27bc0" />
<img width="382" height="362" alt="image" src="https://github.com/user-attachments/assets/7571651e-d010-4190-92d3-5333102ed395" />

-	Ketika username dan password masih belum bisa, maka user diminta untuk mendaftar akun terlebih dahulu untuk melakukan proses login.

<img width="390" height="301" alt="image" src="https://github.com/user-attachments/assets/4baa12be-b784-47ef-a2e9-6c352e108c53" />
<img width="375" height="300" alt="image" src="https://github.com/user-attachments/assets/40cfce4e-341d-4656-a3ef-71ed3fb5ccf0" />

-	Ketika terjadi yang tidak kita inginkan yaitu lupa sandi dan hanya ingat username, maka kita ke halaman lupa sandi dengan di suruh
-	untuk menginput username dan merubah sandi.

<img width="381" height="360" alt="image" src="https://github.com/user-attachments/assets/bb04cf71-f75a-4f65-8769-4000f8521266" />
<img width="381" height="360" alt="image" src="https://github.com/user-attachments/assets/b7c65ecd-9a59-43cf-926e-9aa3eee3d1fb" />

-	Lalu, user diminta untuk menginput kembali password dan diminta untuk merubah kata sandi yang sebelumnya lupa kata sandi, Kemudian
-	user bisa menginput kembali ke halaman login dengan username tetap dan kata sandi baru.

<img width="380" height="382" alt="image" src="https://github.com/user-attachments/assets/f1a4f31b-517a-498f-8600-8c14276b4f6a" />
<img width="376" height="380" alt="image" src="https://github.com/user-attachments/assets/9da364a9-4e36-47d6-8458-9b63b452795a" />

-	Kemudian, user diminta untuk menginput kembali username dan password yang sudah diganti untuk melakukan login. Maka, login berhasil
-	dan di tuntun ke halaman berikutnya.

 <img width="447" height="367" alt="image" src="https://github.com/user-attachments/assets/0f4f2ffd-b07b-4364-99e8-4eb321c099f3" />

-	Ini adalah halaman beranda yang setelah melakukan keberhasilan login.

*Notes
Untuk penginputan semua kolom tidak boleh kosong wajib di isi ketika tidak di isi maka ada peringatan “username atau password tidak boleh kosong” dan itu karena adanya keyword IF di bottom setiap submit.
