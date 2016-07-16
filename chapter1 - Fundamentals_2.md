## Chapter 1 - Fundamentals
__Page 19__

### Countdown

__JavaScript__
```javascript
function countDown(num){
  var arr = []
  for(var x = num; x >= 0; x--){
    arr.push(x)
  }
  console.log(arr)
  return arr
}
```

__Python__
```python
def countDown(num):
  list = []
  for x in range(num, -1, -1):
    list.append(x)
  print list
  return list
```

### Print and return

__JavaScript__
```javascript
var arr = [1,2]
function printAndReturn(arr){
  console.log(arr[0])
  return arr[1]
}
```

__Python__
```python
list = [1,2]
def printAndReturn(list):
  print list[0]
  return list[1]
```

### First Plus Length

__JavaScript__
```javascript
var arr1 = [1,2,3,4] // 5
var arr2 = [true,2,3,4] // 5
var arr3 = [false,2,3,4] // 4
var arr4 = ["string",2,3,4] // "string4"

function firstPlusLength(arr){
  return arr[0] + arr.length
}
```

__Python__
```python
list1 = [1,2,3,4] # 5
list2 = [True,2,3,4] # 5
list3 = [False,2,3,4] # 4
list4 = ["string",2,3,4] # TypeError: cannot concatenate 'str' and 'int' objects

def firstPlusLength(list):
  return list[0] + len(list)
```

### Values Greater Than Second

__JavaScript__
```javascript
function greaterThan(){
  var arr = [1,3,5,7,9,13]
  var counter = 0
  for(var x = 0; x < arr.length; x++){
    if(arr[x] > arr[1]){
      counter++
      console.log(arr[x])
    }
  }
  return counter
}
```

__Python__
```python
def greaterThan():
  list = [1,3,5,7,9,13]
  counter = 0
  for x in range(0, len(list)):
    if list[x] > list[1]:
      counter += 1
      print list[x]
  return counter
```

### Values Greater Than Second, Generalized
__JavaScript__
```javascript
var arr = [1,3,5,7,9,13]
var arr2 = [1] // Returns 0, arr[1] is undefined and when
              //  compared results in a False

function greaterThan(arr){
  var counter = 0
  for(var x = 0; x < arr.length; x++){
    console.log(arr[1])
    if(arr[x] > arr[1]){
      counter++
      console.log(arr[x])
    }
  }
  return counter
}
```
__Python__
```python
list = [1,3,5,7,9,13]
list = [1] # list index out of range
def greaterThan(list):
  counter = 0

  # if len(list) < 1:
  #   return counter

  for x in range(0, len(list)):
    if list[x] > list[1]:
      counter += 1
      print list[x]
  return counter

print greaterThan(list)
```

### This Length, That Values

__JavaScript__
```javascript
function lengthValue(num1,num2){
  if(num1 === num2){
    console.log("Jinx!")
    return "Jinx!"
  } else {
    var arr = []
    for(var x = 1; x <= num1; x++){
      arr.push(num2)
    }
  }
  console.log(arr)
}
```

__Python__
```python
def lengthValue(num1, num2):
  if num1 == num2:
    print "Jinx!"
    return "Jinx!"
  else:  
    list = []
    for x in range(0, num1):
      list.append(num2)
    print list
```

### Fit the First Value

__JavaScript__
```javascript
var arr = [1,2,3,4,5]

function fitFirstVal(arr){
  if(arr[0] > arr.length){
    console.log("Too Big!")
  } else if(arr[0] < arr.length){
    console.log("Too Small!")
  } else {
    console.log("Just Right!")
  }
}
```

__Python__
```python
list = [1,2,3,4,5]

def fitFirstVal(list):
  if list[0] > len(list):
    print "Too Big!"
  elif list[0] < len(list):
    print "Too Small!"
  else:
    print "Just Right"
```

### Fahrenheit to Celsius

__JavaScript__
```javascript
function fahrenheitToCelsius(fDegrees){
  return (fDegrees - 32) * 5/9
}
```

__Python__
```python
def fahrenheitToCelsius(fDegrees):
  return (fDegrees - 32) * 5/9
```
### Celsius to Fahrenheit

__JavaScript__
```javascript
function celsiusToFahrenheit(fDegrees){
  return (9/5 * cDegrees) + 32
}

// OPTIONAL
function celsiusToFahrenheitMATCH(cDegrees){
  for(var start = cDegrees; start >= 0; start--){
    fDegrees = (9/5 * start) + 32
    if(fDegrees === start){
      return true
    }
  }
  return false
}
```

__Python__
```python
def celsiusToFahrenheit(fDegrees):
  return (9/5 * cDegrees) + 32

# OPTIONAL
def celsiusToFahrenheitMATCH(cDegrees):
    for start in range(cDegrees, -1, -1):
        fDegrees = (9/5 * start) + 32
        if fDegrees == start:
            return True
    return False
```
