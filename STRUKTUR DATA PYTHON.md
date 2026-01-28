# 📘 Python Data Structure Dasar

Materi ini membahas 4 struktur data utama dalam Python:
- **List**
- **Tuple**
- **Dictionary**
- **Set**

---

## 1️⃣ LIST

📌 **List** adalah kumpulan data **berurutan**, **mutable (bisa diubah)**, dan **boleh duplikat**.

### 🔹 Ciri-ciri List
* Menggunakan kurung siku `[]`
* Bisa berisi berbagai tipe data
* Index dimulai dari `0`
* Bisa diubah (tambah, hapus, edit)

### 🔹 Contoh Kode List
```python
buah = ["apel", "jeruk", "mangga"]
angka = [1, 2, 3, 4]
campur = ["python", 3.10, True]
```
# Akses Data
```python
print(buah[0])     # Output: apel
print(buah[-1])    # Output: mangga (ambil dari belakang)
```
# Mengubah Data
```python
buah[1] = "pisang"
```
# Menambah Data
```python
buah.append("anggur")     # Menambah di akhir
buah.insert(1, "melon")   # Menambah di index spesifik
```
# Menghapus Data
```python
buah.remove("apel")       # Berdasarkan nilai
buah.pop()                # Menghapus paling akhir
del buah[0]               # Berdasarkan index
```
# Loop List
```python
for b in buah:
    print(b)
```
# List Bersarang (Nested List)
```python
nilai = [
    ["Andi", 80],
    ["Budi", 90]
]
print(nilai[0][0])  # Output: Andi
```
## 2️⃣ TUPLE

📌 Tuple adalah kumpulan data berurutan dan tidak bisa diubah (immutable).

### 🔹 Ciri-ciri Tuple

1. Menggunakan ()
2. Lebih aman dari perubahan
3. Lebih cepat dari list
4. Boleh duplikat

### 🔹 Contoh Tuple
```python
koordinat = (10, 20)
hari = ("Senin", "Selasa", "Rabu")
```
### 🔹 Akses Tuple
```python
print(hari[0])  # Senin
```
❌ Tidak Bisa Diubah
```python
hari[0] = "Minggu"  # ERROR
```
### 🔹 Tuple Unpacking
```python
x, y = (5, 10)
print(x)  # 5
print(y)  # 10
```

📌 Tuple cocok untuk:
Data tetap
Contoh: koordinat, konfigurasi, konstanta

## 3️⃣ DICTIONARY (DICT)

📌 Dictionary adalah kumpulan data key : value, tidak berurutan, mutable.

### 🔹 Ciri-ciri Dict

1. Menggunakan { }
2. Akses pakai key, bukan index
3. Key unik
4. Value bebas

### 🔹 Contoh Dictionary
```python
siswa = {
    "nama": "Andi",
    "kelas": "XI RPL",
    "nilai": 85
}
```
### 🔹 Akses Data
```python
print(siswa["nama"])
```
### 🔹 Menambah / Mengubah Data
```python
siswa["nilai"] = 90
siswa["alamat"] = "Denpasar"
```
###🔹 Menghapus Data
```python
del siswa["kelas"]
```
### 🔹 Loop Dictionary
```python
for key, value in siswa.items():
    print(key, ":", value)
```
### 🔹 Dict Bersarang
```python
data = {
    "siswa1": {"nama": "Andi", "nilai": 80},
    "siswa2": {"nama": "Budi", "nilai": 90}
}

print(data["siswa2"]["nilai"])
```

📌 Dict cocok untuk: data terstruktur
contoh: user, artikel, konfigurasi, JSON API

## 4️⃣ SET

📌 Set adalah kumpulan data unik, tidak berurutan, tanpa index.

### 🔹 Ciri-ciri Set

1. Menggunakan { }
2. Tidak boleh duplikat
3. Tidak bisa akses pakai index
4. Mutable

### 🔹 Contoh Set
```python
angka = {1, 2, 3, 3, 4}
print(angka)  # {1,2,3,4}
```
### 🔹 Menambah Data
```python
angka.add(5)
```
### 🔹 Menghapus Data
```python
angka.remove(2)
```
### 🔹 Operasi Set (PENTING 🔥)
```python
A = {1, 2, 3}
B = {3, 4, 5}

print(A | B)  # union
print(A & B)  # intersection
print(A - B)  # difference
```

📌 Set cocok untuk:

Hilangkan duplikasi
Perbandingan data
contoh: cek user unik, daftar hadir unik
