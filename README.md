# osissmaitfi

Website OSIS SMA IT FTI — kumpulan halaman HTML, gambar, dan aset statis yang digunakan untuk situs organisasi.

Isi utama:
- `index.html` — halaman depan
- `about.html`, `people.html`, `our-social-media.html`, `bidang.html` — halaman statis lain
- folder `about/`, `global/`, `sekbid/` — aset gambar dan halaman sub

Tujuan repository ini:
- Menyimpan versi situs statis.
- Memudahkan deployment/hosting (GitHub Pages, hosting statis lain).

Panduan singkat (jika ingin push ke GitHub dari mesin Anda):

1. Pastikan Anda berada di folder proyek:

```powershell
cd /d J:\bhaskara\bhaskara
```

2. Inisialisasi git (jika belum):

```powershell
git init
git add -A
git commit -m "Initial commit: add website files, README, LICENSE, .gitignore"
git branch -M main
git remote add origin git@github.com:OSISSMAITFI/osissmaitfi.git
git push -u origin main
```

Jika push gagal karena autentikasi SSH, lihat bagian "SSH / HTTPS" di bawah.

SSH / HTTPS:
- Preferred: siapkan kunci SSH dan tambahkan ke GitHub. Lalu gunakan remote `git@github.com:OSISSMAITFI/osissmaitfi.git`.
- Alternatif: gunakan HTTPS remote `https://github.com/OSISSMAITFI/osissmaitfi.git` dan autentikasi dengan PAT.

Lisensi dan .gitignore disediakan di repo ini; sesuaikan bila perlu.

Kontak & kolaborator:
- Untuk menambah kolaborator, buka halaman repo di GitHub -> Settings -> Manage access -> Invite collaborators.

---

Dibuat otomatis oleh tooling lokal untuk mempercepat setup. Sesuaikan README ini sesuai kebutuhan tim.
