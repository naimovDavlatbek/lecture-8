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
      console.log(person.name + " "+person.surname); ///  Davlatbek Naimov
    
  ````

Ҳар як номи хосият пеш аз ду нуқта индентификатор аст (ё ном, рақам ё сатри аслӣ) ҳар як арзиши н ифодаест, ки арзиши он
 бо номи амвол таъин шудааст. Номи амвол метавонад ифода бошад: калидҳои ҳисобшуда бояд дар қавсҳои мураббаъ печонида шаванд. 