Elemen                | SIA-UC07 — Lihat Kalender Akademik                              |
Sumber kebutuhan      | SIA-R07                                                         |
Tujuan                | Menampilkan kalender akademik resmi institusi                   |
Aktor utama           | Civitas Akademika (Mahasiswa dan Dosen)                         |
Pemicu                | Civitas akademika memilih fungsi lihat kalender akademik        |
Prasyarat             | Pengguna telah terautentikasi; data kalender akademik tersedia  |
Pascakondisi berhasil | Kalender akademik resmi institusi ditampilkan                   |
Pascakondisi gagal    | Kalender akademik tidak ditampilkan; tidak ada data yang berubah|
Include               | -                                                               |
Extension point       | -                                                               |
Extend                | -                                                               |
Collaboration         | -                                                               |
Generalization        | -                                                               |


Elemen                | SIA-UC08 — Input Nilai Mata Kuliah                              |
Sumber kebutuhan      | SIA-R08 dan SIA-R12                                             |
Tujuan                | Menyimpan nilai mata kuliah yang diinput oleh dosen pengampu    |
Aktor utama           | Dosen                                                           |
Pemicu                | Dosen memilih fungsi input nilai mata kuliah                    |
Prasyarat             | Dosen telah terautentikasi; dosen adalah pengampu mata kuliah;  |
                      | masa perkuliahan telah berakhir                                 |
Pascakondisi berhasil | Nilai mata kuliah tersimpan dan berstatus belum terpublikasi    |
Pascakondisi gagal    | Nilai tidak tersimpan dan data nilai tidak berubah              |
Include               | SIA-UC09 — Lihat KHS                                            |
Extension point       | -                                                               |
Extend                | -                                                               |
Collaboration         | SIA-CO01 — realisasi Input Nilai Mata Kuliah                    |
Generalization        | -                                                               |


Elemen                | SIA-UC09 — Lihat KHS                                            |
Sumber kebutuhan      | SIA-R09 dan SIA-R12                                             |
Tujuan                | Menampilkan Kartu Hasil Studi semester yang nilainya            |
                      | sudah dipublikasikan                                            |
Aktor utama           | Mahasiswa                                                       |
Pemicu                | Mahasiswa memilih fungsi lihat KHS                              |
Prasyarat             | Mahasiswa telah terautentikasi; nilai semester telah            |
                      | dipublikasikan                                                  |
Pascakondisi berhasil | KHS semester yang dipilih ditampilkan                           |
Pascakondisi gagal    | KHS tidak ditampilkan; tidak ada data yang berubah              |
Include               | -                                                               |
Di-include oleh       | SIA-UC08 — Input Nilai Mata Kuliah                              |
Extension point       | -                                                               |
Extend                | -                                                               |
Collaboration         | SIA-CO02 — realisasi Lihat KHS                                  |
Generalization        | -                                                               |


Elemen                | SIA-UC10 — Kelola Data Mahasiswa                                |
Sumber kebutuhan      | SIA-R10 dan SIA-R11                                             |
Tujuan                | Mengelola data mahasiswa melalui tambah, ubah, dan hapus        |
Aktor utama           | Admin Akademik                                                  |
Pemicu                | Admin akademik memilih fungsi kelola data mahasiswa             |
Prasyarat             | Admin akademik telah terautentikasi dan memiliki hak akses      |
Pascakondisi berhasil | Data mahasiswa berhasil ditambah, diubah, atau dihapus sesuai   |
                      | bentuk yang dipilih                                             |
Pascakondisi gagal    | Data mahasiswa tidak berubah                                    |
Include               | -                                                               |
Extension point       | -                                                               |
Extend                | -                                                               |
Collaboration         | -                                                               |
Generalization        | Induk dari SIA-UC11, SIA-UC12, dan SIA-UC13                     |


Elemen                | SIA-UC11 — Tambah Data Mahasiswa                                |
Sumber kebutuhan      | SIA-R11                                                         |
Tujuan                | Menambahkan data mahasiswa baru ke sistem                       |
Aktor utama           | Admin Akademik                                                  |
Pemicu                | Admin akademik memilih bentuk tambah data mahasiswa             |
Prasyarat             | Admin akademik telah terautentikasi; data mahasiswa baru lengkap|
Pascakondisi berhasil | Data mahasiswa baru tersimpan                                   |
Pascakondisi gagal    | Data mahasiswa baru tidak tersimpan                             |
Include               | -                                                               |
Extension point       | -                                                               |
Extend                | -                                                               |
Collaboration         | -                                                               |
Generalization        | SIA-UC10 — Kelola Data Mahasiswa                                |


Elemen                | SIA-UC12 — Ubah Data Mahasiswa                                  |
Sumber kebutuhan      | SIA-R11                                                         |
Tujuan                | Memperbarui data mahasiswa yang sudah ada                       |
Aktor utama           | Admin Akademik                                                  |
Pemicu                | Admin akademik memilih bentuk ubah data mahasiswa               |
Prasyarat             | Admin akademik telah terautentikasi; data mahasiswa yang        |
                      | diubah tersedia                                                 |
Pascakondisi berhasil | Perubahan data mahasiswa tersimpan                              |
Pascakondisi gagal    | Data mahasiswa tidak berubah                                    |
Include               | -                                                               |
Extension point       | -                                                               |
Extend                | -                                                               |
Collaboration         | -                                                               |
Generalization        | SIA-UC10 — Kelola Data Mahasiswa                                |


Elemen                | SIA-UC13 — Hapus Data Mahasiswa                                 |
Sumber kebutuhan      | SIA-R11                                                         |
Tujuan                | Menghapus data mahasiswa yang tidak lagi diperlukan             |
Aktor utama           | Admin Akademik                                                  |
Pemicu                | Admin akademik memilih bentuk hapus data mahasiswa              |
Prasyarat             | Admin akademik telah terautentikasi; mahasiswa tidak memiliki   |
                      | data akademik aktif (ketentuan fiktif latihan)                  |
Pascakondisi berhasil | Data mahasiswa terhapus                                         |
Pascakondisi gagal    | Data mahasiswa tidak terhapus                                   |
Include               | -                                                               |
Extension point       | -                                                               |
Extend                | -                                                               |
Collaboration         | -                                                               |
Generalization        | SIA-UC10 — Kelola Data Mahasiswa                                |