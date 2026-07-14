# Personal Portfolio Website

Website portofolio pribadi modern, bersih, dan responsif yang dibangun menggunakan HTML5 semantik dan CSS3 murni (Flexbox & CSS Grid).

## Apa yang Saya Buat
Sebuah halaman web portofolio statis satu halaman (Single Page Application layout) yang memuat informasi profil profesional, biografi singkat, daftar keahlian teknis, etalase proyek pemrograman front-end yang telah dikerjakan, serta formulir kontak operasional untuk pesan pengunjung.

## Masalah yang Dihadapi
1. **Responsivitas Grid:** Mengatur agar daftar proyek berbentuk kartu terlihat rapi di layar HP yang sempit dan otomatis melebar menjadi 3 kolom di layar PC.
2. **Fleksibilitas Section Tentang:** Menggabungkan profil teks dan list kemampuan agar posisinya sejajar secara horizontal di layar besar tetapi bertumpuk vertikal di layar kecil.

## Bagaimana Saya Mengatasinya
1. **Solusi Grid:** Menggunakan properti `display: grid` pada CSS dengan setelan dasar 1 kolom (`grid-template-columns: 1fr`). Kemudian memanfaatkaan Media Query `@media (min-width: 768px)` untuk mengubahnya menjadi 2 kolom, dan `@media (min-width: 1024px)` menjadi 3 kolom.
2. **Solusi Flexbox:** Menggunakan `display: flex` dengan properti `flex-direction: column` untuk tampilan mobile bawaan, dan mengubah arahnya menjadi `flex-direction: row` saat resolusi layar mencapai lebar tablet/desktop (>768px).