1. Akses server menggunakan terminal (Windows Terminal/PuTTY/etc.)  
- Untuk bisa mengakses server dari windows terminal kita harus menginstall sshserver terlebih dahulu (sudo apt install openssh-server)
- Lalu cek status apakah ssh sudah aktif (sudo systemctl status ssh)
 <img width="802" height="446" alt="image" src="https://github.com/user-attachments/assets/51636ef5-662a-4390-9e8b-41bdcb65c284" />

- Lalu jalankan ssh di terminal (ssh username@ip address) 
 <img width="802" height="616" alt="image" src="https://github.com/user-attachments/assets/b3b72d14-2545-4074-a483-f4a7eb9a3d32" />

2. Konfigurasi ssh kalian agar bisa di akses *hanya menggunakan publickey* (password opsional, bisa dimatikan)
- Kita juga bisa mengakses menggunakan publickey dengan cara membuat public key terlebih dahulu (ssh-keygen)
- lalu key akan di simpan di direktori ssh , kita juga bisa mengubah nama key ( disini saya ubah dengan kunciguweh)
 <img width="940" height="722" alt="image" src="https://github.com/user-attachments/assets/1a94c582-71c6-4e16-92bf-e2f07bf7534d" />

- Kita bisa copy isi dari file kunciguweh.pub 
- lalu kita akses authorized_key pada direktori ssh, dan paste key yang ada didalam file kunciguweh
 <img width="940" height="134" alt="image" src="https://github.com/user-attachments/assets/adb4d671-4a9e-4fac-bbe5-22abbf00643c" />

 <img width="940" height="168" alt="image" src="https://github.com/user-attachments/assets/a79dce46-8fc6-4ab3-988f-5c26c73fb295" />
 
- lalu kita bisa mengakses server dari terminal menggunakan public key dengan cara ssh -i .ssh/nama file key username@ip
 <img width="940" height="722" alt="image" src="https://github.com/user-attachments/assets/187a3ad3-35c8-48aa-99e1-2ad01c234e3a" />

3. Buat step by step penggunaan text manipulation! (grep, sed, cat, echo)
a. cat = membaca isi file 
- cat bisa membuat file baru dengan cara ( cat > nama file) lalu ketik masukan text
- cat bisa menggabungkan 2 file kedalam file baru ( cat file1 file2 > file3)
- cat bisa menambah isi file dengan cara ( cat file1 >> file3), pada baris terakhir didalam file 3 akan menambahkan isi file1
 <img width="940" height="151" alt="image" src="https://github.com/user-attachments/assets/fb41b471-0e2f-42e6-955e-729a717bdbec" />

 <img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/cdc592a6-3c34-4026-91f1-4942894441f4" />

b. sed = stream editor, bisa mengubah, menghapus text didalam file output
- mengubah kata hello menjadi hai di dalam file1 (sed -i ‘s/hello/hai/g’  file1), -i berguna untuk mengubah file asli, tanpa ada -i hanya yang berubah namun file asli tidak berubah
 <img width="940" height="154" alt="image" src="https://github.com/user-attachments/assets/e255d18b-d1ce-4702-9a77-3d748788d1f4" />

- menghapus baris ke-2 pada file3 (sed -i ‘2s’ file3) 
 <img width="940" height="216" alt="image" src="https://github.com/user-attachments/assets/1343b512-9ae0-4831-9ccc-642cf569633e" />

c. grep = Global Regular Expression Print
- mencari kata didalam file (grep hai file1)
- menghitung kata didalam file (grep -c hai file1)
- mencari kata didalam direktori menggunaan  ‘*’ ( grep hello *)
- menghitung kata didalam direktori menggunakan ‘*’ (grep -c hello *)
 <img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/e6ea6376-bcaf-49fe-8009-f6aa2a5762ea" />

 
d. sort = mengurutkan kata atau angka 
- urut secara asc dengan (sort nama file)
- urut secara des dengan (sort -r nama file)
 <img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/ab8fb5a1-fff7-46e5-882f-63754b9af55f" />

4. Nyalakan ufw dengan memberikan akses untuk port 22, 80, 443, 3000, 5000 dan 6969! 
- ufw = Uncomplicated Firewall 
- untuk mengizinkan/memblokir port 
- menginzinkan sebuah port ( sudo ufw allow port)
 <img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/52a019ed-4d4d-48d1-b092-a130b3b4fd32" />

- memblokir  sebuah port (sudo ufw deny port)  
 <img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/377233bc-eb26-4ec7-9393-264845e0b1af" />
