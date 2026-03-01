# MATERI KAL

**Definisi 1.1.1. Persamaan Linear.**

*Sebuah ekspresi linear* dalam *n* perubah yang tidak diketahui (atau variabel) $x_1, x_2, \ldots, x_n$ adalah suatu bentuk yang dinyatakan sebagai

$$
a_{1}x_{1} + a_{2}x_{2} + \cdots + a_{n}x_{n},
$$

di mana $a_1, a_2, \ldots, a_n$ adalah bilangan real konstan.

Sebuah *persamaan linear* dalam peubah yang tidak diketahui $x_1, x_2, \ldots, x_n$ adalah persamaan yang dapat disederhanakan, hanya dengan menggunakan operasi penjumlahan dan pengurangan, menjadi bentuk

$$
a_{1}x_{1} + a_{2}x_{2} + \cdots + a_{n}x_{n} = b,
$$

(1.1.1)

yang disebut sebagai *bentuk standar*. Suatu persamaan dalam variabel tak diketahui $x_1, x_2, \ldots, x_n$ disebut *nonlinear* jika tidak dapat disederhanakan ke bentuk (1.1.1) hanya dengan menggunakan penjumlahan dan pengurangan.

Diberikan sebuah persamaan linear dengan bentuk standar (1.1.1), persamaan tersebut disebut *homogen* jika \( b = 0 \), dan *nonhomogen* jika $b \ne 0$.




### Definisi 1.1.3. Sistem persamaan linier

Sistem **persamaan linier** (atau **sistem linier**) adalah sekumpulan persamaan linier.

Sistem linier **homogen** adalah sekumpulan persamaan linier homogen.

Saat menampilkan sistem *m* persamaan dalam *n* tidak diketahui $x_1, x_2, \ldots, x_n$,  
kami biasanya menulis setiap persamaan dalam bentuk standar dan menyelaraskan istilah  
yang sesuai dari setiap persamaan ke dalam kolom:

$$
a_{11}x_1 + a_{12}x_2 + \cdots + a_{1n}x_n &= b_1 \\
a_{21}x_1 + a_{22}x_2 + \cdots + a_{2n}x_n &= b_2 \\
\vdots \\
a_{m1}x_1 + a_{m2}x_2 + \cdots + a_{mn}x_n &= b_m
$$

Sistem homogen dengan demikian biasanya ditulis sebagai:

$$
a_{11}x_1 + a_{12}x_2 + \cdots + a_{1n}x_n &= 0 \\
a_{21}x_1 + a_{22}x_2 + \cdots + a_{2n}x_n &= 0 \\
\vdots \\
a_{m1}x_1 + a_{m2}x_2 + \cdots + a_{mn}x_n &= 0
$$

---

### Keterangan 1.1.4

Anda akan ingin merasa nyaman dengan pengindeksan ganda yang digunakan untuk menampilkan sistem linier secepat mungkin.  
Berikut adalah cara yang baik untuk mengarahkan diri Anda:

- Itu $i$ muncul di $a_{ij}$ dan $b_i$ menunjukkan $i$-th dalam sistem yang ditampilkan, atau setara, $i$-persamaan.
- Itu $j$ muncul di $a_{ij}$ menunjukkan $j$-th dalam sistem yang ditampilkan, yang terkait dengan kolom $j$-th, untuk $1 \le j \le n$.