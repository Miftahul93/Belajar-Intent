# Belajar-Intent

Intent adalah mekanisme untuk melakukan sebuah action dan komunikasi antar komponen aplikasi misal Activity, Services, dan Broadcast Receiver. Ada tiga penggunaan umum Intent dalam aplikasi Android yaitu:

    Memindahkan satu Activity ke Activity lain dengan atau tidak membawa data.
    Menjalankan background Service misal melakukan sinkronisasi ke server dan menjalankan proses berulang (periodic/scheduler task).
    Mengirimkan obyek broadcast ke app yang membutuhkan. Misal jika aplikasi membutuhkan proses menjalankan sebuah background service setiap aplikasi selesai melakukan booting. Aplikasi harus bisa menerima obyek Broadcast yang dikirimkan oleh sistem Android untuk event booting tersebut.


Intent memiliki dua bentuk yaitu:

    Explicit Intent adalah tipe intent yang digunakan untuk menjalankan komponen dari dalam sebuah aplikasi. Explicit intent bekerja dengan menggunakan nama kelas yang dituju misal : com.dicoding.activity.DetailActivity. Umumnya intent ini digunakan untuk mengaktifkan komponen pada satu aplikasi.
    Implicit Intent adalah tipe intent yang tidak memerlukan detail nama kelas yang ingin diaktifkan, ini memungkinkan komponen dari aplikasi lain bisa merespon request intent yang dijalankan. Penggunaan tipe Intent ini umumnya diperuntukan untuk menjalankan fitur/fungsi dari komponen aplikasi lain. Contohnya ketika kita membutuhkan aplikasi kita untuk mengambil foto, daripada kita harus membuat sendiri fungsi kamera lebih baik kita menyerahkan proses tersebut pada aplikasi kamera bawaan dari device atau aplikasi kamera lain yang telah terinstal sebelumnya di device atau juga jika kita membutuhkan untuk fungsi berbagi konten, kita bisa memanfaatkan intent untuk menampilkan mana saja aplikasi yang bisa menawarkan fungsi berbagi (share) konten. Implementasi Intent Implicit ini akan sangat memudahkan bagi pengembang agar tetap fokus pada proses bisnis inti dari aplikasi yang dikembangkan.
