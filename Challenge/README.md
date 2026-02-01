1. Jalankan tugas nomor 3 & 4 di day 3 dalam bentuk script BASH! 
- untuk menjalankan script BASH, kita harus membuat file untuk mejalankan script 
 <img width="940" height="163" alt="image" src="https://github.com/user-attachments/assets/daa962e9-33a4-459f-b061-c04fd2149365" />

- untuk menjalankan file tersebut kita harus mengubah hak akses dengan ( chmod +x nama file)
- +x = mengubah hak akses menjadi file bisa di eksekusi
 <img width="940" height="171" alt="image" src="https://github.com/user-attachments/assets/53e638ff-f1e4-4c84-a173-4507d4edfda6" />

a.  cat = membaca file
- membaca file menggunakan script bash dengan mengetik perintah didalam file lalu eksekusi
 <img width="940" height="150" alt="image" src="https://github.com/user-attachments/assets/add740cf-440a-4460-a675-05f23870f59d" />

 <img width="940" height="103" alt="image" src="https://github.com/user-attachments/assets/03b9fc41-9154-4185-9f1f-c171e5dacc1d" />

- bisa juga membaca beberapa perintah 
 <img width="940" height="157" alt="image" src="https://github.com/user-attachments/assets/2a7211c3-4205-41b8-aa2f-7dcc4ab98906" />

- membaca file, menggabungkan file yang disimpan di file baru (file4)
 <img width="940" height="187" alt="image" src="https://github.com/user-attachments/assets/a2dbde0b-e327-4e9c-aa9a-8c3e4eaba62e" />


b. sed 
- mengubah text didalam file
 <img width="940" height="151" alt="image" src="https://github.com/user-attachments/assets/0f79e201-85e7-45cb-8027-7a3946a434cd" />

 <img width="940" height="95" alt="image" src="https://github.com/user-attachments/assets/8f39f9df-ddb2-45c1-8e67-3c2a0a5605ee" />

c. grep 
- mencari text
 <img width="940" height="166" alt="image" src="https://github.com/user-attachments/assets/85ec2eaf-4229-4b85-ad6e-3e8284fb18ff" />

- mencari text dan menghitung kata didalam direktori
 <img width="940" height="398" alt="image" src="https://github.com/user-attachments/assets/14c6e521-21a9-4cab-aa8e-5f08cd56c820" />

 
d. sort 
- mengurutkan angka atau huruf
 <img width="940" height="188" alt="image" src="https://github.com/user-attachments/assets/a8f86ec4-2aea-4eff-80f1-f8f3619e288f" />

- mengurutkan secara ascending dan descending
 <img width="940" height="396" alt="image" src="https://github.com/user-attachments/assets/fb1b9759-5921-402a-ba06-49564005e130" />

 
e. Nyalakan ufw dengan memberikan akses untuk port 22, 80, 443, 3000, 5000 dan 6969!
- dengan menggunakan script bash bisa mengizinkan/menolak izin port secara langsung menggunakan perintah looping, pertama membuat array port lalu melakukan looping pada array yang akan melakukan sudo ufw deny $port 
- karena sebelumnya telah melakukan pengizinan terhadap port maka pada gambar melakukan penolakan
- jika ingin mengizinkan kembali ubah perintah menjadi sudo ufw allow $port
 <img width="940" height="206" alt="image" src="https://github.com/user-attachments/assets/120b4666-8041-4c8d-9272-220cea9e1107" />

 <img width="940" height="660" alt="image" src="https://github.com/user-attachments/assets/65a17c88-4f91-40a8-af9c-2c915950fea5" />

 
2. Scriptnya bisa menyalakan/menambahkan, dan juga bisa mematikan/menghapus konfigurasinya (No. 1)
-  Pada script bash kita bisa menggunalan perintah if-else, yang mana akan membaca text konfirmasi jika “n” maka akan menjalankan perintah sudo systemctl stop ssh
 <img width="940" height="262" alt="image" src="https://github.com/user-attachments/assets/8a6f2352-0af1-4211-b88e-f1b1ee97b388" />

 <img width="940" height="395" alt="image" src="https://github.com/user-attachments/assets/c6770179-7528-4bb9-aace-20217954ef07" />

- Kita coba di terminal akan keluar connection refused karena ssh inactive (dead)
 <img width="940" height="126" alt="image" src="https://github.com/user-attachments/assets/2027f94c-becb-4726-a390-1750f4a73537" />



-  lalu jika saat membaca text konfirmasi  “y” maka akan menjalankan perintah sudo systemctl start ssh
 <img width="939" height="370" alt="image" src="https://github.com/user-attachments/assets/38870e04-3c85-4e3b-96b2-e9961b8c1aac" />

- Kita coba di terminal akan jalan karena ssh sudah active (running)
 <img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/e5d5a47f-17e7-41e2-8c0f-eea7b0538b79" />


