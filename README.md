# lecture-8
 ## Объектҳо, хосиятҳо ва усулҳои ҳаёти воқеӣ.
 Дар ҳаёти воқеӣ, мошин як объект аст .
Мошин дорои хосиятҳое ба монанди вазн ва ранг ва усулҳо ба монанди оғоз ва боздошт:
  
   ### Object
   + Мошин.
  
  ### Хосиятҳо 
  + car.name = BMW.
  + car.model = M5
  + car.weight = 1850kg.
  + car.color = white.

  ### Methods.
  + car.start()
  + car.drive()
  + car.brake()
  + car.stop()
  
  Ҳама мошинҳо хосиятҳои якхела доранд , аммо арзишҳои амвол аз мошин ба мошин фарқ мекунанд.
  Ҳама мошинҳо усулҳои якхела доранд , аммо усулҳо дар вақтҳои гуногун иҷро карда мешаванд .
  ____

  ## What is Object in Java Script?
Объектҳоро дар JavaScript, мисли бисёр забонҳои дигари барномасозӣ бо объектҳои ҳаёти воқеӣ муқоиса кардан мумкин аст. Дар JavaScript, объект як объекти мустақил буда, дорои хосиятҳо ва намуд мебошад. Масалан, онро бо коса муқоиса кунед. Коса ашёест, ки дорои хосиятҳост. Коса дорои ранг, тарҳ, вазн, маводе, ки аз он сохта шудааст ва ғайра. Ба ҳамин тариқ, объектҳои JavaScript метавонанд хосиятҳое дошта бошанд, ки хусусиятҳои онҳоро муайян мекунанд.

## Creating new objects.
 Шумо метавонед объектро бо истифода аз оғозкунандаи объект эҷод кунед. Интихобан шумо метавонед аввал 
 як функсияи созанда эҷод кунед ва сипас бо истифода аз функсия бо оператори нав объектро эҷод кунед.
 ````Javascript 
 let  person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
 ````
````Javascript
let  person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
````
____
 ## Дастрасӣ ба хосиятҳои объект.
 Шумо метавонед ба хосиятҳои объект бо ду роҳ дастрасӣ пайдо кунед:

````Javascript
objectName.propertyName
````
````Javascript
objectName["propertyName"]
````
### Example.

````Javascript
   let person = {
    surname: "Naimov",
     name: "Davlatbek",
     phone: 54146,
   }
      console.log(person.name + " "+person.surname); 
    
  ````

Ҳар як номи хосият пеш аз ду нуқта индентификатор аст (ё ном, рақам ё сатри аслӣ) ҳар як арзиши н ифодаест, ки арзиши он
 бо номи амвол таъин шудааст. Номи амвол метавонад ифода бошад: калидҳои ҳисобшуда бояд дар қавсҳои мураббаъ печонида шаванд. 

 ____


## JavaScript Object.entries()
Усули Object.entries()статикӣ массиви ҷуфтҳои калиди-арзиши моликияти шуморашавандаи дорои сатри калиддори объекти додашударо бармегардонад.

````Javascript
const object1 = {
  a: 'somestring',
  b: 42,
};

for (const [key, value] of Object.entries(object1)) {
  console.log(`${key}: ${value}`);
}

// Expected output:
// "a: somestring"
// "b: 42"

````
ES2017 Object.entries()усулеро муаррифӣ мекунад, ки объектро қабул мекунад ва [key, value]ҷуфтҳои моликияти рақамии сатри калиддори объектро бармегардонад.


Ин аст синтаксиси усул Object.entries():

````Javascript
const ssn = Symbol('ssn');
const person = {
    firstName: 'John',
    lastName: 'Doe',
    age: 25,
    [ssn]: '123-345-789'
};

const kv = Object.entries(person);

console.log(kv);
  //Run 
// //[
//     ['firstName', 'John'],
//     ['lastName', 'Doe'],
//     ['age', 25]
// ]
````
Дар ин мисол:

, firstName, lastNameва ageхосияти шуморишшавандаи сатри калиддори объект мебошанд person, бинобар ин, онҳо ба натиҷа дохил карда мешаванд.
ssn Хусусияти калиди сатри объекти шахс нест, бинобар ин он ба натиҷа дохил карда нашудааст .


___
##  JavaScript Object.keys()

Усули Object.keys()статикӣ массиви номҳои моликияти дорои сатри калиддоршудаи объекти додашударо бармегардонад.

Example 
````Javascript
const object1 = {
  a: 'somestring',
  b: 42,
  c: false,
};

console.log(Object.keys(object1));
// Expected output: Array ["a", "b", "c"]

````
___
##  JavaScript Object.values()

Усули Object.values()статикӣ массиви арзишҳои хосиятҳои рақамии сатри калиддори объекти додашударо бармегардонад.

