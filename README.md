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

## Cara upload / push repo ini ke GitHub

Panduan singkat untuk meng-upload seluruh isi folder proyek ke GitHub dari PowerShell (Windows, `pwsh.exe`). Pilih salah satu metode (SSH direkomendasikan).

- Pastikan berada di folder proyek:

```powershell
cd /d J:\bhaskara\bhaskara
```

- Jika belum ada repo git lokal, inisialisasi dan commit semua file:

```powershell
# Inisialisasi dan commit
git init
git add -A
git commit -m "Initial commit: add website files, README, LICENSE, .gitignore"
git branch -M main
```

- Opsi A — Push via SSH (direkomendasikan)

1. Buat kunci SSH (jika belum):

```powershell
ssh-keygen -t ed25519 -C "you@example.com" -f $env:USERPROFILE\.ssh\id_ed25519 -N ""
```

2. Salin public key dan tambahkan ke GitHub (Settings → SSH and GPG keys → New SSH key):

```powershell
Get-Content $env:USERPROFILE\.ssh\id_ed25519.pub | Set-Clipboard
```

3. (Jika perlu) jalankan ssh-agent dan tambahkan key — atau gunakan per-command SSH (tidak perlu agent):

```powershell
# Jalankan agent (memerlukan hak admin)
Set-Service -Name ssh-agent -StartupType Automatic
Start-Service ssh-agent
ssh-add $env:USERPROFILE\.ssh\id_ed25519

# Alternatif: gunakan ssh per-command tanpa agent
# git -c core.sshCommand="ssh -i C:/Users/<user>/.ssh/id_ed25519 -o IdentitiesOnly=yes" push -u origin main
```

4. Set remote SSH dan push:

```powershell
git remote add origin git@github.com:OSISSMAITFI/osissmaitfi.git
git pull origin main --allow-unrelated-histories   # jika remote berisi commit lain
git push -u origin main
```

- Opsi B — Push via HTTPS (gunakan Personal Access Token)

```powershell
git remote set-url origin https://github.com/OSISSMAITFI/osissmaitfi.git
git pull origin main --allow-unrelated-histories
git push -u origin main
```

Saat diminta autentikasi over HTTPS, gunakan GitHub username dan Personal Access Token (PAT) sebagai password.

Troubleshooting singkat:
- "Permission denied (publickey)": pastikan public key dipasang di akun GitHub yang punya akses ke repo.
- "Updates were rejected because the remote contains work that you do not have locally": jalankan `git pull origin main --allow-unrelated-histories` lalu selesaikan konflik, atau jika Anda ingin menimpa remote gunakan `git push --force` (berisiko).

Menambah collaborator:
- Pemilik repo dapat menambahkan kolaborator via GitHub → Settings → Manage access → Invite collaborators.

---


