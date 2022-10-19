# [Bookself API]

> Proyek Akhir Pelatihan **_"Belajar Membuat Aplikasi Back-End untuk Pemula"_**

## 📑 Persiapan Proyek

1.  Membuat file package.json
    - `npm init --y`
2.  Install Framework NodeJS HAPI
    - 'Note:' hapi: framework yang digunakan untuk membuat sebuah RESTful API
    - `npm install @hapi/hapi`
3.  Install package nodemon
    - `Note:` nodemon: package untuk restart otomatis aplikasi yang sedang dijalankan.
    - `npm install nodemon --save-dev`
4.  Install package eslint

    - `Note:` eslint: package untuk memperbaiki kualtias kode.
    - `npm install eslint --save-dev`

    - `Note kode dibawah:` Digunakan untuk membuat file.eslintrc.json.
    - `npx eslint --init`

5.  Membuat Struktur Proyek

- src `folder`
  -- books.js
  -- handler.js
  -- routes.js
  -- server.js

6. Install package nanoid
   - `Note:` nanoid: package untuk membuat sebuah unique ID secara otomatis.
   - `npm install nanoid@3.3.4`

# 📝 TODO LIST

#### Kriteria 1 : API dapat menyimpan buku

- ✅ Client tidak melampirkan properti namepada request body
- ✅ Client melampirkan nilai properti readPage yang lebih besar dari nilai properti pageCount
- ✅ Server gagal memasukkan buku karena alasan umum (generic error)
- ✅ Bila buku berhasil dimasukkan

#### 📄 Kriteria 2 : API dapat menampilkan seluruh buku

- ✅ API yang Anda buat harus dapat menampilkan seluruh buku yang disimpan melalui route
- ✅ Server harus mengembalikan respons
- ✅ Jika belum terdapat buku yang dimasukkan, server bisa merespons dengan array books kosong

#### 📄 Kriteria 3 : API dapat menampilkan detail buku

- ✅ API yang Anda buat harus dapat menampilkan seluruh buku yang disimpan melalui route
- ✅ Bila buku dengan id yang dilampirkan oleh client tidak ditemukan
- ✅ Bila buku dengan id yang dilampirkan ditemukan

#### 📄 Kriteria 4 : API dapat mengubah data buku

- ✅ API yang Anda buat harus dapat mengubah data buku berdasarkan id melalui route
- ✅ Client tidak melampirkan properti name pada request body
- ✅ Client melampirkan nilai properti readPage yang lebih besar dari nilai properti pageCount
- ✅ Id yang dilampirkan oleh client tidak ditemukkan oleh server
- ✅ Bila buku berhasil diperbarui

#### 📄 Kriteria 5 : API dapat menghapus buku

- ✅ API yang Anda buat harus dapat menghapus buku berdasarkan id melalui route
- ✅ Bila id yang dilampirkan tidak dimiliki oleh buku manapun
- ✅ Bila id dimiliki oleh salah satu buku

#### 📮 POSTMAN Test Kriteria 1

- ✅ [Mandatory] Add Book With Complete Data
- ✅ [Mandatory] Add Book Without Name
- ✅ [Mandatory] Add Book with Page Read More Than Page Count

#### 📮 POSTMAN Test Kriteria 2

- ✅ [Mandatory] Get All Books

#### 📮 POSTMAN Test Kriteria 3

- ✅ [Mandatory] Get Detail Books With Correct Id
- ✅ [Mandatory] Get Detail Books With Invalid Id

#### 📮 POSTMAN Test Kriteria 4

- ✅ [Mandatory] Update Book With Complete Data
- ✅ [Mandatory] Update Book Without Name
- ✅ [Mandatory] Update Book With Page Read More Than Page Count
- ✅ [Mandatory] Update Book with Invalid Id

#### 📮 POSTMAN Test Kriteria 5

- ✅ [Mandatory] Delete Book with Correct Id
- ✅ [Mandatory] Delete Book with Invalid Id

#### 📮 POSTMAN Test Ops-1

- ✅ Add Reading and Finished Book
- ✅ Add Reading and Unfinished Book with "Dicoding" Name
- ✅ Add Unreading Books and Unfinished Book "Dicoding" Name
- ✅ Add Unreading Books and Unfinished Book

#### 📮 POSTMAN Test Ops-2

- ✅ [Optional] Get All Reading Books
- ✅ [Optional] Get All Unreading Books
- ✅ [Optional] Get All Finished Books
- ✅ [Optional] Get All Unfinished Books
- ✅ [Optional] Get All Books Contains "Dicoding" Name
