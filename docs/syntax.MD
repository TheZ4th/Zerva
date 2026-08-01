# Syntax Of Zeron Programing Language

## Import Syntax
this is Import library syntax in zeron Programing Language

### Example

```zeron
load [std.io]
load [str.io]
```

## Declaration the type of data

### Example
this how you Declaration type of data in zeron Programing Language

```zeron
let str >> $Variable > "Example";
let int >> $Number > 16;
let flt >> $Float > 3,14;
let bool >> true;
```

## Print function
this is print syntax in zeron Programing Language

### Example

```zeron
load [std.io]

func main{
    
    let str >> $Example > "hello from Zeron";
    std.io.fprint("%s",$Example);
}
```

## If,Elif,Else and Execption statment
This how you create a If,Elif,Else and Execption statment in Zeron Programing Language

### Example for string Variable

```zeron
load [std.io]/

func main{
    
    let str >> $Name >

    std.io.read(str) >> $Name

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

func main{
    
    let int >> $age;
    std.io.read(int) >> $age;

    if ($age >> 18 -> 30) {
        fprint("You Are Young");
    }
    else if ($age >> 31 -> 60 :! 61) {
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


