A. Ajukan KRS 
Tujuan                  |Mengajukan rencana studi (KRS) untuk semester berjalan.
Aktor Utama             |Mahasiswa
Sumber kebutuhan        |SIA-R03
Pemicu                  |Mahasiswa memilih menu Ajukan KRS dan menekan tombol Ajukan.
Prasayrat               |Pengguna telah terautentikasi; Data mata kuliah, prasyarat, dan jadwal tersedia.
Pascakondisi berhasil   |Pengajuan KRS tersimpan dengan status "menunggu persetujuan dosen wali".
Pascakondisi gagal      |Pengajuan tidak tersimpan dan sistem menampilkan pesan kesalahan
include                 |Validasi KRS
Extension point         |Pada titik konfirmasi penyimpanan pengajuan (setelah KRS berhasil disimpan).
Extend                  |-

B. Validasi KRS
Tujuan                  |Memeriksa kelayakan KRS yang diajukan (kelengkapan, prasyarat, benturan jadwal).
Aktor Utama             |Sistem
Sumber kebutuhan        |SIA-R04
Pemicu                  |Dimulainya proses pengajuan KRS oleh mahasiswa.
Prasayrat               |Use case Ajukan KRS telah dimulai dan mata kuliah telah dipilih.
Pascakondisi berhasil   |Status validasi "Berhasil" dikembalikan ke use case Ajukan KRS.
Pascakondisi gagal      |Status validasi "Gagal" beserta alasannya dikembalikan ke use case Ajukan KRS.
include                 |-
Extension point         |-
Extend                  |-

C. Unduh pengajuan bukti KRS
Tujuan                  |Mendapatkan dokumen bukti pengajuan KRS.
Aktor Utama             |Mahasiswa
Sumber kebutuhan        |SIA-R05
Pemicu                  |Pengajuan KRS berhasil disimpan dan mahasiswa memilih opsi "Unduh Bukti".
Prasayrat               |Pengajuan KRS berstatus "menunggu persetujuan dosen wali".
Pascakondisi berhasil   |File bukti pengajuan berhasil diunduh oleh mahasiswa.
Pascakondisi gagal      |Proses unduh gagal, namun pengajuan KRS tetap tersimpan (tidak membatalkan pengajuan).
include                 |-
Extension point         |-
Extend                  |Ajukan KRS

D. Proses keputusan KRS
Tujuan                  |Memberikan persetujuan atau penolakan terhadap KRS mahasiswa.
Aktor Utama             |Dosen Wali
Sumber kebutuhan        |SIA-R06
Pemicu                  |Dosen wali membuka daftar pengajuan KRS mahasiswa bimbingannya.
Prasayrat               |KRS berstatus "menunggu persetujuan" dan dosen wali telah terautentikasi.
Pascakondisi berhasil   |Status KRS diperbarui menjadi "Disetujui" (tersimpan dalam).
Pascakondisi gagal      |Status KRS diperbarui menjadi "Ditolak" dan dosen wali memberikan catatan keputusan.
include                 |-
Extension point         |-
Extend                  |-