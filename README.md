# TERNAKPRO FINAL
Aplikasi Android manajemen ayam petelur. Project ini siap di-upload ke GitHub untuk build APK.

## Fitur final
Dashboard; periode/siklus ternak; ayam & kandang; produksi telur per kualitas; pakan & obat; penjualan; piutang dan pembayaran; biaya; kerugian; laba/rugi; FCR; filter periode; pencarian; Excel; cetak/Save as PDF; backup/restore.

## Upload ke GitHub
1. Buat repository baru bernama `ternakpro` di GitHub.
2. Upload **isi ZIP ini** (bukan ZIP sebagai satu file).
3. Pastikan folder `.github/workflows` dan file `build-apk.yml` ikut ter-upload.
4. Buka **Actions** → **Build TERNAKPRO APK**.
5. Jika belum berjalan otomatis, pilih **Run workflow**.
6. Setelah status hijau, buka workflow run tersebut → **Artifacts** → `TERNAKPRO-apk`.
7. Download artifact, ekstrak, lalu install APK di Android.

## Build lokal
`npm install` → `npm run build` → `npx cap add android` → `npx cap sync android` → `cd android` → `./gradlew assembleDebug`.

Data aplikasi tersimpan lokal di perangkat. Gunakan Backup dari menu Laporan sebelum mengganti HP atau menghapus aplikasi.
