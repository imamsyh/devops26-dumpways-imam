Challenge Load Balancing:
1. Terapkan Load Balancing untuk wayshub-frontend menggunakan 2 server dengan spek yang sama
2. Gunakan 2 dari 3 pilihan method ini :
  - Round Robin
  - IP Hash
  - Least Connections
-------------------------------------------------------------------------------------------
1. Terapkan Load Balancing untuk wayshub-frontend menggunakan 2 server dengan spek yang sama
-Round Robin

step:
- buat server untuk set lb
<img width="973" height="615" alt="Screenshot 2026-02-08 202701" src="https://github.com/user-attachments/assets/6ec6d8fd-ff4f-447d-8d71-273b64168327" />

- install ssh dan nginx di server lb
- copy direktori app ke server lb karena server tersebut akan di jadikan server ke 2 sekaligus (scp -r wayshub-frontend imam@I192.168.100.210:/home/imam/)
<img width="1115" height="628" alt="Screenshot 2026-02-08 143127" src="https://github.com/user-attachments/assets/5cc26c21-4799-4e84-8bbf-eb7c17bc72ab" />

-buat file configurasi untuk lb round robin di dir nginx/sites-available
<img width="960" height="1032" alt="Screenshot 2026-02-08 203447" src="https://github.com/user-attachments/assets/fb2201eb-3722-4ea3-9f5e-317c1d7fd4f2" />

- karena file konfigurasi tadi ada di sites-available, maka harus di singkronkan ke sites-enable denham symlink (sudo ln -s /etc/nginx/sites-available/wayshub-lb-rr /etc/nginx/sites-enabled/)
<img width="1115" height="142" alt="Screenshot 2026-02-08 201235" src="https://github.com/user-attachments/assets/4417132a-d4e8-48e3-9425-86e2ad3edacf" />

-jalankan nohup agar bisa test dengan curl domain dan jalankan di web dengan mengetik domain yang sudah di set
<img width="1920" height="1030" alt="Screenshot 2026-02-08 202252" src="https://github.com/user-attachments/assets/3bc2a3ae-39e4-4f63-ad16-82a9605b40ee" />

- Ip Hash

step: 
- karena disini saya hanya merubah set pada konfigurasi file, maka untuk step dari installasi sama dengan rr
- lalu pada file konfigurasi yang membedakan set rr dan ip hash hanya pada upstream yaitu dengan menambahkan iphash;
<img width="960" height="1032" alt="Screenshot 2026-02-08 212841" src="https://github.com/user-attachments/assets/72eabea0-8c0e-4a78-827c-c065f1db0f2a" />

-karena disini saya melakukan perubahan nama, maka saya melakukan symlink kembali
- lalu cek nginx dan reload nginx
<img width="960" height="1032" alt="Screenshot 2026-02-08 212841" src="https://github.com/user-attachments/assets/6f36a8ef-3060-4d01-bfa0-3f179048db08" />

- lalu jalankan nohup agar di cek dengan curl dan buka domain di web
<img width="1920" height="1080" alt="Screenshot 2026-02-08 212122" src="https://github.com/user-attachments/assets/673a3cbd-2f93-4f01-a864-0046c14c125f" />




