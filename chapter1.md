## Chapter 1 - Fundamentals
__Page 15__

##### Setting and Swapping

__JavaScript__
```javascript
var myNumber = 42;
var myName = "Tim";
var temp = myNumber;
myNumber = myName;
myName = temp;
```

__Python__
```python
myNumber = 42
myName = "Tim"
temp = myNumber
myNumber = myName
myName = temp
```

#### Print and Count

__JavaScript__
```javascript
function printAndCount(){
  var counter = 0
  for(var x = 512; x <= 4096; x+=5){
    counter++
    console.log(x)
  }
  console.log(counter)
}
```
__Python__
```python
def printAndCount():
  counter = 0
  for x in range(512, 4096, +5):
    counter += 1
    print x
  print counter
```

#### Print -52 to 1066

__JavaScript__

```javascript
function printRange(){
  for(var x = -52; x <= 1066; x++){
    console.log(x)
  }
}
```
__Python__
```python
def printRange(){
  for x in range(-52, 1067){
    print x
  }
}
```

#### Multiples of Six

__JavaScript__
```javascript
function multiplesOfSix(){
  var count = 6
  while(count <= 60000){
  console.log(count)
  count += 6
  }
}
```

__Python__
```python
def multiplesOfSix():
  count = 6
  while count <= 60000:
    print count
    count += 6
```

#### Counting, the Dojo Way

__JavaScript__
```javascript
function dojoCount(){
  for(var x = 1; x <= 100; x++){
    if(x % 5 == 0){
      console.log("Coding")
      if(x % 10 == 0){
        console.log("Dojo")
      }
    } else {
      console.log(x)
    }
  }
}
```

__Python__
```python
def dojoCount():
  for x in range(1,101):
    if x % 5 == 0:
      print "Coding"
      if x % 10 == 0:
        print "Dojo"
    else:
      print x
```

#### What Do You Know?

__JavaScript__
```javascript
function incomingParams(incoming){
  console.log(incoming)
}
```
__Python__
```python
def incomingParams(incoming):
  print incoming
```

#### Whoa, That Sucker's Huge...

__JavaScript__
```javascript
function hugeNum(){
  var sum = 0
  for(var x = -300000; x <= 300000; x++){
    if(x % 2 != 0){
      sum += x
    }
  }
  console.log(x)
}
```

__Python__
```python
def hugeNum():
  sum = 0
  for x in range(-300000, 300001):
    if x % 2 != 0:
      sum += x
  print x
```

#### Countdown By Fours

__JavaScript__
```javascript
function countDown(){
  var start = 2016
  while(start > 0){
    if(start % 2 === 0){
      console.log(start)
    }
    start -= 4
  }
}
```

__Python__
```python
def countDown():
  start = 2016
  while start > 0:
    if start % 2 == 0:
      print start
    start -= 4
```

#### Flexible Countdown

__JavaScript__
```javascript
function flexCount(lowNum, highNum, mult){
  for(var x = highNum; x > lowNum; x -= mult){
    console.log(x)
  }
}
```

__Python__
```python
def flexCount(lowNum, highNum, mult):
  for x in range(highNum, lowNum, -mult):
    print x
```

#### The Final Countdown

__JavaScript__
```javascript
function finalCountDown(num1, num2, num3, num4){
  while(num2 < num3){
    if(num2 % num4 != 0){
      if(num2 % num1 === 0){
        console.log(num2)
      }
    }
    num2++
  }
}
```

__Python__
```python
def finalCountDown(num1, num2, num3, num4):
  while num2 < num3:
    if num2 % num4 != 0:
      if num2 % num1 == 0:
        print num2
    num2 += 1
```
