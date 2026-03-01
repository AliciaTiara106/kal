# contoh penyelesaian

contoh penyelesaian sistem persamaan linear 4 variabel menggunakan metode eliminasi gaussian


```s
# 1. Definisi Matriks Augmentasi
B4 = matrix(QQ, [[1, 1, 1, 1, 10],
                 [1, -1, 2, 1, 8],
                 [2, 1, -1, 2, 11],
                 [1, 2, 1, -1, 6]])

print("Matriks 4 Variabel (M0):")
show(B4)

# 2. Langkah OBE Strategis
M1 = B4.with_added_multiple_of_row(1, 0, -1)
M2 = M1.with_added_multiple_of_row(2, 0, -2)
M3 = M2.with_added_multiple_of_row(3, 0, -1)

# Menghaluskan Baris 2 (Pivot)
M4 = M3.with_rescaled_row(1, -1/2)

# Eliminasi di bawah Pivot baris 2
M5 = M4.with_added_multiple_of_row(2, 1, 1)
M6 = M5.with_added_multiple_of_row(3, 1, -1)

print("Proses OBE sedang berjalan...")
show(M6)

# Hasil Akhir Otomatis
print("Hasil Akhir Bentuk Eselon:")
show(B4.echelon_form())
```

### Matriks Awal
$$
\begin{pmatrix}
1 & 1 & 1 & 1 & 10 \\
1 & -1 & 2 & 1 & 8 \\
2 & 1 & -1 & 2 & 11 \\
1 & 2 & 1 & -1 & 6
\end{pmatrix}
$$
---

### Proses OBE (Sedang Berjalan)

$$
\begin{pmatrix}
1 & 1 & 1 & 1 & 10 \\
0 & 1 & -\frac{1}{2} & 0 & 1 \\
0 & 0 & -\frac{7}{2} & 0 & -8 \\
0 & 0 & \frac{1}{2} & -2 & -5
\end{pmatrix}
$$

---

### Matriks 4 Variabel (M0)  
**Hasil Akhir Bentuk Eselon:**

$$
\begin{pmatrix}
1 & 0 & 0 & 0 & \frac{5}{2} \\
0 & 1 & 0 & 0 & \frac{15}{7} \\
0 & 0 & 1 & 0 & \frac{16}{7} \\
0 & 0 & 0 & 1 & -\frac{43}{14}
\end{pmatrix}
$$


contoh penyelesaian sistem persamaan linear 3 variabel menggunakan metode eliminasi gaussian

```s
B3 = matrix(QQ, [[1, 2, 1, 6],
                 [1, 3, 2, 9],
                 [2, 1, 2, 12]])

print("Matriks Awal (M0):")
show(B3)


M1 = B3.with_added_multiple_of_row(1, 0, -1)   # Baris 2 = B2 - B1
M2 = M1.with_added_multiple_of_row(2, 0, -2)   # Baris 3 = B3 - 2*B1
M3 = M2.with_added_multiple_of_row(2, 1, 3)    # Baris 3 = B3 + 3*B2
M4 = M3.with_rescaled_row(2, 1/3)              # Membuat pivot terakhir menjadi 1

print("Matriks Eselon Baris (Eselon):")
show(M4)

# 3. Solusi Akhir (Reduced Row Echelon Form)
print("Solusi Akhir (RREF):")
show(M4.echelon_form())
```
### Matriks Awal (M0)

$$
\begin{pmatrix}
1 & 2 & 1 & 6 \\
1 & 3 & 2 & 9 \\
2 & 1 & 2 & 12
\end{pmatrix}
$$

---

### Matriks Eselon Baris (Eselon)

$$
\begin{pmatrix}
1 & 2 & 1 & 6 \\
0 & 1 & 1 & 3 \\
0 & 0 & 1 & 3
\end{pmatrix}
$$

---

### Solusi Akhir (RREF)

$$
\begin{pmatrix}
1 & 0 & 0 & 3 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 3
\end{pmatrix}
$$

