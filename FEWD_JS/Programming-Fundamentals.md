## 1. If-Else Statements :- 
- ***If** statement is used to execute a block of code, if a condition is True.*
- ***Else** statement is used to execute a block of code, if a condition is False.* 

**Syntax ->**
```js script
if (Condition){
  // statement which execute when condition is true.
}
else{
  //statement which execute when condition is false.
}
```
**Example ->**
```js script
if( age >= 18 )
{
  alert("Eligible");
}
else{
  alert("Not eligible");
}
```
## 2. Else-If Statements :- 
- ***Else-if** statement is used to specify a new condition if the first condition is false* 

**Syntax ->**
```js script
if (Condition 1){
  // statement which execute when condition is true.
}
else if(condition 2)
{
  // statement which execute when 1st condition is false but 2nd is true. 
else{
  //statement which execute when condition is false.
}
```
**Example ->**
```js script
if( a > b )
{
  alert("a is greater");
}
else( b > a ){
  alert("b is greater");
}
else{
  alert("Both are equal");
}
```

## 3. Switch Statement :- 
***Switch** statement is used to execute one block of code from many different code blocks based on given expression/condition.*

**Syntax ->**
```js script
switch(expression) {
  case x:
    // statements....
    break;
  case y:
    // statements....
    break;
    .
    .
    .
  default:
    // statements....
}
```

**Example ->**
```js script
var grade = 'A';
 switch (grade) {
  case 'A': 
     alert("Excellent");
  break;
     
  case 'B': 
     alert("Good");
  break
    
  case 'C': 
     alert("Passed");
  break;
     
  case 'D': 
     alert("Do better");
  break;
            
  case 'F': 
     alert("Failed");
  break;
            
  default:  
     alert("Unknown grade")
 }
```
