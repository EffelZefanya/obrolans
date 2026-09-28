# Obrolans

Kartu obrolan digital: pilih kategori (Pasangan, Teman & Hangout, Keluarga, Kolega & Kerja, PDKT, Komunitas, Diri Sendiri), pilih topik dan dek, lalu kocok dan ambil kartu.

Satu file `index.html`, tanpa framework atau build step. Buka saja di browser.

## Menambah konten

Semua konten ada di bagian `DATA` di dalam `index.html`:

- **Kategori baru**: tambah objek di `AUDIENCES`.
- **Topik baru**: tambah di `TOPICS` (pakai `shared:true` kalau isinya sama untuk semua kategori).
- **Dek baru**: tambah `{ name, color, topic, cards }`.
- **Warna**: pakai nama dari `PALETTE`.
