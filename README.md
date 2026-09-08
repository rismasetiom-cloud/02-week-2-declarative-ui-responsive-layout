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
1. **Efisiensi Single-pass BoxConstraints**: [...]
2. **Kriteria Modularisasi Widget**: [...]
3. **Manfaat M3 ThemeData Terpusat**: [agar system/aplikasi yang dibuat memiliki design yang konsisten, mulai dari warnanya, font, spasing, hingga ukuran fontnya. Dan apabila terjadi error hanya perlu memperbaikinya di satu file aja, lebih praktis tanpa harus menyeting properti disetiap widget yg lain secara manual.]
