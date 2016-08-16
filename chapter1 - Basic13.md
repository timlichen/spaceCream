####Basic 13
<b>Java</b> - Print 1 - 255
```java
public void print1to255(){
    for (int i=1; i <= 255; i++){
        System.out.println(i);
    }
}
```
<b>Java</b> - Print Odds 1 - 255
```java
public void printOdds(){
    for (int i=1; i <= 255; i+=2){
        System.out.println(i);
    }
}
```
<b>Java</b> - Print And Sum 1 - 255
```java
public void printAndSum255(){
    int sum = 0;
    for (int i=1; i <= 255; i++){
        sum += i;
        System.out.println(i);
    }
    System.out.println("Sum is: "+sum);
}
```
<b>Java</b> - Print Average
```java
public void printAvg(int[] nums){
    double sum = 0;
    for (int i=0; i < nums.length; i++){
        sum += nums[i];
    }
    System.out.println(sum/nums.length);
}
```
<b>Java</b> - Print Max
```java
public int printMax(int[] nums){
    int max = nums[0];
    for (int i=0; i < nums.length; i++){
        if (nums[i] > max){
            max = nums[i];
        }
    }
    return max;
}
```
<b>Java</b> - Array of Odds
```java
public ArrayList makeOddArray(){
    //going with arraylist since it can have a dynamic length
    ArrayList odds = new ArrayList();
    for (int i=1; i <= 255; i+=2){
        odds.add(i);
    }
    return odds;
}
```
<b>Java</b> - Square Array Values
```java
public int[] squared(int[] nums){
    for (int i = 0; i < nums.length; i++){
        nums[i] = nums[i] * nums[i];
    }
    return nums;
}
```
<b>Java</b> - Greater Than Y
```java
public int greaterThanY(int[] nums, int y){
    int count = 0;
    for (int i = 0; i < nums.length; i++){
        if (nums[i] > y){
            count++;
            System.out.println(nums[i]);
        }
    }
    return count;
}
```
<b>Java</b> - Replacing Negatives
```java
public int[] removeNegs(int[] nums){
    for (int i = 0; i < nums.length; i++){
        if (nums[i] < 0){
            nums[i] = 0;
        }
    }
    return nums;
}
```
<b>Java</b> - Min Max Average
```java
public void maxMinAvg(int[] nums){
    int sum = 0;
    int min = nums[0];
    int max = nums[0];
    for (int i = 0; i < nums.length; i++){
        sum += nums[i];
        if (nums[i] > max){
            max = nums[i];
        }
        if (nums[i] < min){
            min = nums[i];
        }
    }
    System.out.println("Max: "+max+" Min: "+min+" Avg: "+sum/nums.length);
}
```
<b>Java</b> - Shift Array
```java
public int[] shiftArray(int[] nums){
    for (int i = 0; i < nums.length-1; i++){
        nums[i] = nums[i+1];
    }
    nums[nums.length-1] = 0;
    return nums;
}
```
<b>Java</b> - "Dojo" Negatives
```java
public ArrayList stringNegs(int[] nums){
    ArrayList dojoNums = new ArrayList();
    for (int i = 0; i < nums.length; i++){
        if (nums[i] < 0){
            dojoNums.add("Dojo");
        }else{
            dojoNums.add(nums[i]);
        }
    }
    return dojoNums;
}
```
