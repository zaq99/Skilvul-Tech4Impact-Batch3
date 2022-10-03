![Image Banner!](../assets/js-banner-DOM.png "Javascript")
# **DOM (Document Object Model)**
### Apa itu DOM ?
>  DOM berisi kumpulan aturan atau cara bagi programmer untuk memanipulasi apapun yang tampil dalam halaman web. DOM tidak terikat dengan JavaScript, dan juga bukan bagian dari JavaScript. DOM yang sama bisa diakses dengan bahasa client-side lain seperti JScript.

### Bagaimana Peran DOM pada WEB development ?
> DOM adalah jembatan agar bahasa pemrograman bisa berinteraksi dengan dokumen html

### Beberapa Syntax/method pada DOM :
1. Traversing/Akses Element
>- Kebawah
>   - getElementById()
>   - getElementsByTagName()
>   - getElementsByClassName()
>   - querySelector()
>   - querySelectorAll()
>   - children()
>- Keatas
>   - parentElement()
>   - closets()
>- Kesamping
>   - nextElementSibling()
>   - previousElentSibling()

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