# 💍 Invitify — Undangan Digital Pernikahan

Platform undangan digital pernikahan yang elegan dan lengkap.

## 📁 Struktur File

```
wedding-invitation/
├── index.html          ← Landing Page utama
├── themes.html         ← Halaman galeri tema
├── form.html           ← Formulir pengisian data undangan (untuk customer)
├── passkeys.json       ← File konfigurasi passkey customer ← EDIT DI SINI
└── README.md
```

## 🚀 Deploy ke GitHub Pages

1. Buat repository baru di GitHub
2. Upload semua file ke repository
3. Pergi ke **Settings → Pages**
4. Pilih source: **Deploy from a branch → main → / (root)**
5. Klik **Save**
6. Website akan tersedia di: `https://username.github.io/nama-repo`

## 🔑 Mengelola Passkey Customer

Edit file `passkeys.json` untuk menambah/mengelola passkey:

```json
{
  "passkeys": {
    "NAMAPASANGAN2024": {
      "customer": "Nama Pasangan",
      "theme": "elegant-rose",
      "package": "Standard",
      "created": "2024-01-01",
      "active": true
    }
  }
}
```

### Tema yang tersedia:
- `elegant-rose` — Pink romantis
- `garden-green` — Hijau alami
- `royal-gold` — Hitam & emas mewah
- `minimalist-white` — Putih minimalis
- `rustic-wood` — Coklat kayu vintage

### Untuk menonaktifkan passkey:
Ubah `"active": true` menjadi `"active": false`

## 📦 Paket yang Tersedia

| Paket | Harga | Masa Aktif |
|-------|-------|------------|
| Basic | Rp99.000 | 3 bulan |
| Standard | Rp199.000 | 6 bulan |
| Premium | Rp349.000 | 12 bulan |

## 🛠 Alur Kerja

1. **Customer pesan** via WhatsApp → Link: wa.me/6282388308450
2. **Bayar & konfirmasi** → Anda kirimkan passkey via WhatsApp
3. **Customer buka** website → masuk ke "Area Pelanggan" → input passkey
4. **Isi formulir** data undangan (nama, tanggal, foto, dll)
5. **Klik Simpan** → File HTML undangan otomatis ter-download
6. **Kirimkan file HTML** ke customer atau deploy ke GitHub Pages

## 💬 Kontak & WhatsApp

Link WhatsApp: `https://wa.me/6282388308450`

Untuk mengubah nomor WhatsApp, cari dan ganti `6282388308450` di semua file HTML.

## 📝 Catatan Penting

- File undangan yang dihasilkan adalah **standalone HTML** — bisa langsung dibuka di browser
- Foto yang diupload disimpan sebagai **base64** di dalam file HTML
- Ucapan tamu tersimpan di **localStorage** browser masing-masing tamu
- Untuk production, pertimbangkan menggunakan backend (Node.js/PHP) untuk menyimpan data secara permanen

---

Made with ❤️ by Invitify
