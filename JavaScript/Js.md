# JAVA SCRIPT

#### JavaScript was created by **Brendan Eich** in 1995 during his time at Netscape Communications. It was inspired by Java, Scheme and Self

**It is a case sensitive language**

# comments

1. single line //
2. Multi line /\*\*/

# Data types

1. undefined
2. null
3. boolean
4. string
5. symbol
6. number
7. object

## some other types

1. var
   - this is used for defining variable whose scope is limited to function it is defined, and you can declare the same datatype many times like
   ```
   var nik="rol"
   var nik="fsf"
   ```
2. let
   - this is same as var but it is limited to block where it is defined,and you can not declare a variable again if it is defined already but you can assign new values to it. **let** is more safer than **var**
3. const
   - this is used for defining const variable and it has all the properties of let keyword
   ```
   const a=[1,2,3]
   // not possible a=[2,34,4] but
   a[0]=1
   a[1]=32 //this is possible

   object.freeze(a); //now you can't change the value of a
   ```


## operator **++** is working like c++

# String

1. A string can be single quotes or double quotes like python
2. you can use 'backtick' and in backtick you can use double and single quotes both

## length of string

```
var str=23
var len= str.length
```

# **Object** dataType

```
var nik={
    "name":["nikhil"],
    "class":"c2",
    "dob":6,
    12:"12"
}

//retrieving values
nik.class,nik.dob,nik["name"]

//changing value of object properties
nik.class="E+f"

//adding new properties
nik.surname="Saini"

//deleting properties
delete nik.dob

//checking existence
nik.hasOwnProperty("dob")
```

# **Object Array**

```
var nik=[
    {
        "n"="i",
        "i"="k"
    },
    {
        "k"="h",
        "h"="i",
        "i"="l"
    }

]
```
# Random function
```
math.random() //it will generate a random number between 0 to 1

math.floor(math.random*20) //it will gererate number from 1 to 19
```

# Parsing INT from a string
```
a="1010"
b=parseInt(a,2) //base 2
c=parseInt(a) //base 10
```

# Anonymous function
```
let a=()=> new Data();

// with args
let a=(arr1,arr2)=>arr1.concat(arr2);

a([1,2,1],[23,423,23])
```

# Multi args function 
```
function a(...){

}

//multi args in an array
function a(...args)
```

# copying array
```
arr2=[...arr1]
arr2=arr1 //it is not copying it is reference passing
```

# assign variable from object Or Destructuring an Object
```
let a=[x:2,y:{nu:23},z:5]
const {x:a,y:{nu:y},z:c}=a;
```

# Destructuring an array
```
let [a,b,c, ,d]=[34,33,2,4,3,33,3]

output 
a=34
b=33
c=2
d=3

//or

[a,b]=[b,a]
```
# Destructuring in args of fun
```
let a={
    max:34,
    min:32
}
function fun({max,min}){
    console.log(max,min) //34,32
}
fun(a)
```
# Returning a object form taking a value as a function args
```
const createPerson=(name,age,gender)=>({name,age,gender})
createPerson("nikhil",20,"male")
```