````Javascript
const object1 = {
  a: 'somestring',
  b: 42,
  c: false,
};

console.log(Object.values(object1));
// Expected output: Array ["somestring", 42, false]
````

____
## What is Destructuring && Spread in Java Script.
Синтаксиси таъиноти вайронкунанда ифодаи JavaScript мебошад, ки имкон медиҳад, ки арзишҳоро аз массивҳо ё хосиятҳо аз объектҳо ба тағирёбандаҳои ҷудогона кушоед.

JavaScript has two awesome data structures that help you write clean and efficient code. But handling them can get messy sometimes.

## Деструктуризатсияи массив дар JavaScript чист?
 Фарз мекунем, ки мо массив дорем, ки панҷ рақамро дар бар мегирад, ба монанди:

 ````Javascript
 let array1 = [1, 2, 3, 4, 5]
 ````
 Барои ба даст овардани элементҳо аз массив, мо метавонем кореро иҷро кунем, ба монанди гирифтани рақам аз рӯи индексҳои он:
 Гирифтани элементҳои массив
 ````Javascript
 array1[0];
array1[1];
array1[2];
array1[3];
array1[4];
````
____
Аммо ин усул кӯҳна ва душвор аст ва роҳи беҳтари иҷрои он вуҷуд дорад - бо истифода аз вайронкунии массив. Чунин ба назар мерасад:
````Javascript
let [ indexOne, indexTwo, indexThree, indexFour, indexFive ] = array1;
````
Ҳарду усули дар боло овардашуда натиҷаи якхела медиҳанд:

___
## What is Object Destructuring in JavaScript?
Ин вайронкунӣ бо объектҳо низ хуб кор мекунад. Ичозат дихед ба шумо як мисол оварам.

````Javascript
let object = {
    name: "Nishant",
    age: 24, 
    salary: 200,
    height: '20 meters',
    weight: '70 KG'
}

````
Фарз мекунем, ки мо мехоҳем, ки ном, маош ва вазни ин объект дар консол чоп карда шавад.
````Javascript
console.log(object.name)
console.log(object.salary)
console.log(object.weight)
````

Мо метавонем онҳоро бо истифода аз калидҳо, ки ном, маош ва вазн мебошанд, ба даст орем.


````Javascript
let a, b, rest;
[a, b] = [10, 20];

console.log(a);
// Expected output: 10

console.log(b);
// Expected output: 20

[a, b, ...rest] = [10, 20, 30, 40, 50];

console.log(rest);
// Expected output: Array [30, 40, 50]

````

___
## Чӣ тавр истифода бурдани вайронкунии объект бо функсияҳо

Фарз мекунем, ки мо функсияе дорем, ки тамоми маълумотро дар массив ба консол чоп мекунад.

````Javascript
let object = {
    name: "Nishant",
    age: 24, 
    salary: 300,
    height: '20 meters',
    weight: '70 KG'
}

function printData(){
    
}

printData(object)
````
Мо объектро ҳамчун параметр дар функсия мегузорем, вақте ки он даъват мешавад:

````Javascript
let object = {
    name: "Nishant",
    age: 24, 
    salary: 300,
    height: '20 meters',
    weight: '70 KG'
}

function printData(object){
    console.log(object)
}

printData(object)
````
Дар ин ҷо, мо объектро ба ном, синну сол, маош, баландӣ ва вазн дар параметрҳои функсия вайрон карда истодаем ва ҳама чизро дар як сатр чоп мекунем.

____

## Оператори Spread дар JavaScript чист?

Паҳншавӣ маънои паҳн кардан ё васеъ карданро дорад. Ва оператори паҳншуда дар JavaScript бо се нуқта ишора шудааст.
Ин оператори паҳншуда истифодаи зиёди гуногун дорад.

Намунаҳои паҳнкунандаи оператор
Фарз мекунем, ки мо ду массив дорем ва мо мехоҳем онҳоро якҷоя кунем.


Якҷоя кардани ду массив бо усули concat
````Javascript
let array1 = [1, 2, 3, 4, 5]
let array2 = [6, 7, 8, 9, 10]

let array3 = array1.concat(array2);
console.log(array3)
````

Мо омезиши ҳарду массивро мегирем, ки массиви 1 ва массиви 2 мебошанд.

Аммо роҳи осонтари ин кор вуҷуд дорад:

Якҷоя кардани ду массив бо Оператори Spread

````Javascript
let array1 = [1, 2, 3, 4, 5]
let array2 = [6, 7, 8, 9, 10]

let array3 = [...array1, ...array2]
console.log(array3)
````
Дар ин ҳолат, мо оператори паҳнро барои якҷоя кардани ҳарду массив истифода мебарем.
