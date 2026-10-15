# CGBUM Clone — Tema Blogger Komik

![CGBUM Clone](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj0yp-VRyoToD3u4pG4kre2uXSREbQ8orkUnWjdBGmpoC_wOp4dSNmx1Jj5UdK_MUrA3rdZ5Hsl9KgftgAKQtcKhLICSuYSGz2O9hBMzNUm2LWC1yAvnaujdbnPxWnevEa_g0gLba1qKI1B01njXXCwrv5Gjuao59aOQnPz3HPnuWwDx47c-7tPRKB8pQp9/s1600/1000280652.jpg)

**CGBUM Clone** adalah tema Blogger untuk situs baca komik (manga, manhwa, dan manhua). Tampilannya mengadaptasi katalog komik modern: kartu komik ringkas, halaman detail seri, filter genre, dan reader chapter bergaya webtoon. Tersedia dalam mode **gelap** dan **terang**.

> **Status: Versi 1 (tahap pengembangan).** Ini rilis awal. Fitur masih disempurnakan dan pembaruan perbaikan bug serta fitur baru akan dirilis kemudian.
>
> **Tanpa License.** Tema ini tidak memakai sistem lisensi, jadi tidak perlu kunci lisensi atau aktivasi apa pun.

---

## Informasi Tema

| Item | Keterangan |
|---|---|
| Nama Tema | CGBUM Clone |
| Platform | Blogger / Blogspot |
| Jenis Tema | Manga / Manhwa / Manhua |
| Mode Tampilan | Gelap & Terang |
| Format File | XML Blogger |
| License | Tidak memakai license |
| Download | Coming soon |


---

## Fitur

### Katalog dan Daftar Komik
- Halaman **Daftar Komik** (`/p/Daftar-Komik.html`) dengan filter **Tipe**, **Status**, **Genre** (maksimal 3 pilihan, ada kolom cari genre), dan **Urutan**.
- Daftar genre dibuat otomatis dari label yang kamu pakai.
- Halaman label, pencarian, dan arsip menampilkan breadcrumb, judul beserta jumlah komik, grid kartu, dan paginasi. Postingan Chapter otomatis disembunyikan sehingga hanya komik yang tampil.
- Paginasi ringkas (Prev / Hal. / Next). Jumlah komik per halaman diatur lewat widget **Blog Posts** di Blogger.

### Kartu Komik
- Cover otomatis dari gambar utama postingan Series.
- Badge tipe (Manga, Manhwa, Manhua), status (Ongoing, Completed/Tamat), dan badge **18+** untuk komik dewasa.
- Judul komik dan chapter terbaru beserta waktunya, misalnya `Ch. 40 · 57 menit lalu`.
- Grid responsif untuk ponsel dan desktop.

### Halaman Detail Komik
- Breadcrumb: Home › Tipe › Judul komik.
- Cover besar, judul, judul alternatif (dari deskripsi penelusuran postingan), dan genre berupa pill yang bisa diklik.
- Tipe, author, dan tanggal publikasi.
- Tombol **Simpan Favorit** dan tombol bagikan ke X, Facebook, WhatsApp, dan Telegram.
- Sinopsis dengan tombol "Lihat selengkapnya".
- Daftar chapter dimuat otomatis dari feed Blogger.

### Reader Chapter (Webtoon)
- Gambar HD selebar layar, di tengah, tanpa celah antar halaman. URL gambar otomatis dinaikkan ke resolusi asli (`/s0/`).
- Tombol menu melayang untuk membuka/menutup bar navigasi bawah. Saat dibuka, judul seri dan chapter muncul di bagian atas.
- **Auto-scroll** 4 kecepatan (Lambat, Normal, Cepat, Sangat Cepat). Berhenti saat layar disentuh atau di akhir chapter.
- **Tap gambar untuk turun**, jaraknya mengikuti kecepatan yang dipilih.
- Dropdown chapter di atas gambar dan di bar bawah, plus tombol Sebelumnya dan Berikutnya.
- Navigasi keyboard dengan panah kiri/kanan di desktop.
- Pengaturan kecepatan dan tap gambar tersimpan di browser.

