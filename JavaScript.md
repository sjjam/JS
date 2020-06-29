# JavaScript

## 변수 할당

var varNum = 3
var varNum = 4
varNum = 15
console.log(varNum)
VM364:4 15



----

let letNum = 3
let letNum = 10
VM433:2 Uncaught SyntaxError: Identifier 'letNum' has already been declared
letNum = 15
15



----

const constNum = 3

const constNum = 19
VM556:1 Uncaught SyntaxError: Identifier 'constNum' has already been declared

constNum = 10
VM588:1 Uncaught TypeError: Assignment to constant variable.
    at <anonymous>:1:10



---

var a = 1
undefined
var b = 2
undefined
if ( a === 1 ) {
    console.log(a)
    var a = 3
    console.log(a)
}
VM836:2 1
VM836:4 3
undefined
console.log(a)
VM879:1 3



----

let lNum = 10

if (lNum === 10) {
    let lNum = 30
    console.log(lNum)
}
console.log(lNum)
VM1218:3 30
VM1218:5 10



변수 선언 var 사용 x

let 재할당 가능

const 재할당 불가능



---

const colors = ['red', 'blue', 'green']
undefined

colors.forEach(function(color) {
    console.log(color)})
VM2063:2 red
VM2063:2 blue
VM2063:2 green



forEach

const images = [
    {width: 30, height: 10},
    {width: 20, height: 20},
    {width: 50, height: 30},
]
undefined
const areas = []



images.forEach(function(image) {
    areas.push(image.width * image.height)
})
undefined
console.log(areas)
VM3567:1 (3) [300, 400, 1500]



![image-20200629103454814](C:\Users\student\AppData\Roaming\Typora\typora-user-images\image-20200629103454814.png)



![image-20200629103614353](C:\Users\student\AppData\Roaming\Typora\typora-user-images\image-20200629103614353.png)



onst name = 'kim'
undefined
console.log('hello,' + name)
VM273:1 hello,kim
undefined
console.log(`hello, ${name}`)
VM352:1 hello, kim
undefined
const greeting = function(name) {
    console.log(name)
}
undefined
greeting()
VM544:2 undefined
undefined
greeting(name)
VM544:2 kim
undefined
const arrow = name => name
undefined
arrow(name)
"kim"
square = function(num) {
    console.log(num**2)
}
ƒ (num) {
    console.log(num**2)
}
square = num => console.log(num**2)
num => console.log(num**2)
square(3)
VM1125:1 9



const noArgs = () => 'noArgs'
undefined



const returnObject = () => ({key: 'value'})



