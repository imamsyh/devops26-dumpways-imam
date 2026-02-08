Challenge Load Balancing:
1. Terapkan Load Balancing untuk wayshub-frontend menggunakan 2 server dengan spek yang sama
2. Gunakan 2 dari 3 pilihan method ini :
  - Round Robin
  - IP Hash
  - Least Connections
-------------------------------------------------------------------------------------------
1. Terapkan Load Balancing untuk wayshub-frontend menggunakan 2 server dengan spek yang sama
a. Round Robin

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

-jalankan nohup agar bisa test dan jalankan di web dengan mengetik domain yang sudah di set
<img width="1920" height="1030" alt="Screenshot 2026-02-08 202252" src="https://github.com/user-attachments/assets/3bc2a3ae-39e4-4f63-ad16-82a9605b40ee" />


