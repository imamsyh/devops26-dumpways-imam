Task :
1. Gambarkan sturktur web server menggunakan reverse proxy dan jelaskan cara kerjanya!
2. Buatlah Reverse Proxy untuk aplilkasi yang sudah kalian deploy kemarin. (wayshub), untuk domain nya sesuaikan nama masing" ex: ade.xyz .
-------------------------------------------------------------------------------------------------------------------------------------------

1. Gambarkan sturktur web server menggunakan reverse proxy dan jelaskan cara kerjanya!
<img width="588" height="292" alt="Reverse Proxy" src="https://github.com/user-attachments/assets/e668fec1-f8c2-497b-8f9a-a737f3475b2d" />

Cara Kerja:
- Client mengirim req berupa http/https
- Reverse proxy menerima request dari client, memeriksa aturan dan keamanan, serta menyimpan cache
- Reverse proxy meneruskan request ke server menggunakan alamat ip-nya sendiri(bukan alamat ip client)
- Server memproses request dan mengirim respon kembali ke reverse proxy
- Reverse proxy menerima respon dan meneruskan ke client dengan ip reverse proxy (bukan ip server)


2. Buatlah Reverse Proxy untuk aplilkasi yang sudah kalian deploy kemarin. (wayshub), untuk domain nya sesuaikan nama masing" ex: ade.xyz .
- Pertama kita tambahkan domain secara local terlebih dahulu pada file hosts yang terdapat di /system32/drivers/etc, jalankan file dengan administaror
<img width="1186" height="780" alt="Screenshot 2026-02-07 122717" src="https://github.com/user-attachments/assets/fb531adb-c8b3-4579-a587-b44cfa357aeb" />

- Tambahkan ip address server dan nama domain
<img width="1430" height="748" alt="Screenshot 2026-02-07 131110" src="https://github.com/user-attachments/assets/b08b0c98-e768-423a-a24b-448aab1011fe" />

- Install nginx atau jalankan nginx
<img width="1920" height="1032" alt="Screenshot 2026-02-07 125238" src="https://github.com/user-attachments/assets/c137f3e9-b0e1-43b6-96fb-82ad785c7ebd" />

- Lalu izinkan port 80 dan 443 agar http/https bisa diakses
<img width="1115" height="628" alt="Screenshot 2026-02-07 125326" src="https://github.com/user-attachments/assets/05a55e6e-e47a-4ccf-8edc-ce59515598b8" />

- Masuk ke direktori /etc/nginx/sites-enabled/ dan buat file konfigurasi untuk app 
<img width="960" height="263" alt="Screenshot 2026-02-07 125832" src="https://github.com/user-attachments/assets/2c46f813-16e0-40c7-b444-eec5acd8d744" />

- Set file konfigurasi dengan ip address nama domain yang sudah di set pada file hosts
<img width="960" height="233" alt="Screenshot 2026-02-07 125838" src="https://github.com/user-attachments/assets/b5fce682-ae6b-4eef-95a5-eb159b4c7401" />

- Jalankan domain di web
<img width="1920" height="1080" alt="Screenshot 2026-02-07 131056" src="https://github.com/user-attachments/assets/cfd799a0-a034-4d1d-8e3d-c6e9c6424744" />


