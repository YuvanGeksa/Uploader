# GitHub File Uploader (Any Repo)

User tidak perlu edit kode. Di website, user cukup isi:
- GitHub token
- owner/username
- repository
- file ZIP

Lalu klik upload, dan file akan di-push ke repo tersebut (kalau token punya akses write).

## Run lokal
```bash
npm i
npm run dev
```

## Deploy ke Vercel
- Push folder ini ke GitHub
- Import project di Vercel
- Deploy (tanpa ENV)

## Catatan
- Upload dilakukan di browser memakai GitHub Contents API (per file).
- Token tidak disimpan.
- Karena ini bisa dipakai publik untuk repo mana pun, pertimbangkan menambah Access Code / rate limiting di versi berikutnya.
