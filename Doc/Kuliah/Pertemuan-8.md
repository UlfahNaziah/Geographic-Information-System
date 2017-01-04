Sistem Informasi Geografis – Konfigurasi MapProxy

1. Latar Belakang

MapProxy adalah proxy open source untuk data geospasial. Cache, mempercepat dan mengubah data dari layanan peta yang ada dan melayani setiap desktop atau web GIS klien.

1. Pembahasan

Konfigurasi menggunakan format YAML. Ada dua file konfigurasi yang digunakan oleh MapProxy. _mappproxy.yaml_

Ini adalah konfigurasi utama MapProxy. Ini mengkonfigurasi semua aspek server: Yang server harus dimulai, di mana berasal data dari, apa yang harus di-cache, dll.

seed.yaml

Service

Di sini Anda dapat mengkonfigurasi layanan harus dimulai. Konfigurasi untuk semua layanan yang dijelaskan dalam dokumentasi Layanan.

Berikut adalah contoh:

services:

  tms:

  wms:

    md:

      title: MapProxy Example WMS

      contact:

      # [...]

Layers

Di sini Anda dapat mendefinisikan semua lapisan MapProxy harus menawarkan. Definisi lapisan mirip dengan WMS: setiap lapisan dapat memiliki nama dan judul dan Anda dapat lapisan sarang untuk membangun pohon lapisan. Lapisan harus dikonfigurasi sebagai daftar (- di YAML), di mana setiap konfigurasi lapisan adalah kamus (key: nilai dalam YAML)

Contoh:

layers:

  - name: mylayer

    title: My Layer

    source: [mysoruce]

1. Penutup

1. Kesimpulan

MapProxy adalah proxy open source untuk data geospasial. Cache, mempercepat dan mengubah data dari layanan peta yang ada dan melayani setiap desktop atau web GIS klien.

1. Saran

Untuk memahami lebih jelasnya alangkah lebih baiknya jika kita mencari di buku-buku yang terpercaya atau melakukan praktikum sendiri.

Link Github:

Plagiarism:

Referensi