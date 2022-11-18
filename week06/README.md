l![Image Banner!](assets/react-lanjutan-banner.png "Javascript")
# **React js Lanjutan**
## Prop Types
> merupakan sebuah library yang dapat membantu kita untuk memeriksa data props yang kita kirim sudah sesuai ekpektasi atau belum. akan muncul eror jika tidak sesuai

### Bagaimana cara install PropTypes
```
npm install prop-types
```

### Bagaimana cara penggunaan Props Types ?
```
import PropTypes from 'prop-types'

function Card(props) {
    return (
        <>
            <h2>name: {props.char}</h2>
            <p>age: {props.age}</p>
        </>
    )
}

Card.PropTypes = {
    char: PropTypes.string,
    age: PropTypes.number
}
```
> Props yang dikirim harus sesuai dengan tipe data yg diinginkan

## React Router
### Apa itu React Router ?
> Dalam web jika ingin berganti halaman satu dan halaman yang lainnya diperlukan suatu proses routing. Routing sendiri adalah proses pemetaan antara sebuah URL ke dalam sebuah halaman yang terdapat konten / UI (User Interface) sesuai dengan URL yang dituju

### Bagaimana Cara Install React Router ?
-  pastikan sudah ada di dalam folder project(react app)
    ```
    npm install react-router-dom@6
    ```

- import di main.jsx
  ```
  import { BrowserRouter } from "react-router-dom";
  ```

- bungkus,component `<app />` dengan BrowserRouter
  ```
   <BrowserRouter>
    <App />
  </BrowserRouter>,
  ```
  
- import di app.jsx
  ```
  import { Routes, Route, Link } from "react-router-dom";
  ```

- playing code in return
  ```
  <>
  <Routes>
  ...<your code> ...
  </Routes>
  </>
  ```

### Bagaimana cara membuat page ?
- buat folder **page** di dalam folder **src**
- lalu buat page, contoh **HomePage.jsx**

### Menghubungkan page
- dalam file **App.jsx**, 

    ```
    <routes>
        <route path='/' element={<HomePage />} />
        <route path='about' element={<AboutPage />} />
    </routes>
    ```

### Cara Berpindah page
> Example :
  ```
  <link to='/'>Home</link>
  <link to='AboutPage>About</link>
  ```

### Noted 
- **path='/'** gunakan untuk menampilkan halaman utama(home)
- letakan nav diatas ``<route>`` jika ingin ditampilkan pada setiap page

### Dokumentasi React Router v.6.30
https://reactrouter.com/en/v6.3.0/getting-started/installation

### Params
> param adalah parameter, digunakan untuk membawa data saat perpindah page

- useNavigate 
  > useNaviage untuk berpindah page sambil membawa data

  ```
  import { useNavigate } from 'react-router-dom'
  ```

- useParams
  > UseParams untuk menangkap data yang dibawa saat berpindah 
  ```
  import { useParams } from 'react-router-dom'
  ```

- noted
   - tambahkan '+' number === +id ( id, akan menjadi number, hasilnya true)


### Nested Route
> adalah page di dalam page

> pada path children tidak perlu di menggunakan parent page dan tanda '/' lagi

   - example:
```
<route path='/about' element={<AboutPage />}>
	<route path='student' element={<AboutStudent />}>
	<route path='teacher' element={<AboutTeacher />}>
</route>
```

- outlet
  > untuk memanggil children page gunakan outlet (dalam parent)

  - import pada parent page
  ```
  import {outlet} from 'react-router-dom';
  ```

  - masukan komponen Outlet di dalam return parent page untuk memanggil nested element
    ```
    <Outlet />
    ```

  - ndex element
  element utama yang pertama kali di tampilkan
  
    ```
    <route index element={<AboutSchool />} />
    ```

---

## React Redux

### Apa itu Redux ?
> Redux adalah State management yang terdapat pada React 

### Apa itu State management ?
> State management adalah suatu management data yang akan membuat data menjadi terpusat sehingga kompenen yang membutuhkan data tersebut dapat langsung mengambil datanya

### Macam-macam State management :
- Redux
- Context
- Jotai
- Zustand

### Analogi :
- Redux == Gudang
- Reducer == Rak/Etalase
- Provider == gerbang yg menyatakan bahwa data tersedia untuk di akses oleh kompenen tersebut

### Cara Install Redux 
1. Install package Redux
    ``` 
    npm install redux react-redux 
    ```
2. buat store (tempat untuk menjadi gudang penyimpanan data)
    - setup store
