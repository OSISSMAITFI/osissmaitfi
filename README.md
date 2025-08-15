# 🏫 OSIS SMAIT FITHRAH INSANI


## 📖 About

Welcome to the official repository of OSIS SMAIT Fithrah Insani! This repository serves as a central hub for our organization's digital resources and projects.

## 🎯 Vision & Mission

### Vision
Welcome to the official repository of OSIS SMAIT Fithrah ! This repository serves as a central hub for our organization's digital resources and projects.

### Mission
- 🌟 Integration of Islamic Values
- 📚 Discipline & Exemplary
- 🎨 Potential Development

## 🔧 Structure

- 👑 **Ketua OSIS**
- 👥 **Wakil Ketua**
- 📝 **Sekretaris**
- 💰 **Bendahara**
- 📋 **Divisi-divisi**
	- Divisi Keagamaan
	- Divisi Kedisiplinan
	- Divisi Pendidikan
	- Divisi Literasi
	- Divisi Bakat dan Minat
	- Divisi Kesehatan
	- Divisi Kewirausahaan
	- Divisi Media

## 📅 Programs

- Responsible for religious and spiritual activities at school.
- Develop a sense of nationalism and patriotism.
- Educate students to be insightful
- Educate students in the field of language
- Developing students' talents and creativity.
- Bertanggung jawab dalam kebersihan dan kesehatan.
- Train entrepreneurship and manage funds.
- Manage OSIS communications and information.

## 📞 Contact

- 📧 Email: [osissmaitfi@gmail.com]
- 📱 Instagram: [https://www.instagram.com/osissmaitfi/]
- 🌐 Website: [https://osissmaitfi.biezz.my.id/]

## 🤝 Contributing

We welcome contributions from all students! Feel free to:
- Submit suggestions for improvement
- Report issues
- Participate in our programs
- Share creative ideas

## ⚖️ License

© 2024 OSIS SMAIT Future Islamic. All Rights Reserved.

---
<div align="center">
	OSIS SMAIT FITHRAH INSANI
	BY: @biezz-2
</div>

Dibuat otomatis oleh tooling lokal untuk mempercepat setup.

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


