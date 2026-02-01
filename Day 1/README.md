1.	Secara konsep, jelaskan apa itu DevOps dengan bahasa kalian!
Jawab:
DevOps adalah perantara atau penghubung antara tim development dengan tim operation yang mana akan memperlancar atau mengefesienkan dalam perilisan sebuah update,  perbaikan bug atau aplikasi itu sendiri, selain itu juga dengan adanya DevOps akan memperkecil kegagalan dalam perilisan. 

2.	Install Ubuntu Server 22.04.x LTS menggunakan Virtualbox/VMware/Virtualization Tool pilihan kalian dan buat step-by-step langkah instalasinya!
Jawab:
-	Download dan install Virtualbox, lalu jalankan aplikasi
-	Lalu tekan new VM
-	Input nama  VM, pilih ISO ubuntu yang sudah di download, set ukuran base memory dan CPU, dan set ukuran  harddisk, lalu finish
-	Lalu jalankan VM dengan menekan start
-	Tunggu instalasi ubuntu sampi muncul pilih bahasa, lalu pada type instalaltion pilih ubuntu server, lalu set network configuration seperti point 3
-	Setelah itu custom storage dengan membagi harddisk(total 10GB pada set awal) menjadi 7GB untuk ext4 dan 2.8GB untuk  swap
-	Lalu masukan profile configuration  dengan mengisi nama, nama server, username dan password
-	Selanjutnya kosongkan semua karena kita ingin menginstall VM secara bersih
-	Lalu tunggu installing system
-	Setelah  selesai akan muncul input username dan password, lalu masukan username dan password untuk test ping seperti point 4
3.	Gunakan IP Address xxx.xxx.xxx.208 untuk server VM kalian!
Jawab :
-	Pada network configuration edit IPv4 sesuai dengan  ip yang sedang tersambung dengan perangkat (192.168.100.208), lalu pada name  server gunakan dns 8.8.8.8,  8.8.4.4
4.	Pastikan Ubuntu Server kalian ada jaringan dengan test menggunakan command ping 8.8.8.8 / ping google.com
Jawab :
-	Setelah input username  dan password lalu ketik ping 8.8.8.8 untuk test ping kalau terminal mengembalikan report berarti server sudah berhasil dijalankan

