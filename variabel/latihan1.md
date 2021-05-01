
# variabel 
```
tidak semua yang saya bayangkan itu bakal terjadi
saya sadar apa yang harus saya lakukan saat itu
tapi pada kenyataannya harapan dan usaha yang saya 
lakukan terlalu berlebihan hingga merusak taman saya sendiri.

kutipan : m++
27/04/2021
```

## apa itu variabel?
```
variabel adalah tempat menyimpan nilai
```
contoh sederhananya :
```js
var nama = "marrochi"
console.log(nama) // marrochi
```
bandingkan jika tidak menggunakan variabel
```js
console.log("marrochi") // marrochi
```

## ada  3 jenis variabel

<ol>
  <li>var</li>
  <li>let</li>
  <li>const</li>
</ol>

### perbedaan yang jelas yaitu scope

```
var => function scope

let dan const => block scope
```
<p>tentang masalah ini nanti liat materi</p>

> block scope 

> function scope 

> perbedaan variabel   [ jika ada ]

## pemberian jenis variabel
```js
// pemberian let
let nama = "aryo seto"

// tidak diberi
nama2   = "winda"


console.log(nama+nama2)
```

```
output:
aryo seto
winda
```

> pemberian yang tidak diberi biasanya berjenis ***let***

## perbedaan diberi atau tidak
```js
let nama
nama2

console.log(nama) // undifined / tidak terdefinisi
console.log(nama) // error
```

```js
let ok
if(ok){
    console.log("true-ok")
}else{
    console.log("else-ok") // tampil
}

ok2
if(ok2){
    console.log("true-ok2")
}else{
    console.log("else-ok2") // error
}
```

```js
let nama 

function namaku() {
    console.log(nama)
}

nama2

function namadia(){
    console.log(nama2)
}


namaku()  // undifined
namadia() // error
```
kesimpulanya ketika kita ***tidak memberikan jenis variabel maka harus menetukan nilainya jika tidak terjadi eror/kesalahan***