### Filter Konten
Panel **Filter Konten** di header mengatur apa yang tampil di semua halaman katalog:
- **Tutup komik dewasa**: kartu berlabel dewasa ditutup dengan overlay "Ditutup".
- **Tutup Yaoi/Jomok**: menutup komik dengan label terkait.
- **Genre ditutup**: pilih genre yang tidak ingin ditampilkan.

Pilihan pembaca tersimpan di browser dan berlaku di Daftar Komik, halaman label, dan hasil pencarian.

> **Sesuaikan label dewasa.** Label yang dianggap dewasa dan Yaoi/Jomok ditentukan oleh daftar kecil di script (`ADULT` dan `YAOI`). Tambahkan label yang kamu pakai, dengan huruf kecil, agar badge 18+ dan filter bekerja sesuai isi blogmu.

### Komentar
Menampilkan jumlah komentar pada judul, pesan saat belum ada komentar, dan pesan saat komentar ditutup. Komentar hanya muncul di halaman postingan tunggal.

---

## Cara Kerja

Seluruh data dibaca langsung dari **feed Blogger**, tanpa database tambahan.

- Satu komik = satu postingan berlabel **`Series`** (cover, sinopsis, genre).
- Satu chapter = satu postingan berlabel **`Chapter`** (berisi gambar halaman).
- Keduanya dihubungkan oleh **label nama seri** yang sama.

---

## Panduan Label

Label adalah kunci utama tema ini. Ganti `Judul Komik` dengan judul komikmu:

```text
Postingan Series  : Series, Judul Komik, Manhwa, Ongoing, Action, Fantasy
Postingan Chapter : Chapter, Judul Komik
```

| Label | Fungsi |
|---|---|
| `Series` | Menandai halaman detail komik |
| `Chapter` | Menandai postingan chapter (reader) |
| Nama seri | Harus **sama persis** di postingan Series dan seluruh chapter-nya |
| `Manga` / `Manhwa` / `Manhua` | Tipe komik |
| `Ongoing` / `Completed` / `Tamat` | Status komik |
| `Action`, `Romance`, `School Life`, dst. | Genre |
| `Adult` (dan sejenisnya) | Memunculkan badge 18+ dan memberlakukan filter/blur konten dewasa |

**Judul chapter** sebaiknya berformat konsisten, misalnya `One Piece Chapter 1192`. Nomor pada judul dipakai untuk label `Ch. 1192` dan untuk mengurutkan daftar chapter.

> **Tips:** Penulisan label bersifat *case-sensitive* pada beberapa bagian tema. Tentukan format sejak awal (misalnya selalu `Manhwa`, bukan kadang `manhwa`).

---

## Pemasangan

1. **Cadangkan tema lama.** Dari menu **Tema** di Blogger, simpan cadangan sebelum mengganti template.
2. **Unggah file XML.** Gunakan opsi **Pulihkan (Restore)** pada menu Tema, lalu pilih file XML CGBUM Clone.
3. **Atur jumlah postingan per halaman.** Buka **Tata Letak**, edit widget **Blog Posts**, lalu isi jumlah yang sesuai dengan grid (misalnya `24`).
4. **Buat halaman statis.** Buat halaman **Daftar Komik** dengan tautan permanen kustom `Daftar-Komik`, lalu halaman **History** jika dipakai. Tempel kode halaman pada tampilan HTML.
5. **Buat postingan percobaan.** Satu postingan Series dan dua postingan Chapter dengan label sesuai panduan.
6. **Uji tampilan dan fitur.** Periksa halaman label, Daftar Komik, halaman detail, reader (auto-scroll, tap gambar, dropdown chapter), filter konten, favorit, dan komentar, terutama di ponsel.

> Lakukan pengujian di blog percobaan sebelum diterapkan ke blog utama.

---

## Format Isi Chapter

Isi postingan Chapter cukup berupa gambar halaman yang berurutan:

