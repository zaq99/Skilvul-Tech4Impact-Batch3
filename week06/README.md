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
