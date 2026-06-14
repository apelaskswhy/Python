Sintaks dasar Python adalah **aturan penulisan kode Python** agar komputer dapat memahami instruksi yang diberikan. Tanpa sintaks, kode hanya menjadi teks biasa yang sok pintar tetapi tidak bisa dijalankan. Tragis, seperti manusia yang punya rencana hidup tapi tidak punya langkah konkret.

# Sintaks Dasar Python

## 1. `print()`

Digunakan untuk menampilkan output ke layar.

```python
print("Halo, dunia!")
```

Output:

```text
Halo, dunia!
```

---

## 2. Komentar

Komentar adalah catatan dalam kode yang **tidak dijalankan** oleh Python.

```python
# Ini adalah komentar
print("Belajar Python")
```

Komentar dipakai untuk menjelaskan maksud kode, bukan untuk menulis novel penderitaan batin.

---

## 3. Variabel

Variabel adalah tempat menyimpan data.

```python
nama = "Mughni"
umur = 16
tinggi = 165.5
aktif = True
```

Penjelasan:

```python
nama    # string / teks
umur    # integer / bilangan bulat
tinggi  # float / bilangan desimal
aktif   # boolean / True atau False
```

---

## 4. Tipe Data Dasar

Python memiliki beberapa tipe data dasar:

```python
teks = "Python"          # str
angka = 10               # int
desimal = 3.14           # float
benar = True             # bool
daftar = [1, 2, 3]       # list
data = ("A", "B")        # tuple
unik = {1, 2, 3}         # set
profil = {"nama": "Ali"} # dict
```

---

## 5. Input Pengguna

Digunakan untuk menerima data dari pengguna.

```python
nama = input("Masukkan nama: ")
print("Halo,", nama)
```

Catatan penting: `input()` selalu menghasilkan **string**.

Kalau ingin angka:

```python
umur = int(input("Masukkan umur: "))
```

---

## 6. Operator

### Operator Aritmatika

```python
a = 10
b = 3

print(a + b)  # tambah
print(a - b)  # kurang
print(a * b)  # kali
print(a / b)  # bagi
print(a // b) # bagi bulat
print(a % b)  # sisa bagi
print(a ** b) # pangkat
```

### Operator Perbandingan

```python
print(10 > 5)   # True
print(10 < 5)   # False
print(10 == 10) # True
print(10 != 5)  # True
```

### Operator Logika

```python
print(True and True)
print(True or False)
print(not True)
```

---

## 7. Percabangan `if`, `elif`, `else`

Digunakan untuk membuat keputusan.

```python
nilai = 85

if nilai >= 90:
    print("Sangat baik")
elif nilai >= 75:
    print("Baik")
else:
    print("Perlu belajar lagi")
```

Python menggunakan **indentasi** untuk menentukan blok kode.

Ini benar:

```python
if True:
    print("Benar")
```

Ini salah:

```python
if True:
print("Benar")
```

Python akan marah. Dan kali ini, Python benar.

---

## 8. Perulangan `for`

Digunakan untuk mengulang berdasarkan urutan data.

```python
for angka in range(1, 6):
    print(angka)
```

Output:

```text
1
2
3
4
5
```

Contoh dengan list:

```python
buah = ["apel", "mangga", "pisang"]

for item in buah:
    print(item)
```

---

## 9. Perulangan `while`

Digunakan untuk mengulang selama kondisi masih benar.

```python
angka = 1

while angka <= 5:
    print(angka)
    angka += 1
```

Hati-hati dengan infinite loop:

```python
while True:
    print("Tidak berhenti")
```

Kode seperti ini berjalan selamanya, seperti overthinking manusia yang tidak punya tombol stop.

---

## 10. Fungsi

Fungsi adalah blok kode yang dapat dipakai ulang.

```python
def sapa(nama):
    print("Halo,", nama)

sapa("Mughni")
```

Fungsi dengan `return`:

