![Image Banner!](assets/react-lanjutan-banner.png "Javascript")
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