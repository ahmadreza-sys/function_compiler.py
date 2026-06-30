# 🖥️ Proyek Akhir Teknik Kompilasi

## Representasi Tahapan Kompilasi Menggunakan Deklarasi Fungsi

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Status](https://img.shields.io/badge/Status-Selesai-brightgreen)
![License](https://img.shields.io/badge/License-MIT-green)

---

### Nama
Ahmad Reza

### NIM
(231011403385)

### Mata Kuliah
Teknik Kompilasi

---

# Deskripsi

Proyek ini merupakan simulasi sederhana proses kompilasi menggunakan bahasa Python.

Konstruksi yang dipilih adalah **Deklarasi Fungsi (Function Declaration)**.

Program mensimulasikan empat tahapan utama compiler, yaitu:

- Lexical Analysis
- Syntax Analysis (AST)
- Semantic Analysis
- Three Address Code (TAC)

---

# Source Code

```c
int tambah(int a, int b){
    return a + b;
}
```

---

# Grammar (BNF)

```text
<function> ::= <type> <identifier> "(" <parameter_list> ")" "{" <return_stmt> "}"

<parameter_list> ::= <parameter> | <parameter> "," <parameter_list>

<parameter> ::= <type> <identifier>

<return_stmt> ::= "return" <expression> ";"

<expression> ::= <identifier> "+" <identifier>

<type> ::= "int" | "float" | "char"
```

---

# Tahapan Kompilasi

## 1. Lexical Analysis

Source code dipecah menjadi token seperti keyword, identifier, dan symbol.

## 2. Syntax Analysis

Parser membentuk Abstract Syntax Tree (AST).

## 3. Semantic Analysis

Memastikan tipe data dan parameter valid.

## 4. Three Address Code

Menghasilkan intermediate code berupa TAC.

---


# Contoh Output

## Semantic Analysis

```
Semantic Analysis Berhasil
```

## Three Address Code

```
BeginFunc tambah

t1 = a + b

return t1

EndFunc
```

---
