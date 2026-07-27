# Completion Notes

## Ringkasan penyelesaian

- File utama telah dipindahkan ke folder project.
- Halaman CV telah disempurnakan dengan profil visual, tautan unduh CV, penyesuaian mobile, dan fokus keyboard yang lebih jelas.
- Konten proyek diperbarui dengan satu card tambahan untuk portofolio website CV.
- Aset profil dan file PDF placeholder disimpan di folder assets.

## Review akhir

- Semua section utama sudah tersedia: hero, about, skills, projects, education, dan contact.
- Tautan kontak sudah mengarah ke email, GitHub, LinkedIn, dan TryHackMe.
- Tombol unduh CV sudah mengarah ke file PDF di folder assets.
- Layout sudah disesuaikan untuk layar mobile dan mendukung fokus keyboard serta reduced motion.

## Panduan deploy

### GitHub Pages

1. Buat repository GitHub baru (atau gunakan repository yang sudah ada).
2. Upload seluruh isi folder project ke repository tersebut.
3. Buka tab Settings > Pages di repository GitHub.
4. Pada bagian Build and deployment, pilih Source: Deploy from a branch.
5. Pilih branch utama, misalnya `main`, lalu pilih folder `/root`.
6. Klik Save dan tunggu hingga status berubah menjadi "Your site is live at ...".
7. Setelah selesai, buka URL yang diberikan untuk melihat website.

### Catatan penting

- Karena website ini adalah file statis, tidak ada build step yang diperlukan.
- Pastikan file utama yang dipublikasikan adalah `index.html` di root repository atau folder yang dipilih.
- Jika Anda ingin URL lebih rapi, gunakan nama repository yang singkat dan jelas.

## Catatan lanjutan

- Jika ingin, file CV dapat diganti dengan versi PDF asli yang lebih formal.
- Untuk hasil yang lebih matang, lakukan pengujian langsung di perangkat mobile setelah deployment.
