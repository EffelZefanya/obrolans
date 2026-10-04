# Obrolans

Kartu obrolan digital. Pilih mau ngobrol sama siapa (Pasangan, Teman & Hangout, Keluarga, Kolega & Kerja, PDKT, Komunitas, Diri Sendiri), pilih dek, lalu kocok dan ambil kartu.

Setiap dek punya deskripsi singkat dan label kedalaman (**Ringan** atau **Dalam**). Dek *Dalam* kadang memberi pertanyaan lanjutan.

Satu file `index.html`, tanpa framework atau build step. Buka saja di browser.

## Menambah konten

Semua konten ada di bagian `DATA` di dalam `index.html`:

- **Kategori baru**: tambah objek di `AUDIENCES`. Pakai `solo:true` untuk main sendirian, `pair:true` untuk berdua.
- **Dek khusus satu kategori**: tambah `{ name, color, depth, desc, cards }` di `decks` kategori itu.
- **Dek umum**: tambah di `SHARED_DECKS`. Isi `for:['pasangan', ...]` untuk membatasi ke kategori tertentu, atau hapus `for` supaya muncul di semua kategori.
- **`depth`**: `'ringan'` atau `'dalam'`.
- **`tag`** (opsional): label pendek, mis. `'Game · 3+ orang'`.
- **Warna**: pakai nama dari `PALETTE`.
- **Suasana kategori**: isi `theme` di kategori (warna latar, punggung kartu, font, pola, sudut, tulisan di punggung kartu). Pilihan font dan pola ada di komentar `DATA`.
