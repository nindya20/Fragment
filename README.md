# Fragment
Fragment merupakan kombinasi sebuah layout XML dan kelas java yang mirip dengan sebuah Activity yang memiliki fungsi untuk menampilkan antarmuka ke pengguna. Dengan menggunakan support library, fragment dapat mendukung hampir semua versi Android. Fragment digunakan agar komponen tampillan aplikasi menjadi fleksibel dan dapat digunakan kembali (reusable). Fragment merupakan komponen utuh yang memiliki view, event, dan logic (meskipun tetap membutuhkan sebuah fragment agar dapat bekerja).

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
![109187982-0325be80-77c5-11eb-8e0e-c9cb9907ae22](https://user-images.githubusercontent.com/60589822/111760253-13672000-88d1-11eb-8b28-0ead431a8351.png)
1. onAttach() dipanggil saat sebuah fragment terhubung ke activity.
2. onCreate() diapnggil saat sebuah fragment dibuat (objeknya di memori).
3. onCreateView() dipanggil saat fragment sudah siap membaca sebuah layout.
4. onViewCreated() dipanggil setelah onCreateView() dan memastikan layout yang dibaca fragment adalah non-null. Semua pengaturan view seperti pembacaan findViewById, menambah onClickListener dapat dilakukan di sini.
5. onActivityCreated() dipanggil setelah activity pembaca sudah menyelesaikan onCreate()-nya.
6. onStart() dipanggil setelah fragment siap untuk ditampilkan di layar.
7. onResume() - Dipakai untuk melakukan pembacaan data yang lebih “rumit” seperti lokasi, sensor, dll.
8. onPause() - Tempat melepas data “rumit”. Lakukan commit di sini.
9. onDestroyView() dipanggil saat layout sebuah fragment akan dihapus dari memori, namun fragmentnya masih ada di memori.
10. onDetach() dipanggil saat fragment tidak lagi terhubung ke sebuah activity.

# Pembuatan Sebuah Fragment
Sebuah fragment, seperti activity, memiliki XML layout-nya sendiri dan sebuah kelas java sebagai controller dari Fragment tersebut.Layout XML yang dimiliki oleh fragment, sama seperti layout-layout lainnya dan bisa memiliki nama apa saja (selama memiliki format yang ditentukan).

# Penerapan Fragment
![WhatsApp Image 2021-03-19 at 16 18 47](https://user-images.githubusercontent.com/60589822/111758805-7bb50200-88cf-11eb-9103-5375208c50cc.jpeg)
![WhatsApp Image 2021-03-19 at 16 18 45](https://user-images.githubusercontent.com/60589822/111758829-840d3d00-88cf-11eb-8954-d93017618f6d.jpeg)
