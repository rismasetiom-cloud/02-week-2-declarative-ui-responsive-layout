# Laporan Praktikum Modul 02: Declarative UI & Responsive Layout

- **Nama**: [RISMA SETIO MUHTAFIROH]
- **NIM**: [362558302037]
- **Kelas / Prodi**: 2C - TEKNOLOGI REKAYASA PERANGKAT LUNAK
- **Mata Kuliah**: Pemrograman Perangkat Bergerak (Semester 3)

---

## 1. Ringkasan Implementasi
Saya merancang dashboard responsif dengan LayoutBuilder dan tema Material 3 pada modul 2 ini awalnya karna memang mengikuti modul, tapi dari situ saya mengerti dam menahami bagaimana konsep mob dev itu bekerja. menggunakan konsep widget tata letak fundamental (Row, Column, Expanded, Flexible, spacer, stack), mengelola state dengan StatefulWidget, serta merancang antarmuka responsif yang adaptif terhadap berbagai resolusi layar hp dan laptop. 
yang artinya ketika saya menggunakan Flexible berarti widget akan otomatis menyesuaikan ukuran secara fleksibel. Row digunakkan untuk menyusun widget agar posisinya horizontal (dari kiri ke kanan) begitupun sebaliknya ketika menggunakan Column yang nantinya akan menyusun widget secara vertikal (dari atas kebawah). 


## 2. Bukti Tangkapan Layar (Running App)
| Mode Portrait (Light) | Mode Dark Theme | Mode Landscape / Tablet (2 Kolom) |
|---|---|---|
| ![Portrait](./screenshots/Screenshot%202026-09-09%20032319.png) | ![Dark](./screenshots/Screenshot%202026-09-09%20032330.png) | ![Wide](./screenshots/Screenshot%202026-09-09%20033417.png) |

## 3. Kendala Layout yang Dihadapi & Solusinya
- **Kendala**: [Ketidak sesuaian frame/layout, jadi yg awalnya muncul garis2 hitam malah jadi nggak muncul apa2 kalau dipaksa mode potrait]
- **Solusi**: [Mengganti Column (krn awalnya saya pake column) menjadi widget yg scrollable yaitu ListView. agar tampilannya dapat menyesuaikan secara otomatis dengan berbagai resolusi tanpa harus error lagi]

## 4. Jawaban Pertanyaan Refleksi
1. **Efisiensi Single-pass BoxConstraints**: [Efisiensi mekanis layout Single-pass BoxConstraints di Flutter terletak pada efektivitasnya dalam meminimalkan beban komputasi saat rendering UI. Dengan prinsip utama "Constraints Go Down, Sizes Go Up, Parent Sets Position", Flutter hanya perlu menelusuri pohon widget (widget tree) sebanyak satu kali jalan saja untuk menentukan ukuran dan posisi setiap elemen. Proses ini sangat efisien karena parent widget langsung menurunkan batasan ukuran minimum dan maksimum, kemudian child widget menentukan ukurannya sendiri secara mandiri di dalam batasan tersebut sebelum melaporkannya kembali ke atas.]

2. **Kriteria Modularisasi Widget**: [Kriteria pertama adalah reusability, yang berarti bahwa komponen antarmuka pengguna, seperti tombol kustom atau kartu data, dapat digunakan di berbagai tempat, sehingga tidak perlu membaginya menjadi widget kecil untuk mempermudah debugging dan kerja tim. Kriteria kedua adalah manajemen kompleksitas, yang berarti bahwa membagi komponen UI menjadi widget kecil akan mencegah duplikasi kode. Terakhir, elemen isolasi status dan kinerja rendering juga sangat penting.]

3. **Manfaat M3 ThemeData Terpusat**: [agar system/aplikasi yang dibuat memiliki design yang konsisten, mulai dari warnanya, font, spasing, hingga ukuran fontnya. Dan apabila terjadi error hanya perlu memperbaikinya di satu file aja, lebih praktis tanpa harus menyeting properti disetiap widget yg lain secara manual.]
