# Aplikasi Buku Tour Rohani 📖✝️  

Buku Tour Rohani adalah aplikasi Android yang dirancang untuk mempermudah peserta dalam mengakses informasi, berkomunikasi, dan menjalankan aktivitas selama perjalanan atau acara rohani. Aplikasi ini bertindak sebagai pendamping digital yang membantu peserta agar tetap terorganisir dan mendapatkan pengalaman yang lebih terstruktur selama tour berlangsung.  

---

## Pengertian  
Aplikasi Buku Tour Rohani adalah solusi modern yang mengintegrasikan informasi jadwal acara, daftar tempat yang akan dikunjungi, lagu/pujian, serta fitur komunikasi dan notifikasi dalam satu platform digital. Selain itu, aplikasi ini juga menyediakan fitur darurat (SOS) yang memberikan rasa aman kepada peserta dengan memungkinkan mereka menghubungi panitia saat menghadapi situasi genting.  

---

## Latar Belakang  
Dalam sebuah acara tour rohani, peserta sering kali dihadapkan pada berbagai kendala, seperti kesulitan mengakses informasi jadwal acara, kurangnya deskripsi tentang tempat yang akan dikunjungi, atau keterbatasan komunikasi dengan peserta dan panitia. Kondisi ini dapat mengurangi kenyamanan peserta dan menyulitkan panitia dalam mengelola acara.  

Untuk mengatasi tantangan ini, Buku Tour Rohani hadir sebagai solusi inovatif. Dengan memanfaatkan teknologi Firebase dan integrasi berbagai fitur digital, aplikasi ini tidak hanya mempermudah peserta, tetapi juga mendukung admin atau panitia dalam menyampaikan informasi secara efektif.  

---

## Tujuan  
1. **Menyediakan akses informasi yang terpusat:** Memastikan peserta memiliki semua informasi penting yang dibutuhkan selama tour.  
2. **Meningkatkan komunikasi:** Memfasilitasi interaksi antara peserta melalui forum chat dan notifikasi.  
3. **Mendukung pengelolaan acara:** Memberikan kemudahan bagi admin dalam mengelola data peserta, konten acara, dan penyampaian informasi.  
4. **Menjamin rasa aman:** Menyediakan fitur SOS untuk memberikan solusi cepat dalam situasi darurat.  

---

## Fitur Aplikasi  

### **Fitur Sisi User:**  
1. **Login:**  
   - Peserta dapat login menggunakan email dan password melalui Firebase Authentication.  

2. **Menu Home:**  
   - Menampilkan informasi utama aplikasi, dengan tiga ikon utama:  
     - **Buku Tour:**  
       - Menyediakan rundown acara yang rinci berdasarkan hari.  
       - Menampilkan deskripsi tempat yang akan dikunjungi serta aktivitas terkait.  
       - Menyediakan daftar lagu/pujian lengkap dengan lirik dan informasi penulis.  
     - **Friend List:**  
       - Menampilkan daftar peserta tour. Peserta dapat melihat nama-nama peserta lainnya.  
     - **SOS:**  
       - Tombol darurat untuk menghubungi panitia melalui panggilan telepon langsung. Nomor panitia telah ditentukan sebelumnya dan siap digunakan saat peserta menghadapi situasi mendesak.  

3. **Forum Chat (Pesan):**  
   - Peserta dapat berkomunikasi dan berdiskusi melalui fitur forum chat. Data percakapan disimpan dalam Firebase Realtime Database.  

4. **Menu Notification:**  
   - Menampilkan pemberitahuan dari admin terkait jadwal, pengumuman, atau informasi penting lainnya. Push notification dilakukan menggunakan Firebase Cloud Messaging.  

5. **Menu Profile:**  
   - Peserta dapat melihat dan mengedit profil mereka, termasuk nama lengkap, email, nomor telepon, alamat, dan lainnya. Semua data tersimpan dengan aman di Firebase Realtime Database.  

---

### **Fitur Sisi Admin:**  
1. **Manage User:**  
   - Admin memiliki kemampuan untuk menambahkan, mengedit, melihat, dan menghapus data peserta.  

2. **Manage Content:**  
   - Admin dapat mengelola konten acara, seperti rundown, deskripsi aktivitas, dan daftar lagu. Konten ini akan terlihat oleh peserta di aplikasi.  

3. **Manage Broadcast:**  
   - Admin dapat mengirimkan notifikasi broadcast ke peserta untuk memberikan informasi terkini.  

---

## Teknologi yang Digunakan  
1. **Firebase Authentication:** Untuk proses autentikasi login peserta.  
2. **Firebase Realtime Database:** Untuk menyimpan data rundown, aktivitas, lagu, percakapan chat, dan notifikasi.  
3. **Firebase Cloud Messaging:** Untuk push notification dari admin ke peserta.  
4. **Android Native:** Untuk membangun fitur tombol darurat (SOS) yang menghubungkan langsung ke nomor telepon panitia.  

---

## Cara Implementasi/Instalasi  

### **Prasyarat:**  
- Android Studio (versi terbaru)  
- Akun Firebase untuk mengintegrasikan project  
- Emulator Android atau perangkat fisik untuk pengujian  

### **Langkah Instalasi:**  
1. **Clone Repository:**  
   - Unduh source code dari repository GitHub ini dengan perintah berikut:  
     ```bash  
     git clone https://github.com/andrsginting/Religion-Tour-App.git  
     cd buku-tour-rohani  
     ```  

2. **Import Project ke Android Studio:**  
   - Buka Android Studio.  
   - Pilih **Open an Existing Project** dan arahkan ke folder yang telah di-clone.  

3. **Konfigurasi Firebase:**  
   - Buat project baru di [Firebase Console](https://firebase.google.com/).  
   - Unduh file `google-services.json` dari Firebase Console dan letakkan di dalam folder `app/` pada project.  
   - Aktifkan fitur Firebase berikut:  
     - **Authentication**  
     - **Realtime Database**  
     - **Cloud Messaging**  

4. **Sinkronisasi Gradle:**  
   - Pastikan semua dependencies ter-update. Lakukan sinkronisasi Gradle di Android Studio.  

5. **Build dan Jalankan Aplikasi:**  
   - Sambungkan emulator atau perangkat fisik ke Android Studio.  
   - Klik tombol **Run** untuk menguji aplikasi.  

6. **Pengujian:**  
   - Gunakan email dan password untuk login.  
   - Coba semua fitur seperti Buku Tour, Friend List, SOS, dan Forum Chat untuk memastikan aplikasi berjalan sesuai fungsi.  

---
