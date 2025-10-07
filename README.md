# lab3web
# Praktikum 3 — Membuat Form Data Diri dengan HTML dan CSS
# Nama : Arya Zhalna Nugraha
# Kelas : Ti.24.A.3
# Matkul : Pemrograman web
##  Tujuan
Membuat sebuah **form data diri** menggunakan elemen-elemen HTML seperti `<form>`, `<input>`, `<textarea>`, `<select>`, `<option>`, dan `<fieldset>` serta menerapkan **CSS** untuk memperindah tampilan.

---

##  Langkah-Langkah Praktikum

### 1. Membuat Struktur Dasar HTML
Buka teks editor seperti **VS Code** dan buat file baru dengan nama:  
`lab3web.html`

Tambahkan struktur HTML dasar berikut:
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Form Data Diri</title>
</head>
<body>
  <h1>FORM DATA DIRI</h1>
</body>
</html>
```
<img width="678" height="124" alt="Screenshot (221)" src="https://github.com/user-attachments/assets/8bf0f15b-111f-4bb1-9dfa-25618e059d0d" />


---

### 2. Menambahkan Elemen Form
Gunakan tag `<form>` dan `<fieldset>` untuk membungkus data pelanggan.
```html
<form>
  <fieldset>
    <legend>Data Diri</legend>

    <label>Nama :</label>
    <input type="text" name="nama"><br>

    <label>Alamat :</label>
    <textarea name="alamat"></textarea><br>

    <label>Jenis Kelamin :</label>
    <input type="radio" name="jk" value="Laki-laki">Laki-laki
    <input type="radio" name="jk" value="Perempuan">Perempuan<br>

    <label>Kota :</label>
    <select name="kota">
      <option>-- Pilih Kota --</option>
      <option>Jakarta</option>
      <option>Bandung</option>
      <option>Surabaya</option>
      <option>Yogyakarta</option>
    </select><br>

    <label>Hobi :</label>
    <select name="hobi" multiple>
      <option>Musik</option>
      <option>Olahraga</option>
      <option>Traveling</option>
      <option>Menulis</option>
    </select><br>

    <input type="submit" value="Login">
  </fieldset>
</form>
```
<img width="669" height="665" alt="Screenshot (222)" src="https://github.com/user-attachments/assets/2162681c-7ff9-426f-b8f7-a84726298cec" />

---

### 3. Menambahkan CSS untuk Tampilan
Tambahkan elemen `<style>` di dalam `<head>` agar tampilan lebih menarik:
```html
<style>
  body {
    background-color: lightblue;
    font-family: Arial, sans-serif;
  }

  h1 {
    text-align: center;
    text-decoration: underline;
  }

  fieldset {
    width: 400px;
    margin: auto;
    border: 2px solid blue;
    background-color: #e8f4ff;
  }

  legend {
    color: red;
    font-weight: bold;
  }

  label {
    display: inline-block;
    width: 120px;
  }

  input[type="text"], textarea, select {
    border: 1px solid green;
  }

  input[type="submit"] {
    background-color: green;
    color: white;
    border: none;
    padding: 6px 15px;
    border-radius: 4px;
  }

  input[type="submit"]:hover {
    background-color: darkgreen;
  }
</style>
```

---

### 4. Menjalankan Program di Browser
Buka file `lab3web.html` di browser (Chrome/Edge) → tampil form seperti berikut:

 *Hasil Akhir:*  
![Hasil Akhir]
<img width="711" height="813" alt="Screenshot (220)" src="https://github.com/user-attachments/assets/aeef582d-200f-4b64-8be6-7e87448ad632" />


---

##  Penjelasan Elemen yang Digunakan

| Tag | Fungsi |
|-----|---------|
| `<form>` | Pembungkus semua elemen input |
| `<fieldset>` | Memberi batas visual dan kelompok data |
| `<legend>` | Judul untuk fieldset |
| `<label>` | Label teks untuk tiap input |
| `<input type="text">` | Kolom input teks untuk nama |
| `<textarea>` | Input teks panjang untuk alamat |
| `<input type="radio">` | Pilihan jenis kelamin |
| `<select>` | Dropdown list untuk kota |
| `<select multiple>` | Listbox untuk memilih beberapa hobi |
| `<input type="submit">` | Tombol untuk mengirim form |

---

##  Kesimpulan
Dari praktikum ini, kita telah mempelajari cara membuat form data diri yang interaktif dengan HTML dan mempercantik tampilannya menggunakan CSS. Form ini bisa dikembangkan menjadi form pendaftaran, login, atau input data pelanggan.

---

##  Daftar Screenshot
- Screenshot219.png → Tampilan akhir form data diri