```python
def tambah(a, b):
    return a + b

hasil = tambah(5, 3)
print(hasil)
```

---

## 11. List

List digunakan untuk menyimpan banyak data dalam satu variabel.

```python
angka = [10, 20, 30]

print(angka[0])
print(angka[1])
print(angka[2])
```

Index dimulai dari **0**, bukan 1. Karena programmer rupanya sepakat membuat pemula sedikit menderita.

Menambah data:

```python
angka.append(40)
```

Menghapus data:

```python
angka.remove(20)
```

---

## 12. Dictionary

Dictionary menyimpan data dalam bentuk **key-value**.

```python
siswa = {
    "nama": "Mughni",
    "kelas": "10 RPL",
    "umur": 16
}

print(siswa["nama"])
print(siswa["kelas"])
```

---

## 13. Import Modul

Digunakan untuk memakai fitur tambahan.

```python
import math

print(math.sqrt(16))
```

Contoh lain:

```python
import random

angka = random.randint(1, 10)
print(angka)
```

---

## 14. Error Handling

Digunakan untuk menangani kesalahan agar program tidak langsung berhenti.

```python
try:
    angka = int(input("Masukkan angka: "))
    print(10 / angka)
except ValueError:
    print("Input harus berupa angka.")
except ZeroDivisionError:
    print("Tidak bisa membagi dengan nol.")
```

---

# Contoh Program Dasar Lengkap

```python
def hitung_status(nilai):
    if nilai >= 75:
        return "Lulus"
    else:
        return "Tidak lulus"


nama = input("Masukkan nama: ")
nilai = int(input("Masukkan nilai: "))

status = hitung_status(nilai)

print("Nama:", nama)
print("Nilai:", nilai)
print("Status:", status)
```

---

# Langkah Progres Menuju Ahli Python

Urutan belajar yang masuk akal:

1. **Pahami sintaks dasar**

   Variabel, tipe data, input, output, operator, `if`, loop, fungsi.

2. **Latih logika pemrograman**

   Buat program kecil seperti kalkulator, biodata, sistem nilai, konversi suhu, dan validasi umur.

3. **Kuasai struktur data**

   Pelajari `list`, `tuple`, `set`, dan `dictionary`.

4. **Pelajari fungsi dengan serius**

   Biasakan membuat kode yang rapi, tidak menumpuk semua di satu tempat seperti kamar remaja setelah ujian.

5. **Masuk ke file handling**

   Belajar membaca dan menulis file `.txt`, `.csv`, atau `.json`.

6. **Pelajari OOP**

   Class, object, method, inheritance, encapsulation.

7. **Gunakan library**

   Contoh:

   ```python
   math
   random
   datetime
   os
   json
   requests
   pandas
   flask
   django
   ```

8. **Buat proyek nyata**

   Contoh:

   * aplikasi kasir sederhana
   * sistem login
   * todo list
   * web sederhana dengan Flask
   * scraping data
   * bot otomatisasi
   * API sederhana

9. **Pelajari testing dan debugging**

   Ahli Python bukan orang yang tidak pernah error. Ahli Python adalah orang yang tahu cara menemukan dan memperbaiki error.

10. **Baca dokumentasi resmi**

Ini tahap ketika seseorang mulai berhenti menebak-nebak dan mulai menjadi programmer sungguhan.

---

# Kesimpulan

Sintaks dasar Python mencakup **aturan penulisan kode**, seperti variabel, tipe data, input-output, percabangan, perulangan, fungsi, struktur data, modul, dan penanganan error.

Untuk menjadi ahli Python, jangan hanya menghafal sintaks. Gunakan sintaks itu untuk **membangun program nyata**. Karena kemampuan coding tidak lahir dari membaca definisi saja, melainkan dari menulis kode, membuat error, memperbaikinya, lalu mengulangi siklus menyedihkan itu sampai otakmu akhirnya tunduk pada logika.

