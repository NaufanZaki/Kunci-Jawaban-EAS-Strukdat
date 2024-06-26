# Kunci-Jawaban-EAS-Strukdat
### Nomor 1
Gambarkan AVL-tree dari deretan nilai: k, m, u, t, v, p, x.

### Proses pembentukan AVL-tree:
1. Masukkan k (AVL tree hanya memiliki root k).
2. Masukkan m (k tetap root, m di sebelah kanan k).
3. Masukkan u (k tetap root, m di sebelah kanan k, u di sebelah kanan m).
4. Masukkan t (k tetap root, m di sebelah kanan k, u di sebelah kanan m, t di sebelah kiri u).
5. Masukkan v (k tetap root, m di sebelah kanan k, u di sebelah kanan m, t di sebelah kiri u, v di sebelah kanan u).
6. Masukkan p (k tetap root, m di sebelah kanan k, u di sebelah kanan m, t di sebelah kiri u, v di sebelah kanan u, p di sebelah kiri u).
7. Masukkan x (k tetap root, m di sebelah kanan k, u di sebelah kanan m, t di sebelah kiri u, v di sebelah kanan u, p di sebelah kiri u, x di sebelah kanan v).

#### AVL Tree final:
```
      k
       \
        m
         \
          u
         / \
        t   v
       /   / \
      p   x
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
   a   c w   z
          /   \
         v     y
        /       \
       e         f
```

### Nomor 3
Mengacu BST berikut ini, gambarkan perubahan tree-nya jika dilakukan penghapusan satu node berikut. Untuk masing-masing penghapusan berikut ini, proses dilakukan terhadap BST awal.

#### a) c
```
      h
     / \
    e   l
   / \   \
  b   f   j
 /       / \
a       i   k
```

#### b) j
```
      h
     / \
    e   l
   / \   \
  b   f   m
 /       / \
a       i   k
```

#### c) h
```
      i
     / \
    e   l
   / \   \
  b   f   j
 /       / \
a       g   k
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

Jika ada pertanyaan lebih lanjut atau penjelasan tambahan yang diperlukan, silakan tanyakan.
