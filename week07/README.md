l![Image Banner!](assets/react-lanjutan-banner.png "Javascript")
# **React js Lanjutan**
## React Context

### Apa itu Reat context ?
> React Context dirancang untuk berbagi data atau variable global untuk pohon komponen React, seperti pengguna yang diautentikasi saat ini, tema, atau bahasa pilihan

### Bagaimana menggunakan React Context ?
1. Buat Sebuah Folder context di dalam folder src dan di dalam folder tersebut terdapat file dengan nama **AppContext.jsx**

    ```
    // 1. Import React Library
    import React from "react"

    // 2. Definisikan variable dengan assign value React.createContext()
    export const AppContext = React.createContext()
    Lalu beralih ke <App.js> dan jangan lupa ,mengimport Home dan file-file yg kita butuhkan.
    ```

2. Buat sebuah folder **components** dan di dalamnya ada folder navbar lalu di dalam folder navbar ada file **<Navbar.jsx>**


---
## React Testing

### Apa itu React Testing ?
> Dalam jargon tech, Testing adalah mengecek apakah code kita sudah memenuhi harapan atau belum

### Tipe Testing
- manual testing
  dilakukan oleh developer secara manual, seperti me runnin react atau juga console.log
- automation testing
 dilakukan secara otomatis oleh code yang dibuat oleh developer

### 3 Kategori Testing
- unit tes
    melakukan pengujian pada bagian yang paling kecil
- integration
    melakukan pengujian saling terhubung ke aplikasi yg lain, contoh terhubung ke database
- End to end
    melakukan testing dari sisi user/pengguna

### Apa itu Jest?
> Jest adalah sebuah library JavaScript untuk pengetesan (membuat, menjalankan, dan menyusun pengujian)

### Alur testing 
1. Import fungsi untuk diuji
2. Berikan input ke fungsi tersebut
3. Tentukan apa yang diharapkan sebagai output
4. Periksa apakah fungs menghasilkan output yang diharapkan.

### jest documentations
https://jestjs.io/

### install dependcy jest
https://jestjs.io/docs/getting-started

### react testing library
https://testing-library.com/docs/react-testing-library/intro/
