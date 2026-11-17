# Diary App – React Native Redux Toolkit

## Deskripsi Project

Diary App merupakan aplikasi mobile sederhana yang dibuat menggunakan React Native, Expo, TypeScript, dan Redux Toolkit.

Aplikasi ini digunakan untuk mencatat aktivitas sehari-hari, memilih suasana hati (mood), menyimpan diary ke daftar favorite, mengedit catatan, dan menghapus diary.

## Teknologi yang Digunakan

- React Native
- Expo
- TypeScript
- Redux Toolkit
- React Redux
- Expo Router

## Fitur Aplikasi

1. Menampilkan daftar diary.
2. Menambahkan diary baru.
3. Mengedit diary.
4. Menghapus diary.
5. Menambahkan dan menghapus favorite.
6. Menghapus semua favorite.
7. Filter diary berdasarkan mood.
8. Statistik Total Diary dan Total Favorite.
9. Validasi judul minimal 3 karakter.
10. Empty state pada Home dan Favorites.

## Perbedaan Local State, Global Redux State, dan Persistent Database

### 1. Local State

Local State adalah state yang digunakan untuk mengelola data sementara pada satu komponen.

Pada aplikasi Diary App, Local State menggunakan useState.

Contohnya:
- Input judul diary.
- Input isi diary.
- Pemilihan mood.
- Filter mood yang sedang dipilih.

Local State cocok digunakan untuk data yang hanya dibutuhkan oleh komponen tertentu.

### 2. Global Redux State

Global Redux State adalah state yang dapat diakses oleh beberapa komponen atau screen dalam aplikasi.

Pada aplikasi Diary App, Redux Toolkit digunakan untuk mengelola data diary secara terpusat.

Contohnya:
- Daftar diary.
- Judul dan isi diary.
- Mood diary.
- Status favorite.

Redux menggunakan Store, Action, Reducer, Dispatch, dan Selector untuk mengelola perubahan data.

### 3. Persistent Database

Persistent Database adalah tempat penyimpanan data secara permanen sehingga data tetap tersedia meskipun aplikasi ditutup atau dijalankan kembali.

Contohnya:
- MySQL
- PostgreSQL
- SQLite
- Firebase

Pada praktikum ini, aplikasi belum menggunakan database permanen. Redux Store hanya menyimpan data di memory aplikasi sehingga data yang ditambahkan dapat kembali ke initialState setelah aplikasi direstart.

## Kesimpulan

Berdasarkan praktikum ini, Redux Toolkit membantu mengelola global state pada aplikasi React Native secara terstruktur.

Local State digunakan untuk mengelola input sementara, sedangkan Redux Toolkit digunakan untuk mengelola data diary yang dibutuhkan oleh beberapa screen.

Persistent Database memiliki fungsi berbeda, yaitu menyimpan data secara permanen.

Dengan menggunakan Redux Toolkit, perubahan data pada Home, Create, Favorites, dan Detail dapat tersinkronisasi melalui satu Redux Store.