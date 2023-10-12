<table>
  <tr>
    <th colspan="2">DATA MAHASISWA</th>
  </tr>
  <tr>
    <td>Nama</td>
    <td>Aas Novitasari</td>
  </tr>
  <tr>
    <td>NIM</td>
    <td>312210167</td>
  </tr>
  <tr>
    <td>Kelas</td>
    <td>TI.22.A1</td>
  </tr>
</table>

## **Daftar Isi** ##

**1. [Instruksi Praktikum](#instruksi-praktikum)**  
**2. [Langkah-langkah Praktikum](#langkah-langkah-praktikum)**  
**3. [Pertanyaan dan Tugas](#pertanyaan-dan-tugas)**

## **Instruksi Praktikum**

1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama Lab3Web
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

## **Langkah-langkah Praktikum**
**1. Membuat Ordered List & Unordered List**

```<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
    <link rel="stylesheet" href="css/style.css">
</head>

<body>
    <nav>
        <a href="lab3_list.html">List HTML</a>
        <a href="lab3_tabel.html">Tabel HTML</a>
        <a href="lab3_form.html">Form HTML</a>
        <a href="lab3_tugas.html">Form Dropdown & Listbox</a>
    </nav>

    <header>
        <h1>Membuat List</h1>
    </header>

    <section id="order-list">
        <h2>Ordered List</h2>
        <ol>
            <li>Pemrograman Web</li>
            <li>Sistem Informasi</li>
            <li>Basis Data 2</li>
        </ol>
    </section>

</body>

</html>
```
### Hasil Run Ordered List
![1](https://github.com/aasnovita114/Lab3_web/assets/116045324/f8d55a47-b2b8-4c37-93b1-19a706420b7b)

```html
<section id="unorder-list">
  <h2>Unordered List</h2>
  <ul type="square">
    <li>Jaringan Komputer</li>
    <li>Struktur Data</li>
    <li>Algoritma &amp; Pemrograman</li>
  </ul>
</section>
```
### Hasil Run Unordered List

![image](https://github.com/aasnovita114/Lab3_web/assets/116045324/099515b5-5158-4f71-ac3e-c9f79ce8193d)

**2. Membuat Description List**
```html
<section id="unorder-list">
  <h2>Description List</h2>
  <dl>
    <dt>Fakultas Teknik</dt>
    <dd>Teknik Industri</dd>
    <dd>Teknik Informatika</dd>
    <dd>Teknik Lingkungan</dd>
    <dt>Fakultas Ekonomi dan Bisnis</dt>
    <dd>Akuntansi</dd>
    <dd>Manajemen</dd>
    <dd>Bisnis Digital</dd>
  </dl>
</section>
```
### Hasil Run  Description List
![image](https://github.com/aasnovita114/Lab3_web/assets/116045324/aa138d67-8ece-49ac-9526-9347ffd5b383)

**3. Membuat Tabel**

```html
<table border="1" cellpadding="4" cellspacing="0">
  <thead>
    <tr>
      <th>No.</th>
      <th>Fakultas</th>
      <th>Program Studi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td>Teknik</td>
      <td>Teknik Informatika</td>
    </tr>
    <tr>
      <td>2.</td>
      <td>Teknik</td>
      <td>Teknik Industri</td>
    </tr>
    <tr>
      <td>3.</td>
      <td>Teknik</td>
      <td>Teknik Lingkungan</td>
    </tr>
  </tbody>
</table>
```
### Hasil Run Membuat Table
![image](https://github.com/aasnovita114/Lab3_web/assets/116045324/2bcb5159-cc2f-4b5e-9d61-85fb2e22e48b)

**4. Mengatur Margin dan Padding**

```html
<table border="1" cellpadding="4" cellspacing="0"></table>
```

### Hasil Run Mengatur Margin dan Padding
![image](https://github.com/aasnovita114/Lab3_web/assets/116045324/a2b22023-c794-47c7-834e-a47f5167477e)


**5. Menggabungkan Sel Data**

```html
<tr>
  <td>1.</td>
  <td rowspan="3">Teknik</td>
  <td>Teknik Informatika</td>
</tr>
```
### Hasil Run Menggabungkan Sel data
![image](https://github.com/aasnovita114/Lab3_web/assets/116045324/a423d619-edda-4d16-b8a8-3288a531b134)

**6. Membuat Form**

```html
<form action="proses.php" method="post">
  <fieldset>
    <legend>Data Pelanggan</legend>
    <p>
      <label for="nama">Nama</label>
      <input type="text" id="nama" name="nama" />
    </p>
    <p>
      <label for="alamat">Alamat</label>
      <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
    </p>
    <p>
      <label>Jenis Kelamin</label>
      <input id="jk_l" type="radio" name="kelamin" value="L" /><label for="jk_l"
        >Laki-laki</label
      >
      <input id="jk_p" type="radio" name="kelamin" value="P" /><label
        qafor="jk_p"
        >Perempuan</label
      >
    </p>
    <p><input type="submit" value="Login" /></p>
  </fieldset>
</form>
```
### Hasil Run Membuat From
![image](https://github.com/aasnovita114/Lab3_web/assets/116045324/2b2642aa-80e3-4801-854d-69dd208e55c8)

**7. Menabahkan Style**

```
body {
  font-family: Tahoma;
}

h1 {
  margin-top: 50px;
  text-align: center;
  color: darkcyan;
}

.tabel {
  margin: 20px auto;
}

form p > label {
  display: inline-block;
  width: 100px;
}

form input[type="text"],
form textarea {
  border: 1px solid #197a43;
}

form input[type="submit"] {
  border: 1px solid #197a43;
  background-color: #197a43;
  color: #ffffff;
  font-weight: bold;
  padding: 5px 15px;
  border-radius: 10px;
}

form input[type="submit"]:hover {
  background-color: #3d9a38;
  cursor: pointer;
}

nav {
  background-color: #4dacd1c5;
  padding: 10px;
  position: fixed;
  top: 0px;
  right: 0px;
  left: 0px;
  text-align: center;
}

nav a {
  color: #fff;
  text-decoration: none;
  padding: 2px 4px;
  font-size: 13px;
}

nav a:hover {
  color: #3399c2;
}

nav a:active {
  color: #7da8b9;
}

/* Style untuk form dropdown & listbox */
.form_tugas {
  max-width: 400px;
  margin: 0 auto;
  padding: 20px;
  border: 1px solid #ccc;
  background-color: #f9f9f9;
  border-radius: 5px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

/* Style untuk label */
.form_tugas label {
  display: block;
  font-weight: bold;
  margin-bottom: 5px;
}

/* Style untuk select dropdown dan listbox */
.form_tugas select {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  border: 1px solid #ccc;
  border-radius: 3px;
}

/* Style untuk tombol Submit */
.form_tugas #input_tugas {
  background-color: #007bff;
  color: #fff;
  padding: 5px 15px;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

.form_tugas #input_tugas:hover {
  background-color: #4dacd1;
}
```

### Hasil Run Menambahkan Style
![image](https://github.com/aasnovita114/Lab3_web/assets/116045324/3965ac5f-aeec-4f7b-a128-eed0b22e2f54)

## **Pertanyaan dan Tugas** ##

1. Buatlah form yang menampilkan **dropdown** menu dan **listbox**dengan _multiple selection_.

   ```html
    <form class="form_tugas">
        <label for="dropdown">Pilih salah satu buah:</label>
        <select name="dropdown" id="dropdown">
            <option value="apel">Apel</option>
            <option value="jeruk">Jeruk</option>
            <option value="durian">Durian</option>
            <option value="mangga">Mangga</option>
            <option value="semangak">Semangka</option>
        </select>

        <br><br>

        <label for="listbox">Pilih beberapa buah:</label>
        <select name="buah[]" multiple id="listbox">
            <option value="apel">Apel</option>
            <option value="jeruk">Jeruk</option>
            <option value="durian">Durian</option>
            <option value="mangga">Mangga</option>
            <option value="semangka">Semangka</option>
            <option value="kelapa">Kelapa</option>
            <option value="anggur">Anggur</option>
            <option value="melon">Melon</option>
            <option value="pepaya">Pepaya</option>
            <option value="nanas">Nanas</option>
        </select>

        <br>

        <input type="submit" value="Submit" id="input_tugas">
    </form>
     </fieldset>
   </form>
   ```
   ![image](https://github.com/aasnovita114/Lab3_web/assets/116045324/1389d668-e406-4d25-91aa-c04a96ee9ee2)

## Terimakasih

   




