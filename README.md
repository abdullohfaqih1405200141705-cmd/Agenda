# YaumiyahQu (APK Android)

Bismillah. Proyek ini membungkus aplikasi web `src/index.html` menjadi APK dengan Capacitor.
APK dikompilasi online oleh GitHub Actions, tanpa Android Studio.

## Langkah (sekitar 10 menit, lewat komputer)
1. Buka https://github.com/new, buat repositori baru (nama bebas, mis. `yaumiyahqu`).
2. Ekstrak zip ini. Di halaman repositori pilih **Add file → Upload files**,
   lalu seret SEMUA isi folder (termasuk folder `.github` dan `src`). Tekan **Commit changes**.
3. Buka tab **Actions**. Proses "Bangun APK YaumiyahQu" jalan otomatis (2–5 menit).
   Jika tidak, pilih proses itu lalu **Run workflow**.
4. Setelah hijau, buka **Releases** di halaman utama repositori, lalu unduh `YaumiyahQu.apk`.
5. Di HP: ketuk berkas APK, izinkan "Pasang dari sumber ini" jika diminta, lalu pasang.

## Catatan
- Jika tombol unggah folder `.github` tidak terbaca, buat berkas lewat **Add file → Create new file**
  dengan nama `.github/workflows/build-apk.yml` lalu tempel isinya.
- APK ini bertanda tangan kunci debug: aman dipasang di HP sendiri, tetapi belum untuk Play Store.
- Mengubah tampilan: edit `src/index.html`, commit, lalu APK baru dibuat otomatis.
- Alarm hitung mundur berbunyi saat aplikasi terbuka. Untuk alarm saat aplikasi tertutup,
  perlu plugin `@capacitor/local-notifications`.
