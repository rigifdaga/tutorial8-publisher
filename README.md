1. How many data your publisher program will send to the message broker in one run?
   Program publisher akan mengirimkan lima set informasi ke dalam sistem pengirim pesan pada satu waktu.
   Penyebabnya adalah karena ada lima kali pemanggilan fungsi bernama publish_event. Setiap kali fungsi dipanggil, itu akan mengirim satu pesan yang berisi informasi tentang kejadian pembuatan pengguna atau UserCreatedEventMessage ke dalam sistem pengirim pesan.

2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
   URL amqp://guest:guest@localhost:5672 dipergunakan dalam kedua program subscriber dan publisher. Ini mengindikasikan bahwa kedua subscriber dan publisher terkoneksi ke server AMQP yang identik.
   Koneksi menggunakan informasi akun yang serupa, dengan nama pengguna "guest" dan sandi "guest". Server AMQP aktif di localhost menggunakan port 5672.

3. Running RabbitMQ

   [![Whats-App-Image-2024-04-22-at-11-15-41-ec51e3d6.jpg](https://i.postimg.cc/SsF7M4x9/Whats-App-Image-2024-04-22-at-11-15-41-ec51e3d6.jpg)](https://postimg.cc/Ty0WzZm2)