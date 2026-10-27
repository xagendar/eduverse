# EDUVERSE — Prototaip Unit Emas (T1-MT-B01-U01)

Fail data untuk menguji unit "Kenali 1 hingga 10" di GitHub Pages.

## Struktur folder

```
(akar repo)
├─ index.html              ← pemain unit (langkah seterusnya)
├─ css/    js/
├─ data/
│  ├─ kurikulum.json       ← rangka subjek, bab dan unit
│  ├─ kemahiran.json
│  ├─ audio-manifest.json  ← senarai klip audio + teks untuk dirakam
│  ├─ unit/T1-MT-B01-U01.json
│  └─ soalan/T1-MT-B01-U01.json
├─ audio/                  ← letak fail MP3 di sini (N01.mp3, AR01.mp3, ...)
└─ aset/                   ← gambar (prototaip guna emoji dahulu)
```

## Cara terbit di GitHub Pages

1. Cipta repo baharu (cadangan: nama berasingan daripada prototaip lama) atau guna folder baharu dalam repo sedia ada.
2. Upload semua fail dan folder ini ke cabang `main`.
3. Settings > Pages > Source: "Deploy from a branch" > Branch: `main` / folder `/ (root)` > Save.
4. Tunggu 1 hingga 2 minit. Alamat: `https://<nama-pengguna>.github.io/<nama-repo>/`

## Perkara yang selalu menyusahkan

- **Jangan buka index.html dengan klik dua kali** semasa menguji. Pelayar menyekat `fetch()` fail JSON daripada `file://`. Guna "Live Server" (VS Code) atau `python3 -m http.server`.
- **Guna laluan relatif** (`data/kurikulum.json`), bukan `/data/...`. Di GitHub Pages, tapak berada di bawah `/<nama-repo>/`.
- **Nama fail sensitif huruf besar/kecil** di GitHub (Linux). `N01.mp3` bukan `n01.mp3`.
- **Audio perlu ketikan pengguna dahulu** pada telefon. Letak skrin "Mula" yang perlu diketik sebelum audio pertama dimainkan.
- **Cache:** selepas kemas kini, tekan muat semula paksa, atau tambah `?v=2` pada URL fail data.
- **Tambah** `<meta name="robots" content="noindex">` dalam index.html supaya prototaip tidak muncul dalam Google.
- **Repo awam = semua kandungan boleh dilihat.** Sesuai untuk unit percuma ini. Jangan letak kandungan berbayar di sini.
- **Data murid:** untuk pilot, simpan kemajuan dalam `localStorage` pelayar sahaja (tiada data keluar daripada peranti). Jangan kumpul nama penuh atau maklumat peribadi kanak-kanak.

## Perubahan kecil daripada bahan sebelum ini

Supaya objek konsisten dengan set tetap (1 bola, 2 kasut, 3 epal, 4 bunga, 5 ikan, 6 telur, 7 burung, 8 belon, 9 buku, 10 bintang): Q03 kini kasut, Q12 bunga, Q13 belon, Q14 telur. Audio bertambah 4 klip (AR19, AC01, AC03, AC04), jumlah 32.
