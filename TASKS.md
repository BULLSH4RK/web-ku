# Task Breakdown — Website CV Aditya Yudha Hari Pratama

Base file sudah ada di `index.html` (single-file HTML, sudah termasuk hero, about, skills graph,
projects, education, contact). Breakdown di bawah ini untuk **penyempurnaan & finalisasi**,
dipecah kecil-kecil supaya tiap sesi Claude Code tetap ringan.

Kerjakan **1 task per sesi/prompt**. Jangan gabung beberapa task sekaligus.

---

## Task 1 — Setup project & baseline check
- Pindahkan `index.html` ke folder project.
- Buka di browser, screenshot tiap section (hero, about, skills, projects, education, contact).
- Catat bug visual/typo kalau ada (jangan diperbaiki dulu, cukup dicatat).

## Task 2 — Ganti foto profil
- Tambahkan foto profil di hero atau about section.
- Minta user upload file foto, simpan di folder `assets/`, referensikan via `<img>`.
- Pastikan ada fallback (inisial "AYHP" dalam lingkaran) kalau foto belum tersedia.

## Task 3 — Hubungkan CV PDF
- Minta user upload file CV PDF.
- Simpan di `assets/cv-aditya-yudha.pdf`.
- Update tombol "Unduh CV (PDF)" di hero supaya link ke file tersebut (pakai atribut `download`).

## Task 4 — Review copywriting
- Baca ulang teks di section About, Skills, Projects, Education.
- Tanyakan ke user: apakah ada detail yang salah/kurang (misal semester, tahun masuk kuliah, tanggal project).
- Update teks sesuai jawaban user. Jangan menambah klaim yang belum dikonfirmasi.

## Task 5 — Tambah 1 proyek terbaru (opsional)
- Kalau user punya proyek baru sejak website ini dibuat, tambahkan 1 card baru di timeline `#projects`.
- Ikuti struktur `.t-item` yang sudah ada (jangan ubah struktur CSS).

## Task 6 — Accessibility pass
- Cek kontras warna teks vs background di semua section (terutama teks abu di atas putih).
- Pastikan semua tombol/link punya focus state yang terlihat saat ditab pakai keyboard.
- Tambahkan `prefers-reduced-motion` media query untuk mematikan animasi typing & fade-up bagi user yang sensitif motion.

## Task 7 — Responsive check (mobile)
- Test tampilan di lebar layar 375px (mobile) dan 768px (tablet).
- Perbaiki spacing/overflow di skill graph SVG kalau terpotong di layar kecil.
- Pastikan side-nav dots (yang di-hide di mobile) tidak meninggalkan celah kosong.

## Task 8 — Performance & cleanup
- Cek apakah font Google Fonts loading terlalu lambat; pertimbangkan `font-display: swap` (biasanya sudah default, cukup diverifikasi).
- Minify tidak wajib, tapi pastikan tidak ada CSS/JS yang tidak terpakai.

## Task 9 — Deploy
- Tanyakan ke user platform deploy pilihan (GitHub Pages, Vercel, Netlify).
- Siapkan langkah deploy sesuai platform yang dipilih (misal GitHub Pages: push ke repo, enable Pages di Settings).
- Setelah live, update link GitHub/LinkedIn di CV fisik (PDF) atau profil lain supaya konsisten mengarah ke website ini.

## Task 10 — Final review
- Buka website versi live di browser & mobile asli (bukan simulator).
- Cek semua link kontak (GitHub, LinkedIn, TryHackMe, email) benar-benar mengarah ke tujuan yang tepat.
- Screenshot final, kirim ke user untuk approval.

---

### Catatan tambahan
- File utama: `index.html` (self-contained, tidak perlu build step).
- Kalau butuh restart context di Claude Code, cukup lampirkan `index.html` + task yang sedang dikerjakan, tidak perlu seluruh riwayat chat ini.
- Warna & font sudah didefinisikan sebagai CSS variable di `:root` — kalau mau ubah tema, cukup ubah di situ, tidak perlu ubah tiap section.
