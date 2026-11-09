# JKS Time Planner

Web satu file (`index.html`) untuk bikin Excel Time Management Salesman dari JKS Genap + Route Feedback.
Waktu tempuh diambil dari OSRM (rute jalan), bukan jarak lurus.

## Deploy
1. Taruh `index.html` di root repo GitHub.
2. Di Vercel: Add New Project, pilih repo, Framework Preset "Other", tanpa build command. Deploy.

## Cara pakai
1. Upload JKS Genap dan Route Feedback.
2. (Opsional) Buka "Kalibrasi faktor waktu", upload file Rute Kunjungan (RutaMap), pakai faktor yang disarankan.
3. Pilih salesman, klik Hitung rute, cek preview, lalu Export.

## Catatan
- Salesman dicocokkan lewat Id Salesman, bukan nama.
- Server OSRM publik (router.project-osrm.org) ada batas pemakaian wajar dan menghitung waktu mobil tanpa macet.
  Alamat server bisa diganti di panel Aturan kalau punya server sendiri.
- Library dimuat dari cdnjs (SheetJS 0.18.5, ExcelJS 4.4.0), jadi butuh internet.
