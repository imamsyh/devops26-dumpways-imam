1. Buat sebuah diagram sebuah jaringan komputer dengan 4 device dengan kondisi : 
- IP Class C : 192.168.4.xxx 
- CIDR Block : 192.168.11.0/24 
 <img width="464" height="374" alt="image" src="https://github.com/user-attachments/assets/b3b7e832-128b-4fc8-92cd-50e95de9b834" />

2. Jelaskan perbedaan antara SH (Shell) dan BASH (Bourne-Again Shell)
Jawab :
Shell merupakan bahasa yang umum digunakan pada OS UNIX/Linux sedangkan BASH adalah jenis pengembangan dari shell itu sendiri yang mana lebih lengkap dan modern dan sering dijadikan default
Perbedaan :
	Shell	BASH
Fitur	Sederhana	Lebih lengkap dan modern
Script 	Terbatas	Sangat mendukung 
Digunakan	Unix Lama	Linux modern (sering dijadikan default)

 
3. Buat dokumentasi/kumpulan command linux yang kalian ketahui! (Command diluar materi akan diberi nilai ++)
- sudo apt update = update repo sebagai admin
 <img width="590" height="146" alt="image" src="https://github.com/user-attachments/assets/2edb1f0d-5f3c-46dc-876f-717fd2d39521" />
 
- sudo apt list –upgradable = untuk melihat list repo yang bisa di upgarde
 <img width="590" height="444" alt="image" src="https://github.com/user-attachments/assets/04a99c15-56d5-4da8-aead-17bd6a10f08e" />
 
- mkdir  “nama folder” =  membuat folder
- ls = melihat isi direktori
- touch “nama file” = membuat file kosong
- ls -la = melihat isi direktori secara detail beserta file hidden
- cd  “nama direktori”/ = pindah ke direktori
- cd .. = kembali direktori sebelumnya  
<img width="590" height="341" alt="image" src="https://github.com/user-attachments/assets/25e6a71a-2d83-4de3-b9e2-c880f35afb50" />

- cp “nama file yang ada” “nama file baru” = copy file 
- mv  “nama file” “tujuan” = pindah file 
 <img width="587" height="171" alt="image" src="https://github.com/user-attachments/assets/ad98be5c-0f9b-458a-bfca-9d55be9268d5" />
 
-echo “text” = menampilkan text
-echo “text” > “nama file” = membuat text dan menyimpan di file baru (jika belum ada file)
- cat “nama file” = menampilkan isi file
- echo “text” >> “nama file” = menambah text di akhir baris file
- echo “text baru” > “nama file yang sudah ada” = mengganti text dengan yang baru 
 <img width="587" height="185" alt="image" src="https://github.com/user-attachments/assets/54576d59-2dc7-4af5-9fd8-a9607df1066f" />
 
- find = mencari file
- find -type f = mencari semua file biasa
-find -type d = mencari seluruh direktori
 <img width="587" height="399" alt="image" src="https://github.com/user-attachments/assets/ee7618b9-8ecc-44e1-bc66-2178ef015f78" />
 
-find -type f -name “nama file” = mencari file biasa (jika ada akan menampilkan lokasi file jika tidak ada maka tidak menampilkan apapun”
 <img width="587" height="101" alt="image" src="https://github.com/user-attachments/assets/7027450e-56a3-4650-b2cb-3091a084eed6" />
 
- grep “text” “nama file” = mencari text di dalam file (jika tidak ada maka tidak akan menampilkan apapun)
 <img width="585" height="89" alt="image" src="https://github.com/user-attachments/assets/6cf5afe8-adf8-4b39-a26c-4c88c929b6ff" />
 
- nano “nama file” = menampilkan gui file sederhana  (bisa edit, tambah, hapus dll)
 <img width="585" height="446" alt="image" src="https://github.com/user-attachments/assets/c5da6d0f-7e0f-4e05-badb-600a9d0ca2ed" />
 
-chmod 777 file.js = mengubah hak akses kepada semua  user
- chmod 773 file.js = mengubah hak akses, hanya bisa tulis dan eksekusi untuk selain yang mempunyai file
 <img width="591" height="443" alt="image" src="https://github.com/user-attachments/assets/f76a459d-3e62-4fb3-90c8-a4eb28829536" />
 
-sudo chown root:root file.js = mengubah kepemilikan file
 <img width="588" height="255" alt="image" src="https://github.com/user-attachments/assets/84767380-d3b5-4cb0-b001-1ba9ca5cf4a6" />

-history = melihat histori komen
-sudo su = berpindah ke user root
-exit = keluar dari user root
 <img width="588" height="441" alt="image" src="https://github.com/user-attachments/assets/deba898e-2c18-41cb-9535-46d2566188df" />


