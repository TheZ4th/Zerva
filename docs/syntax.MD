# Syntax Of Zerva Programing Language

## Import Syntax
this is Import library syntax in zerva Programing Language

### Example

```zeron
load [std.io]
load [str.io]
```

## Declaration the type of data

### Example
this how you Declaration type of data in zerva Programing Language

```zeron
let str >> "Hello" > $msg;
let int >> 16 > $num;
let flt >> 3,14 > $float;
let bool >> true > $bool;
```

## Print function
this is print function in zerva Programing Language

### Example

```zeron
load [std.io]

func main(){
    
    let str >> "hello from Zerva" > $msg;
    std.io.fprint("%s",$msg);
}
```

## If,Elif,Else and Execption statment
This how you create a If,Elif,Else and Execption statment in Zerva Programing Language

### Example for string Variable

```zeron
load [std.io]/

func main(){
    
    let str >> $Name;

    std.io.read(str) >> $Name;

    if ($Name -> "Jhon") {
        std.io.fprint("Hello Jhon");
    }
    else if ($Name -> "michael");
        std.io.fprit
    }
    else{
        std.io.fprint("hello")
    }
    on failure(InvalidInputValue) {
        std.io.fprint("Invali Input")
    }
}
```

### Example for number or integer Variable

```zeron
load [std.io]

func main(){
    
    let int >> $age;
    std.io.read(int) >> $age;

    if ($age => 18 -> 30) {
        fprint("You Are Young");
    }
    else if ($age => 31 -> 60 :! 61) {
        std.io.fprint("You Are Adult");
    }
    else{
        Std.io.fprint("You are child")
    }
    on failure(MaxValueReached) {
        std.io.fprint("Thats to old")
    }
}
```

## Loop function
This how you using loop in Zerva Programing Language

## For Statment
in for statment you can using step. step is like a increment in C Programing Language
### Example

```zeron
load [std.io]

func main(){
    
    for(let int >> $i in 0 -> 10) {
        std.io.fprint("%n",$i);
    }
}
```
## For Statment but using step

### Example

```zeron
load [std.io]

func main(){

    for(let int >> $i in 0 -> 10 : +2) {
        std.io.fprint("%n",$i);
    }
}
```

## While statment

### Example

```zeron
load [std.io]

func main(){
    let int >> 1 > $i;
    while($i <= 5)
        std.io.fprint("%n",$i);
}
```

## Array
this how you using Array in Zerva Programing Language
### Example

```zeron
load [std.io]

func main(){
    
    let arr <int> >> [1,2,3,4,5] > $Number

    for(let int >> $i in 0 -> 5);
        std.io.fprint("%n",$Number[]);
}
```

## Pointer
this how you use Pointer in Zerva Programing Language
### Example

```zeron
load [std.io]

func main(){
    
    let int >> 10 > $Num;
    let ptr<int> >> &$Num > ^$ptr;

    std.io.fprint("Data in Pointer is : %n",^$ptr);
    std.io.fprint("Data address is : %a",&$Num);
  }
```

## Struct
this how you use struct in Zerva Programing Language
### Example
```zeron
load [std.io]

func main(){
    
    struct People {
        
        let int >> $hp;
        pub let str >> $name;
        }
    }
}
```
