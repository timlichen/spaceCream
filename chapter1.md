## Chapter 1 - Fundamentals

### Setting and Swapping


```(javascript)
var myNumber = 42;
var myName = Tim
var temp = myNumber
myNumber = myName
myName = temp
```
### Print and Count
```(javascript)
function printAndCount(){
  var counter = 0
  for(var x = 512; x <= 4096; x+=5){
    counter++
    console.log(x)
  }
  console.log(counter)
}
```

### Print -52 to 1066
```
function printRange(){
  for(var x = -52; x <= 1066; x++){
    console.log(x)
  }
}
```

### Multiples of Six
```
var count = 6
while(count <= 60000){
  console.log(count)
  count += 6
}
```
