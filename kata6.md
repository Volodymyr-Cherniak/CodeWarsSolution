# CodeWars Tasks
## Kata 6
* https://www.codewars.com/kata/mexican-wave/train/javascript
```js
function wave(str){
  console.log(str);
  let arr = [];
  let arrClear;
  
  for (let i in str){
    arr.push(words(str, i));
  } 
   
  arrClear = arr.filter(el => el !== undefined);
  
  return arrClear;
}


function words(str, num){

  let arr = str.split('');

  if(str[num] != ' '){
   arr[num] = arr[num].toUpperCase();
   return arr.join('');
  }
}
```
* https://www.codewars.com/kata/roman-numerals-decoder/train/javascript
```js
function solution(r){
    let sum = 0; 
  
  for (let i in r){
    if (r[i] == 'M') sum += 1000;if (r[i] == 'D') sum += 500;
     if (r[i] == 'C') sum += 100;
     if (r[i] == 'L') sum += 50;
     if (r[i] == 'X') sum += 10;
     if (r[i] == 'V') sum += 5;
     if ((r[i-1] == 'I') && (r[i] == 'V')) sum -= 1;
     if (r[i] == 'I') sum += 1;
     if ((r[i-1] == 'I') && (r[i] == 'V')) sum -= 1;
  }
  return sum;
}
```
* https://www.codewars.com/kata/multi-tap-keypad-text-entry-on-an-old-mobile-phone/train/javascript
```js
function presses(phrase) {
   let res = phrase.replace(/[23456S8Z]/gi, '4')
                   .replace(/[79]/gi,'5')
                   .replace(/[ADGJMPTW ]/gi,'1')
                   .replace(/[BEHKNQUX0]/gi, '2')
                   .replace(/[CFILORVY]/gi,'3')
                   .split('')
                   .reduce(function(a, b) {
                             return +a + +b;
                           });
  return +res;
};
```
* https://www.codewars.com/kata/break-camelcase/train/javascript
```js
function solution(str) {
    let strWithSpace = [];
    
    for (let i in str){
      if (str[i] === str[i].toUpperCase()) strWithSpace.push(' ');
        strWithSpace.push(str[i]);
    }
    return strWithSpace.join('');
}
```
* https://www.codewars.com/kata/triple-trouble-1/train/javascript
```js
function tripledouble(num1, num2){
  num1 = num1 + '';
  num2 = num2 + '';
  
  for (let i = 0; i < num1.length; i++){

    for(let j = 0; j < num2.length; j++){

      if ((num2[j] === num1[i]) && (num2[j+1] === num1[i+1]) && (num2[j+1] === num1[i+2]) && (num2[j] === num1[i+2])) return 1;
    }
  }
  return 0;
}
```