```html
<div class="separator" style="clear: both;">
  <a href="URL-GAMBAR/s0/halaman-1.jpg">
    <img alt="Halaman 1" src="URL-GAMBAR/s0/halaman-1.jpg"/>
  </a>
</div>
```

**Gambar terlihat buram?** Blogger sering menyimpan gambar dengan batas `/s1600/`, yang mengecilkan lebar pada gambar sangat panjang. Gunakan `/s0/` pada URL gambar. Reader sudah mengubahnya otomatis, tetapi mengubahnya langsung di postingan lebih hemat bandwidth.

---

## Favorit dan Riwayat

- Tombol **Simpan Favorit** ada di halaman detail komik.
- Riwayat membaca menyimpan komik yang pernah dibuka beserta chapter terakhirnya, tampil di halaman **History Baca** dengan tombol hapus per komik.

> Favorit dan riwayat disimpan di browser (`localStorage`), sehingga berbeda antar perangkat/browser dan hilang jika data browser dibersihkan. Ini bukan sinkronisasi akun.

---

## Schema.org

Tema menyertakan markup schema.org:

- **BreadcrumbList** pada breadcrumb halaman detail, reader, dan katalog.
- **ItemList** dan **ListItem** pada grid komik di halaman label, pencarian, dan arsip.
- **JSON-LD** pada postingan tunggal: `ComicSeries` (Series), `ComicIssue` (Chapter), `BlogPosting` (postingan biasa), `WebPage` (halaman statis).
- **Comment** pada setiap komentar, lengkap dengan penulis dan jumlah komentar.

Markup ini membantu mesin pencari memahami konten, tetapi tidak menjamin tampil sebagai hasil yang diperkaya. Uji dengan *Rich Results Test* atau *Schema Markup Validator* setelah tema terpasang.

---

## Batasan

- Chapter terbaru pada kartu diambil dari **500 postingan Chapter terbaru**. Pada katalog yang sangat besar, komik lama bisa tampil tanpa info chapter.
- Feed Blogger dimuat bertahap (150 postingan per permintaan) dan di-cache sementara selama 10 menit.
- Favorit, riwayat, dan pengaturan reader disimpan per browser.
- Nama label harus konsisten, terutama label nama seri.
- Gunakan gambar yang sudah dioptimalkan untuk web dan hindari script tambahan yang fungsinya tumpang tindih.
- Pastikan kamu memiliki izin atau hak atas konten komik yang dipublikasikan.
- Uji ulang seluruh fitur setiap kali mengubah XML atau JavaScript.

---

## FAQ

**Apakah bisa dipakai di Blogger gratis?**
Ya. Tema ini hanya memakai fitur bawaan Blogger: label, feed, dan halaman statis.

**Apakah label `Series` dan `Chapter` wajib?**
Ya. `Series` menentukan halaman detail dan daftar komik, `Chapter` menentukan reader. Tanpa keduanya, postingan tampil sebagai postingan biasa.

**Kenapa chapter terbaru tidak muncul di kartu komik?**
Biasanya label nama seri di postingan Chapter berbeda dengan di postingan Series, atau chapter tersebut berada di luar 500 postingan Chapter terbaru. Samakan penulisan labelnya.

**Kenapa gambar chapter buram?**
Cek URL gambarnya. Jika masih `/s1600/`, ganti dengan `/s0/`. Jika file aslinya beresolusi rendah, tema tidak bisa memperbaikinya.

**Apakah favorit dan riwayat sinkron antar perangkat?**
Tidak. Datanya tersimpan di browser masing-masing perangkat.

**Apakah perlu license key?**
Tidak. Tema ini tidak memakai license.

---

## Penutup

CGBUM Clone menggabungkan katalog komik yang terstruktur, reader chapter yang nyaman di ponsel, dan filter konten yang bisa diatur pembaca, semuanya di atas fitur bawaan Blogger. Dengan label yang konsisten dan pengujian yang teliti, tema ini siap dijadikan dasar situs baca komik.

Tutorial Blogger, template website, HTML, CSS, JavaScript, dan pembahasan pengembangan web lainnya tersedia di **Hiru404**.
