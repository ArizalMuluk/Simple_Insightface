<div align="center">
  <h1>Simple_Insightface</h1>
</div>

## Pendahuluan

Selamat datang di repositori **Simple_Insightface**! Repositori ini berisi kumpulan notebook Google Colab yang dirancang untuk memudahkan pengguna dalam melakukan eksperimen _face swapping_ (pertukaran wajah) menggunakan pustaka populer `InsightFace`.

Tujuan utama dari proyek ini adalah menyediakan alat yang siap pakai, di mana pengguna tidak perlu repot mengunduh file model secara manual. Cukup siapkan gambar sumber (wajah yang ingin digunakan) dan gambar/video target, lalu jalankan notebooknya.

Saat ini tersedia dua notebook utama:
1.  **Face Swap Gambar-ke-Gambar**: Menukar wajah dari satu gambar ke gambar lainnya.
2.  **Face Swap Gambar-ke-Video (File)**: Menukar wajah dari sebuah gambar ke setiap frame dalam sebuah file video.

## Fitur Utama

* **Siap Digunakan di Google Colab**: Dirancang khusus untuk kemudahan penggunaan di lingkungan Google Colab.
* **Unduhan Model Otomatis**: Notebook secara otomatis akan mengunduh model-model yang diperlukan (termasuk `inswapper_128.onnx` dari Hugging Face) saat pertama kali dijalankan. Anda tidak perlu mengunduh model secara manual.
* **Dukungan untuk Berbagai Skenario**:
    * Pertukaran wajah antara dua gambar statis.
    * Pertukaran wajah dari gambar ke file video.
* **Menggunakan InsightFace**: Ditenagai oleh pustaka `InsightFace` yang canggih untuk analisis dan pertukaran wajah.
* **Prioritas GPU**: Kode akan mencoba menggunakan GPU jika tersedia di lingkungan Colab untuk pemrosesan yang lebih cepat.

## Notebook yang Tersedia

### 1. `FaceSwap_Image_to_Image.ipynb`

* **Deskripsi**: Notebook ini memungkinkan Anda untuk mengambil wajah dari "gambar sumber" dan menempelkannya ke wajah yang terdeteksi pada "gambar target".
* **Cara Menggunakan**:
    1.  Buka file `FaceSwap_Image_to_Image.ipynb` di Google Colab.
    2.  Jalankan sel-sel kode secara berurutan dari atas ke bawah.
    3.  **PENTING**: Setelah menjalankan sel instalasi library pertama, **restart runtime Colab** (`Runtime` > `Restart runtime`).
    4.  Saat diminta, unggah gambar sumber Anda (yang berisi wajah asli).
    5.  Kemudian, unggah gambar target Anda (gambar tempat wajah akan diganti).
    6.  Hasilnya akan ditampilkan di dalam notebook.

### 2. `FaceSwap_Image_to_Video_File.ipynb`

* **Deskripsi**: Notebook ini mengambil wajah dari "gambar sumber" dan menempelkannya ke wajah yang terdeteksi pada setiap frame dari "file video target" yang Anda unggah. Video hasil akan disimpan dan bisa diunduh.
* **Cara Menggunakan**:
    1.  Buka file `FaceSwap_Image_to_Video_File.ipynb` di Google Colab.
    2.  Jalankan sel-sel kode secara berurutan.
    3.  **PENTING**: Setelah menjalankan sel instalasi library pertama, **restart runtime Colab** (`Runtime` > `Restart runtime`).
    4.  Unggah gambar sumber Anda saat diminta.
    5.  Unggah file video target Anda saat diminta.
    6.  Proses akan berjalan frame per frame (mungkin memakan waktu untuk video panjang).
    7.  Video hasil (tanpa audio) akan disimpan di lingkungan Colab dan siap diunduh.

## Cara Menggunakan (Instruksi Umum)

1.  **Buka di Google Colab**: Klik pada file `.ipynb` yang ingin Anda gunakan di repositori ini dan pilih "Open in Colab".
2.  **Atur Runtime (Opsional, tapi Direkomendasikan)**: Untuk performa terbaik, disarankan untuk menggunakan GPU. Di Colab, pilih `Runtime` > `Change runtime type` > `Hardware accelerator` > `GPU`.
3.  **Jalankan Sel**: Jalankan setiap sel kode secara berurutan. Ikuti instruksi yang ada di dalam notebook, terutama untuk mengunggah file.
4.  **Restart Runtime**: Ingat untuk me-restart runtime setelah sel instalasi library awal (`!pip install ...`) selesai dijalankan.

## Pernyataan Penggunaan

Modul-modul dalam repositori ini adalah bagian dari proses pembelajaran mandiri saya dan dikembangkan untuk tujuan edukasi serta eksplorasi teknologi _face swapping_.

Semua kode dan notebook di sini **bebas untuk digunakan, dimodifikasi, dan didistribusikan oleh siapapun**. Saya berharap ini bisa bermanfaat bagi orang lain yang juga sedang belajar atau ingin mencoba teknologi ini.

Meskipun demikian, harap gunakan teknologi ini secara bertanggung jawab dan etis.

## Sumber dan Referensi

Berikut adalah beberapa sumber daya dan pustaka utama yang digunakan atau terkait dengan proyek ini:

* **InsightFace (Official GitHub)**: [https://github.com/deepinsight/insightface](https://github.com/deepinsight/insightface)
* **Model `inswapper_128.onnx` yang digunakan (Hugging Face)**: [https://huggingface.co/ezioruan/inswapper_128.onnx/tree/main](https://huggingface.co/ezioruan/inswapper_128.onnx/tree/main) (Tautan unduhan langsung yang digunakan dalam kode adalah `.../resolve/main/inswapper_128.onnx`)
* **ONNXRuntime**: [https://onnxruntime.ai/](https://onnxruntime.ai/)
* **OpenCV**: [https://opencv.org/](https://opencv.org/)
* **Google Colaboratory**: [https://colab.research.google.com/](https://colab.research.google.com/)

---

Saran dan kontribusi untuk perbaikan repositori ini sangat dipersilakan!