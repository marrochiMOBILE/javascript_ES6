
# block-scope

```
aku tidak membutuhkan pasangan ataupun yang lainya. aku hanya butuh seseorang yang bisa menerangi jalan hidup.

kutipan : m++
01/05/2021
```

## apa itu block-scope
```
block scope adalah ruang lingkup di dalam area kurung kurawal {}, seperti if statement, switch statement, for loop, while loop, dan do while loop. Variabel yang dideklarasikan dalam block scope biasa disebut block level variable
```

cotohnya sederahana :
```js
if(true){
    var nama ="marrochi"
}
console.log(nama) // marrochi

if(true){
    let umur = 90
}
console.log(umur) // ERROR

if(true){
    const tinggi = 170
}

console.log(tinggi) // ERROR

```
contoh kedua :

```js
number = 0
for(var i = 0 ; i<4; i++){
   number =number + i
}

console.log(i) // 4
console.log(number) // 6

/*
---------------------------------------------
  i  |   i < 4 | number = number + i |  i++ |
---------------------------------------------
 0   |    t    |   number = 0 + 0    |  0+1 |
 1   |    t    |   number = 0+1      |  1+1 |
 2   |    t    |   number = 1+2      |  2+1 |
 3   |    t    |   number = 3+3      |  3+1 |
 4   |    f    |                     |      |
 --------------------------------------------
*/

```
coba bandingkan dengan ini
```
number = 0
for(let i = 0 ; i<4; i++){
   number =number + i
}

console.log(i) // error
console.log(number) // 6

```

## no 1 yang tidak diperbolehkan dalam block-scope
1 nama variabel yang sama didalam scope. maksudnya ketika global-scope dan block-scope dengan nama yag sama bernama `nama` maka mesin akan bingung membaca mau yg mana? karena dua duanya sama sama di init/inisialisasi
```js
let nama = "marrochi"


if(true){
    console.log(nama) // marrochi
}

if(true){
console.log(nama) // error
let nama ="aryo"
console.log(nama)
}

if(true){
    let nama = "aryo seto"
    console.log(nama)  // aryo seto

    if(true){
        // console.log(nama)  error = karena bingung dia mau ngambil nama yang mana karena didalam if ada variabel nama lagi
        let nama = "eko"
        console.log(nama) // eko
    }
}
```
