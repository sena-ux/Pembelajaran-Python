1️⃣ LIST

📌 List adalah kumpulan data berurutan, bisa diubah (mutable), dan boleh duplikat.

🔹 Ciri-ciri List

Menggunakan []

Bisa berisi berbagai tipe data

Index dimulai dari 0

Bisa diubah (tambah, hapus, edit)

🔹 Contoh List
buah = ["apel", "jeruk", "mangga"]
angka = [1, 2, 3, 4]
campur = ["python", 3.10, True]

🔹 Akses Data
print(buah[0])     # apel
print(buah[-1])    # mangga

🔹 Mengubah Data
buah[1] = "pisang"

🔹 Menambah Data
buah.append("anggur")
buah.insert(1, "melon")

🔹 Menghapus Data
buah.remove("apel")
buah.pop()
del buah[0]

🔹 Loop List
for b in buah:
    print(b)

🔹 List Bersarang
nilai = [
    ["Andi", 80],
    ["Budi", 90]
]

print(nilai[0][0])  # Andi


📌 List cocok untuk: data yang sering berubah
contoh: keranjang belanja, daftar siswa, absensi

2️⃣ TUPLE

📌 Tuple adalah kumpulan data berurutan, tidak bisa diubah (immutable).

🔹 Ciri-ciri Tuple

Menggunakan ()

Lebih aman dari perubahan

Lebih cepat dari list

Boleh duplikat

🔹 Contoh Tuple
koordinat = (10, 20)
hari = ("Senin", "Selasa", "Rabu")

🔹 Akses Tuple
print(hari[0])  # Senin

❌ Tidak Bisa Diubah
hari[0] = "Minggu"  # ERROR

🔹 Tuple Unpacking
x, y = (5, 10)
print(x)  # 5
print(y)  # 10


📌 Tuple cocok untuk: data tetap
contoh: koordinat, konfigurasi, konstanta

3️⃣ DICTIONARY (DICT)

📌 Dictionary adalah kumpulan data key : value, tidak berurutan, mutable.

🔹 Ciri-ciri Dict

Menggunakan { }

Akses pakai key, bukan index

Key unik

Value bebas

🔹 Contoh Dictionary
siswa = {
    "nama": "Andi",
    "kelas": "XI RPL",
    "nilai": 85
}

🔹 Akses Data
print(siswa["nama"])

🔹 Menambah / Mengubah Data
siswa["nilai"] = 90
siswa["alamat"] = "Denpasar"

🔹 Menghapus Data
del siswa["kelas"]

🔹 Loop Dictionary
for key, value in siswa.items():
    print(key, ":", value)

🔹 Dict Bersarang
data = {
    "siswa1": {"nama": "Andi", "nilai": 80},
    "siswa2": {"nama": "Budi", "nilai": 90}
}

print(data["siswa2"]["nilai"])


📌 Dict cocok untuk: data terstruktur
contoh: user, artikel, konfigurasi, JSON API

4️⃣ SET

📌 Set adalah kumpulan data unik, tidak berurutan, tanpa index.

🔹 Ciri-ciri Set

Menggunakan { }

Tidak boleh duplikat

Tidak bisa akses pakai index

Mutable

🔹 Contoh Set
angka = {1, 2, 3, 3, 4}
print(angka)  # {1,2,3,4}

🔹 Menambah Data
angka.add(5)

🔹 Menghapus Data
angka.remove(2)

🔹 Operasi Set (PENTING 🔥)
A = {1, 2, 3}
B = {3, 4, 5}

print(A | B)  # union
print(A & B)  # intersection
print(A - B)  # difference


📌 Set cocok untuk:

Hilangkan duplikasi

Perbandingan data
contoh: cek user unik, daftar hadir unik
