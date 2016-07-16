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
