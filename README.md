Apa itu Git?

•	Git adalah salah satu sistem pengontrol versi (Version Control System) pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds.

•	Pengontrol versi bertugas mencatat setiap perubahan pada file proyek yang dikerjakan oleh banyak orang maupun sendiri.

•	Git dikenal juga dengan distributed revision control (VCS terdistribusi), artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja.

Membuat Reposiory Local

•	Buka direktory aktif, misal: d:\labs_pemrograman1 (buka menggunakan Windows Explorer)

•	klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash commad

•	Buat direktory project praktikum pertama dengan nama latihan1

•	Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya •	masuk kedalam direktori tersebut dengan perintah cd (change directory)

•	direktory aktif menjadi: d:\labs_pemrograman1\latihan6
![latihan 8](https://user-images.githubusercontent.com/46995335/51738351-927db680-20c1-11e9-9c89-c28154a328d1.png)
Membuat Reposiory Local

•	Jalankan perintah git init, untuk membuat repository local.

•	Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git

•	Pada direktori tersebut, semua perubahan pada working directory akan disimpan. 
![untitled 2](https://user-images.githubusercontent.com/46995335/51738527-f6a07a80-20c1-11e9-9a85-5d3be76e71e9.png)
Menambahkan File baru pada repository

•	Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)

•	disini kita akan coba buat satu file bernama README.md (text file)

$ echo “#Latihan 1” >> README.md

•	File README.md berhasil dibuat.
![latihan 1](https://user-images.githubusercontent.com/46995335/51738679-467f4180-20c2-11e9-83d9-96d0245102e5.png)
Menambahkan File baru pada repository

•	Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.

$ git add README.md

•	File README.md berhasil ditambahkan.
![latihan 3](https://user-images.githubusercontent.com/46995335/51738954-e8069300-20c2-11e9-9b83-e8fefa1a0b9e.png)
Commit (Menyimpan perubahan ke database)

•	Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit”

$ git commit -m “File pertama saya”

•	Perubahan berhasil disimpan
![untitled 3](https://user-images.githubusercontent.com/46995335/51739141-54819200-20c3-11e9-8530-849a7918b02c.png)
Membuat repository server

•	Isi nama repositorynya, misal: latihan001.

•	lalu klik tombol Create repository
![untitled 5](https://user-images.githubusercontent.com/46995335/51739217-82ff6d00-20c3-11e9-8683-31195a92cbd1.png)
Menambahkan Remote Repository

•	Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

•	Untuk menambahkan remote repository server, gunakan perintah Menambahkan Remote Repository

•	Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

•	Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url] 
![untitled 8](https://user-images.githubusercontent.com/46995335/51739335-cd80e980-20c3-11e9-84f7-7ca78b967551.png)
•	Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.

$ git push -u origin master

•	Perintah ini akan meminta memasukkan username dan password pada akun github.com 
![latihan 10](https://user-images.githubusercontent.com/46995335/51739485-1f297400-20c4-11e9-830f-fb5c73207cf9.png)
Melihat hasilnya pada server repository
Buka laman github.com, arahkan pada repositorynya , maka perubahan akan terlihat pada laman tersebut.
![latihan 11](https://user-images.githubusercontent.com/46995335/51739587-70d1fe80-20c4-11e9-9785-8aa33772b7f7.png)
Clone Repository

•	Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory).

•	Untuk melakukan cloning, gunakan perintah git clone [url]

![latihan 31](https://user-images.githubusercontent.com/46995335/51739715-bc84a800-20c4-11e9-8b76-1797a2a5f768.png)
