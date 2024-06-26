# Kunci-Jawaban-EAS-Strukdat
### Nomor 1
Gambarkan AVL-tree dari deretan nilai: k, m, u, t, v, p, x.

### Proses Pembentukan AVL Tree:

### Langkah 1: Masukkan k
```
k
```

### Langkah 2: Masukkan m
```
  k
   \
    m
```

### Langkah 3: Masukkan u
```
  k
   \
    m
     \
      u
```
(Tidak seimbang, putar kiri pada k)
```
  m
 / \
k   u
```

### Langkah 4: Masukkan t
```
  m
 / \
k   u
   /
  t
```
(Tidak seimbang, putar kanan pada u)
```
  m
 / \
k   t
     \
      u
```

### Langkah 5: Masukkan v
```
  m
 / \
k   t
     \
      u
       \
        v
```
(Tidak seimbang, putar kiri pada t)
```
  m
 / \
k   u
   / \
  t   v
```

### Langkah 6: Masukkan p
```
  m
 / \
k   u
   / \
  t   v
 /
p
```
(Tidak seimbang, putar kanan pada t)
```
  m
 / \
k   u
   / \
  p   v
   \
    t
```

### Langkah 7: Masukkan x
```
  m
 / \
k   u
   / \
  p   v
   \   \
    t   x
```
(Tidak seimbang, kita perlu melakukan beberapa rotasi untuk menyeimbangkan. Setelah beberapa rotasi, hasil akhir adalah:)
```
      t
     / \
    m   v
   / \ / \
  k  p u  x
```

### Penjelasan Rotasi Akhir:

- Masukkan 'p': Menyebabkan ketidakseimbangan di sub-pohon kiri dari 'u', sehingga dilakukan rotasi kanan pada 't' menjadi:
```
      m
     / \
    k   u
       / \
      p   v
```
- Masukkan 'x': Menyebabkan ketidakseimbangan di sub-pohon kanan dari 'u', sehingga dilakukan rotasi kiri pada 'u' menjadi:
```
      t
     / \
    m   v
   / \ / \
  k  p u  x
```

Dengan langkah-langkah ini, kita mendapatkan AVL tree yang seimbang:
```
      t
     / \
    m   v
   / \ / \
  k  p u  x
```

### Nomor 2
Gambarkan AVL-tree dari deretan nilai: a, z, b, y, c, x, d, w, e, v, f.

### Proses pembentukan AVL-tree:
1. Masukkan a (AVL tree hanya memiliki root a).
2. Masukkan z (a tetap root, z di sebelah kanan a).
3. Masukkan b (a tetap root, z di sebelah kanan a, b di sebelah kanan a).
4. Masukkan y (a tetap root, z di sebelah kanan a, b di sebelah kanan a, y di sebelah kiri z).
5. Masukkan c (a tetap root, z di sebelah kanan a, b di sebelah kanan a, y di sebelah kiri z, c di sebelah kanan b).
6. Masukkan x (a tetap root, z di sebelah kanan a, b di sebelah kanan a, y di sebelah kiri z, c di sebelah kanan b, x di sebelah kiri y).
7. Masukkan d (a tetap root, z di sebelah kanan a, b di sebelah kanan a, y di sebelah kiri z, c di sebelah kanan b, x di sebelah kiri y, d di sebelah kanan c).
8. Masukkan w (a tetap root, z di sebelah kanan a, b di sebelah kanan a, y di sebelah kiri z, c di sebelah kanan b, x di sebelah kiri y, d di sebelah kanan c, w di sebelah kiri x).
9. Masukkan e (a tetap root, z di sebelah kanan a, b di sebelah kanan a, y di sebelah kiri z, c di sebelah kanan b, x di sebelah kiri y, d di sebelah kanan c, w di sebelah kiri x, e di sebelah kanan d).
10. Masukkan v (a tetap root, z di sebelah kanan a, b di sebelah kanan a, y di sebelah kiri z, c di sebelah kanan b, x di sebelah kiri y, d di sebelah kanan c, w di sebelah kiri x, e di sebelah kanan d, v di sebelah kiri w).
11. Masukkan f (a tetap root, z di sebelah kanan a, b di sebelah kanan a, y di sebelah kiri z, c di sebelah kanan b, x di sebelah kiri y, d di sebelah kanan c, w di sebelah kiri x, e di sebelah kanan d, v di sebelah kiri w, f di sebelah kanan e).

