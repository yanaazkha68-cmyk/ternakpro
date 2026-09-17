# Struktur Data TERNAKPRO

## Entitas
- periode_ternak: satu siklus ternak dari ayam masuk sampai selesai.
- kandang: kapasitas dan lokasi.
- batch_ayam: populasi per pembelian/sumber.
- produksi_harian: populasi, kematian, telur, pakan, kesehatan.
- stok: pakan/obat/vaksin dan mutasinya.
- penjualan + detail_penjualan: transaksi telur/ayam.
- pelanggan + piutang + pembayaran_piutang.
- biaya: biaya operasional.
- kerugian: ayam/telur/pakan.
- kas: uang masuk/keluar.

## Rumus inti
Ayam hidup = ayam awal + ayam masuk - mati - hilang - terjual

Stok = stok awal + masuk - terpakai - rusak - hilang

Nilai penjualan = kuantitas x harga satuan

Sisa piutang = total transaksi kredit - seluruh pembayaran

Laba kotor = pendapatan - biaya operasional

Laba bersih = pendapatan - biaya operasional - kerugian

Produksi (%) = telur / rata-rata ayam hidup x 100

FCR telur = kg pakan / kg telur

## Aturan penting
1. Penjualan kredit tidak langsung menambah kas; masuk ke piutang.
2. Pembayaran piutang menambah kas dan mengurangi saldo piutang.
3. Ayam mati mengurangi populasi dan dicatat sebagai kerugian.
4. Telur retak/busuk tidak masuk penjualan normal.
5. Semua mutasi stok tidak boleh mengubah stok tanpa membuat riwayat transaksi.
