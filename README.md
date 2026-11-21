# Willi Invoices

Invoice generator satu file untuk Willi Prabowo Endi. Satu `index.html`, tanpa build, tanpa server.

## Cara pakai

1. Buka `index.html` di browser (klik dua kali, atau lewat GitHub Pages). Internet hanya dibutuhkan untuk font Montserrat.
2. Isi form di kiri: nomor invoice, tanggal, klien, item, diskon, DP, dan info pembayaran.
3. Pratinjau di kanan ikut berubah langsung.
4. Klik **Print / Save PDF**, lalu pilih **Save as PDF** (ukuran A4, margin None).

Isian tersimpan otomatis di browser (localStorage) dan tidak pernah dikirim ke mana pun. Tombol **Reset** mengosongkan semuanya untuk invoice baru.

## Mengubah isi

Semua ada di bagian `<script>` di `index.html`:

- `SVC`: daftar layanan beserta harga batas bawah. Memilih nama layanan di kolom deskripsi mengisi harga otomatis.
- `fresh()`: nilai awal invoice (nama pengirim, kontak, info pembayaran, catatan, DP default 50%).

## Font

- Heading: Jetsy Trial (versi trial, personal use only; beli lisensinya sebelum dipakai untuk dokumen komersial).
- Angka: Chunk Party.
- Teks biasa: Montserrat (Google Fonts).

Kedua font display sudah tertanam di file, jadi tidak perlu folder `fonts/`.

## Catatan

- Data invoice tidak punya backup. Kalau cache browser dihapus, isiannya hilang, jadi simpan PDF-nya.
- Jangan tulis nomor rekening permanen di `fresh()` kalau repo ini public.