#### AVL Tree final:
```
        d
      /   \
     b     x
    / \   / \
   a   c w   y
         / \ / \
        e   v   z

```

### Nomor 3
#### a) Hapus Node `c`:
```
      h
     / \
    e   l
   / \  / \
  b   f j   m
 / \   \   / \
a   d   g i   k
```

#### b) Hapus Node `j`:
```
      h
     / \
    e   l
   / \  / \
  b   f k   m
 / \   \  /
a   d   g i
```

#### c) Hapus Node `h`:
```
      i
     / \
    e   l
   / \  / \
  b   f j   m
 / \   \    \
a   c   g    k
      \     
       d
```

### Nomor 4
Mengacu BST pada soal nomor 3 (sebelum penghapusan node), lakukan traversal dengan preorder.

#### Traversal preorder:
```
h, e, b, a, c, f, d, g, l, j, i, k, m
```
### Nomor 5
![image](https://github.com/NaufanZaki/Kunci-Jawaban-EAS-Strukdat/assets/111356493/0afa9039-c1e5-4a4a-86dd-837abddbc989)
![image](https://github.com/NaufanZaki/Kunci-Jawaban-EAS-Strukdat/assets/111356493/67ede16c-c7e5-483f-81db-c8ef742d0adb)

### Soal Nomor 6
#### Adjacency List dan Bobot (Jarak):
- Tenggarong <-> Bontang (140 km)
- Tenggarong <-> Samarinda (35 km)
- Tenggarong <-> IKN (150 km)
- Bontang <-> Samarinda (115 km)
- Samarinda <-> IKN (125 km)
- Samarinda <-> Balikpapan (110 km)
- IKN <-> Balikpapan (90 km)

#### Langkah-langkah menggunakan Algoritma Kruskal:
1. Urutkan semua edge berdasarkan bobot (jarak).
2. Pilih edge dengan bobot terendah, dan tambahkan ke MST jika tidak membentuk siklus.
3. Ulangi langkah 2 hingga semua node terhubung.

#### Penerapan Algoritma Kruskal:
1. Urutkan edges:
   - Tenggarong <-> Samarinda (35 km)
   - IKN <-> Balikpapan (90 km)
   - Samarinda <-> Balikpapan (110 km)
   - Bontang <-> Samarinda (115 km)
   - Samarinda <-> IKN (125 km)
   - Tenggarong <-> Bontang (140 km)
   - Tenggarong <-> IKN (150 km)

2. Pilih edges dan tambahkan ke MST jika tidak membentuk siklus:
   - Tenggarong <-> Samarinda (35 km)
   - IKN <-> Balikpapan (90 km)
   - Samarinda <-> Balikpapan (110 km)
   - Bontang <-> Samarinda (115 km)
   - Tenggarong <-> Bontang (140 km)

   **MST yang terbentuk:**
   ```
   Tenggarong <-> Samarinda (35 km)
   IKN <-> Balikpapan (90 km)
   Samarinda <-> Balikpapan (110 km)
   Bontang <-> Samarinda (115 km)
   ```
#### Langkah-langkah menggunaka Algoritma Prim
1. Mulai dari node acak, misalnya "Tenggarong".
2. Pilih edge dengan bobot terendah yang menghubungkan node yang sudah dikunjungi dengan node yang belum dikunjungi.
3. Tambahkan node tersebut ke dalam MST.
4. Ulangi langkah 2 dan 3 sampai semua node sudah dikunjungi.

#### Penerapan Algoritma Prim:
1. Mulai dari **Tenggarong**.
   - Pilih edge dengan bobot terendah: Tenggarong <-> Samarinda (35 km)
   - MST: Tenggarong <-> Samarinda (35 km)
   
2. Dari **Samarinda**, pilih edge dengan bobot terendah:
   - Pilih edge dengan bobot terendah: Samarinda <-> Balikpapan (110 km)
   - MST: Tenggarong <-> Samarinda (35 km), Samarinda <-> Balikpapan (110 km)
   
3. Dari **Balikpapan**, pilih edge dengan bobot terendah:
   - Pilih edge dengan bobot terendah: IKN <-> Balikpapan (90 km)
   - MST: Tenggarong <-> Samarinda (35 km), Samarinda <-> Balikpapan (110 km), IKN <-> Balikpapan (90 km)
   
4. Dari **IKN**, pilih edge dengan bobot terendah:
   - Pilih edge dengan bobot terendah: Samarinda <-> IKN (125 km)
   - MST: Tenggarong <-> Samarinda (35 km), Samarinda <-> Balikpapan (110 km), IKN <-> Balikpapan (90 km), Samarinda <-> IKN (125 km)
   
5. Dari **Samarinda**, pilih edge dengan bobot terendah:
   - Pilih edge dengan bobot terendah: Bontang <-> Samarinda (115 km)
   - MST: Tenggarong <-> Samarinda (35 km), Samarinda <-> Balikpapan (110 km), IKN <-> Balikpapan (90 km), Samarinda <-> IKN (125 km), Bontang <-> Samarinda (115 km)

Setelah semua node terhubung, MST yang terbentuk adalah:
```
Tenggarong <-> Samarinda (35 km)
IKN <-> Balikpapan (90 km)
Samarinda <-> Balikpapan (110 km)
Bontang <-> Samarinda (115 km)
Samarinda <-> IKN (125 km)
```
### Soal Nomor 7
Tunjukkan tahapan proses pengurutan data / sorting dengan:
- **(a) Quicksort**
- **(b) Insertionsort**

#### Deretan data yang akan diurutkan:
3, 7, 8, 5, 2, 1, 9, 5, 4

#### (a) Quicksort:
1. Pilih pivot (misal pivot = 4)
2. Partisi data menjadi dua bagian, yang lebih kecil dari pivot di kiri dan yang lebih besar di kanan.
   ```
   [3, 2, 1] 4 [7, 8, 5, 9, 5]
   ```
3. Rekursif pada bagian kiri dan kanan:
   - Kiri: [3, 2, 1]
     - Pivot = 1
     - [ ] 1 [3, 2]
     - Rekursif pada [3, 2]
       - Pivot = 2
       - [ ] 2 [3]
       - Rekursif pada [3]
   - Kanan: [7, 8, 5, 9, 5]
     - Pivot = 5
     - [5] 5 [7, 8, 9]
     - Rekursif pada [7, 8, 9]
       - Pivot = 8
       - [7] 8 [9]
       - Rekursif pada [7] dan [9]

Hasil akhir:
```
[1, 2, 3, 4, 5, 5, 7, 8, 9]
```

#### (b) Insertionsort:
1. Ambil elemen kedua dan bandingkan dengan elemen pertama, tukar jika perlu.
   ```
   [3, 7, 8, 5, 2, 1, 9, 5, 4]
   ```
2. Ambil elemen ketiga dan bandingkan dengan elemen sebelumnya, sisipkan di tempat yang sesuai.
   ```
   [3, 7, 8, 5, 2, 1, 9, 5, 4]
   ```
3. Ambil elemen keempat dan bandingkan dengan elemen sebelumnya, sisipkan di tempat yang sesuai.
   ```
   [3, 5, 7, 8, 2, 1, 9, 5, 4]
   ```
4. Lanjutkan hingga elemen terakhir.
   ```
   [2, 3, 5, 7, 8, 1, 9, 5, 4]
   [1, 2, 3, 5, 7, 8, 9, 5, 4]
   [1, 2, 3, 5, 5, 7, 8, 9, 4]
   [1, 2, 3, 4, 5, 5, 7, 8, 9]
   ```

Hasil akhir:
```
[1, 2, 3, 4, 5, 5, 7, 8, 9]
```
