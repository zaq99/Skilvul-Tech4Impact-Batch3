![Image Banner!](../assets/js-banner-DOM.png "Javascript")
# **DOM (Document Object Model)**
### Apa itu DOM ?
>  DOM berisi kumpulan aturan atau cara bagi programmer untuk memanipulasi apapun yang tampil dalam halaman web. DOM tidak terikat dengan JavaScript, dan juga bukan bagian dari JavaScript. DOM yang sama bisa diakses dengan bahasa client-side lain seperti JScript.

### Bagaimana Peran DOM pada WEB development ?
> DOM adalah jembatan agar bahasa pemrograman bisa berinteraksi dengan dokumen html

### Beberapa Syntax/method pada DOM :
1. Traversing/Akses Element
>- Kebawah
>   - ```getElementById()``` akses element menggunakan Id
>   - ```getElementsByTagName()``` akses element menggunakan Tag
>   - ```getElementsByClassName()``` akses element menggunakan class
>   - ```querySelector()``` aksess element menggunakan selector seperti css (tag, class, id)
>   - ```querySelectorAll()``` aksess element menggunakan selector lebih dari satu
>   - ```children()``` akses anak dari element
>- Keatas
>   - ```parentElement()``` akses ke parent element/pembungkus element
>   - ```closets()``` akes ke nenek moyang element/2x pembungkus element
>- Kesamping
>   - ```nextElementSibling()``` akes element yang sejajar setelahnya
>   - ```previousElentSibling()``` akses element yang sejajar sebelumnya

2. Manipulations Element
>- ```innerHTML``` untuk menambahkan tag html + string
>- ```innerText```  untuk menambahkan string/text
>- ```createElement()``` untuk membuat element baru
>- ```append()``` untuk memasukan element baru ke dokument html
>- ```appendChild()``` untuk memasukan element baru ke dokument html (tidak bisa memasukan string)
>- ```remove()``` untuk menghapus element
>- ```attributes``` untuk melihat attribute
>- ```getAttributes``` untuk mendapatkan attribute
>- ```setAttributes``` untuk mensetting attribute
3. Styling Element
>- ```style``` untuk memberikan style pada element
> ``` 
> h1.style.color = 'red'; 
> div.style.backgroundColor = '#fff';
> ```
>- ```getComputedStyle``` untuk mendapatkan styling pada element
>```
> let body = getComputedStyle(variable)
>```

### Bekerja dengan DOM
- Document HTML
```
<head>
    <meta charset="UTF-8">
    <title>Dom Selection</title>
    <script src="script.js" defer></script>
</head>

<body>

    <h1 id="judul">Hello World</h1>
    <div id="container">
        <section id="a">
            <p class="p1">paragraf 1</p>
            <p class="p2">paragraf 2</p>
            <p class="p3">paragraf 3</p>
        </section>
        <section id="b">
            <p>paragraf 4</p>
            <ul>
                <li>item 1</li>
                <li>item 2</li>
                <li>item 3</li>
            </ul>
        </section>
    </div>
</body>

</html>
```
- ambil Element judul dengan id, dan masukan ke variabel judul
```
let judul = document.getElementById('judul');
```
> judul =  ``` <h1 id="judul">Hello World</h1> ```
- rubah tulisan Hello World menjadi "I'm comming World"
```
judul.innerText = "I'm comming World";
```
> judul =  ``` <h1 id="judul">I'm comming World</h1> ```