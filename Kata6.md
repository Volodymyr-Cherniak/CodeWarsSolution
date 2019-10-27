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
