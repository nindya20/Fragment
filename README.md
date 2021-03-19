# Fragment
Fragment merupakan kombinasi sebuah layout XML dan kelas java yang mirip dengan sebuah Activity yang memiliki fungsi untuk menampilkan antarmuka ke pengguna. Dengan menggunakan support library, fragment dapat mendukung hampir semua versi Android. Fragment digunakan agar komponen tampillan aplikasi menjadi fleksibel dan dapat digunakan kembali ( reusable). Fragment merupakan komponen utuh yang memiliki view, event, dan logic (meskipun tetap membutuhkan sebuah fragment agar dapat bekerja).

Fragment juga bisa disebut sub nya activity (Sebuah fragment harus berada di dalam sebuah activity, mereka tidak dapat berjalan sendiri tanpa adanya activity tempat mereka menempel). Dalam satu activity bisa memiliki lebih dari satu fragment.

# Pentingnya Sebuah Fragment
- Penggunaan Komponen View dan Logic Berulang Kali : Fragment dapat dipakai untuk menampilkan data atau melakukan event tertentu dibeberapa activity berbeda.
- Dukungan Untuk Tablet : Fragment memungkinkan activity untuk menggunakan fragment dalam membuat antarmuka sesuai dengan perangkat yang membukanya.
- Orientasi Layar : Fragment memungkinkan untuk menggunakan tampilan yang berbeda( horizontal atau vertikal) menggunakan elemen yang sama.

# Keuntungan Menggunakan Fragment
- [x] Tidak perlu memasukkan nama file fragment ke dalam “AndroidManifest” yang diperlukan oleh activity.
- [x] Fungsi yang berada pada activity dapat langsung digunakan dalam fragment tersebut tanpa harus membuat ulang.

# Fragment Lifecycle
Fragment memiliki sirkulasi kehidupan atau yang biasanya disebut “lifecycle”, seperti yang ditunjukkan pada Gambar di bawah ini :


