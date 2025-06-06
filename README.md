<div align="center">
  <img src="./Header.png" alt="Simple_Insightface Banner" width="700">
</div>

<p align="center">
  Kumpulan notebook Google Colab untuk eksperimen <i>face swapping</i> yang mudah digunakan dengan pustaka InsightFace.
</p>

---

## 🚀 Pendahuluan

Selamat datang di repositori **Simple_Insightface**! 

Repositori ini bertujuan untuk menyediakan alat _face swapping_ (pertukaran wajah) yang siap pakai dan mudah diakses melalui Google Colab. Keunggulan utama adalah pengguna tidak perlu lagi direpotkan dengan pengunduhan file model secara manual; notebook akan menanganinya secara otomatis. Cukup siapkan gambar sumber dan target Anda, lalu biarkan keajaiban terjadi!

Saat ini, Anda akan menemukan dua notebook utama yang siap dieksplorasi:
1.  🖼️ **Face Swap Gambar-ke-Gambar**: Menukar wajah antara dua gambar.
2.  🎬 **Face Swap Gambar-ke-Video (File)**: Mengaplikasikan wajah dari gambar sumber ke setiap frame dalam sebuah file video.

## 🌟 Fitur Utama

* **🚀 Siap Digunakan di Google Colab**: Dirancang khusus untuk berjalan mulus di lingkungan Google Colab.
* **⚙️ Unduhan Model Otomatis**: Model-model penting (termasuk `inswapper_128.onnx` dari Hugging Face) akan diunduh secara otomatis oleh notebook.
* **🖼️➡️🖼️ Dukungan Gambar-ke-Gambar**: Lakukan pertukaran wajah antara dua gambar statis dengan mudah.
* **🖼️➡️🎬 Dukungan Gambar-ke-Video (File)**: Aplikasikan wajah dari gambar ke seluruh frame dalam file video yang Anda unggah.
* **🧠 Ditenagai InsightFace**: Memanfaatkan kehebatan pustaka `InsightFace` untuk analisis dan pertukaran wajah berkualitas.
* **⚡ Prioritas GPU**: Kode secara otomatis mencoba memanfaatkan GPU di Colab untuk akselerasi pemrosesan.

---

## 📖 Notebook yang Tersedia

### 1. `FaceSwap_Image_to_Image.ipynb`
   * **Deskripsi**: Notebook ini memungkinkan Anda untuk mengambil wajah dari "gambar sumber" dan menempelkannya ke wajah yang terdeteksi pada "gambar target".
   * **Cara Menggunakan**:
        1. Buka file `FaceSwap_Image_to_Image.ipynb` di Google Colab.
        2. Jalankan sel-sel kode secara berurutan dari atas ke bawah.
        3. **PENTING**: Setelah menjalankan sel instalasi library (`!pip install ...`), **restart runtime Colab** melalui menu `Runtime` > `Restart runtime`.
        4. Unggah gambar sumber Anda (yang berisi wajah asli) saat diminta oleh notebook.
        5. Selanjutnya, unggah gambar target Anda (gambar di mana wajah akan diganti).
        6. Hasil pertukaran wajah akan ditampilkan langsung di dalam output notebook.

### 2. `FaceSwap_Image_to_Video_File.ipynb`
   * **Deskripsi**: Dengan notebook ini, Anda dapat mengambil wajah dari "gambar sumber" dan mengaplikasikannya ke wajah yang terdeteksi pada setiap frame dari "file video target" yang Anda unggah. Video hasil akan disimpan dan dapat diunduh.
   * **Cara Menggunakan**:
        1. Buka file `FaceSwap_Image_to_Video_File.ipynb` di Google Colab.
        2. Jalankan sel-sel kode secara berurutan.
        3. **PENTING**: Setelah menjalankan sel instalasi library, jangan lupa untuk **restart runtime Colab**.
        4. Unggah gambar sumber Anda ketika diminta.
        5. Unggah file video target yang ingin Anda proses.
        6. Proses _face swapping_ akan berjalan frame per frame (ini mungkin memakan waktu, tergantung durasi dan resolusi video).
        7. Video hasil (yang tidak menyertakan audio asli) akan disimpan di lingkungan Colab dan siap untuk Anda unduh.

---

## 🛠️ Cara Menggunakan (Instruksi Umum)

1.  **Buka di Google Colab**: Klik pada file `.ipynb` pilihan Anda di repositori ini, lalu pilih opsi "Open in Colab".
2.  **Atur Runtime ke GPU (Sangat Direkomendasikan)**: Untuk performa yang jauh lebih baik, pastikan Anda menggunakan akselerator GPU. Di Google Colab, navigasi ke `Runtime` > `Change runtime type`, lalu pada `Hardware accelerator`, pilih `GPU` dan simpan.
3.  **Jalankan Sel secara Berurutan**: Ikuti alur notebook dengan menjalankan setiap sel kode dari atas ke bawah. Perhatikan instruksi di dalam notebook, terutama saat diminta untuk mengunggah file.
4.  **Restart Runtime Awal**: Selalu ingat untuk me-restart runtime Colab setelah sel yang berisi perintah `!pip install ...` selesai dijalankan. Ini memastikan semua library terinstal dengan benar.

---

## 📜 Pernyataan Penggunaan & Lisensi

Repositori dan notebook di dalamnya merupakan bagian dari eksplorasi dan pembelajaran mandiri saya dalam bidang _computer vision_ dan _deep learning_, khususnya teknologi _face swapping_. Proyek ini dibuat dengan tujuan edukasi dan untuk berbagi pengetahuan.

Semua konten di sini **bebas untuk digunakan, dimodifikasi, dan didistribusikan oleh siapa pun**. Saya senang jika ini bisa bermanfaat bagi rekan-rekan lain yang tertarik untuk belajar atau bereksperimen.

> **Catatan Etika**: Harap gunakan teknologi _face swapping_ secara bertanggung jawab dan etis. Hindari penggunaan yang dapat merugikan, menyesatkan, atau melanggar privasi individu lain.

---

## 🔗 Sumber dan Referensi

Berikut adalah beberapa sumber daya dan pustaka utama yang menjadi dasar atau inspirasi proyek ini:

* **InsightFace (Official GitHub)**: [https://github.com/deepinsight/insightface](https://github.com/deepinsight/insightface)
* **Model `inswapper_128.onnx` (Hugging Face)**: Repositori [ezioruan/inswapper_128.onnx](https://huggingface.co/ezioruan/inswapper_128.onnx/tree/main) (Tautan unduhan langsung yang digunakan: `.../resolve/main/inswapper_128.onnx`)
* **ONNXRuntime**: [https://onnxruntime.ai/](https://onnxruntime.ai/)
* **OpenCV**: [https://opencv.org/](https://opencv.org/)
* **Google Colaboratory**: [https://colab.research.google.com/](https://colab.research.google.com/)

---

<p align="center">
  Saran dan kontribusi untuk pengembangan lebih lanjut sangat diterima! Fork repositori ini dan mari berkreasi bersama.
</p>