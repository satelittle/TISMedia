# Landing Page — Jasa Digital Marketing

Situs statis satu file (`index.html`), tanpa build, tanpa database.

## Yang wajib diganti sebelum online

| Placeholder | Lokasi |
|---|---|
| `Nama Agensi` | judul tab, meta, logo, footer |
| `62XXXXXXXXXXX` | `WA_NUMBER` di bagian `<script>` paling bawah (format 628xxx, tanpa + dan spasi) |
| `[HARGA]` | 3 kartu paket |
| `[JUMLAH]` | kartu Press Release |
| `[DURASI]` | FAQ kontrak minimum |
| `[ALAMAT EMAIL]` | bagian kontak (2 tempat) |
| `[KOTA]` | footer |

Formulir tidak butuh server: saat dikirim, isinya dibuka sebagai pesan WhatsApp ke `WA_NUMBER`.

## Struktur

```
index.html          halaman
deploy/nginx.conf   konfigurasi Nginx (diblokir dari publik)
```

## Update setelah online

Mac: edit → `git commit` → `git push`
Server: `cd /var/www/landing-digital-marketing && git pull`
