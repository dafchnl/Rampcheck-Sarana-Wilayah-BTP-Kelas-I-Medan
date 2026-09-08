# BTP Kelas I Medan — Monitoring & Rampcheck

## File GitHub
- `index.html` — halaman Login, Daftar Akun, Verifikasi Email, dan Reset Password.
- `dashboard.html` — Dashboard Rampcheck.

## Alur sistem
**Daftar → kode verifikasi 6 angka → verifikasi email → persetujuan admin untuk pengguna biasa → Login → otomatis masuk Dashboard.**

- Kode verifikasi hanya menerima **angka** dan maksimal 6 digit.
- Password yang dibuat saat pendaftaran **tidak diubah saat verifikasi email**.
- Dashboard tanpa sesi login akan otomatis kembali ke halaman login.
- Logout menghapus sesi dan kembali ke halaman login.

## Google Apps Script Auth
Web App Auth yang dipakai:
`https://script.google.com/macros/s/AKfycbwl8-xNtLhTeCdFxvrXMrkslqslFXEgaoqHBcv3RiXEbLzF2-uiowYXwRlRWmhW5T_v/exec`

Backend Web App tersebut harus tetap aktif dan dapat diakses oleh halaman GitHub Pages.

## Upload ke GitHub
1. Buat repository baru.
2. Upload `index.html`, `dashboard.html`, dan `README.md`.
3. Buka **Settings → Pages**.
4. Pilih **Deploy from a branch**.
5. Branch: `main`, folder: `/ (root)`.
6. Simpan.

Setelah aktif, buka alamat GitHub Pages repository. Halaman pertama yang tampil adalah `index.html`.
