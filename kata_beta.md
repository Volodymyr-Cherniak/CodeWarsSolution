# CodeWars Tasks
## Kata Beta
* https://www.codewars.com/kata/566039931cb747be82000095/train/javascript
```js
const lastTwo = (arr) => arr.slice(-2).sort((a,b)=>a-b);
```  
* https://www.codewars.com/kata/switch/train/javascript
```js
function caseInSwitch(val) {
  if (val === 1) return "alpha";
  if (val === 2) return "beta";
  if (val === 3) return "gamma";
  if (val === 4) return "delta"; 
}
```
* https://www.codewars.com/kata/letter-to-ascii/train/javascript
```js
const charToASCII = (c) => c.charCodeAt(0);
```
* https://www.codewars.com/kata/percentage-of-number-array/train/javascript 
### stupid task

```js
function percentageSumArray(arr){
  if (arr == null) return false;
  if (arr.length == 0)return false;
  let arr2 = [],
      num = 0,
      sum = 0;      
  
  for (let i in arr) {
    if (arr[i] != 0) {
      if (typeof arr[i] == "object") return false;
      arr2.push(arr[i]);
      sum += arr[i];
    }  
  }
  if (sum <= 0) return false;
  if (arr2.length == 0) return false;
  num = (arr2.length * sum)/100;
  if (f(num) > 2) return +num.toFixed(2);
  return num;
}

const f = x => ( (x.toString().includes('.')) ? (x.toString().split('.').pop().length) : (0) );
```
* https://www.codewars.com/kata/need-change/train/javascript
### stupid task
```js
function getChange(m) {
  console.log(m);
  let num = 0;
  let arr = [];
  let arr2 = [25,10,5,1];
  
  
  while (m >= 1){
    
    if (m / arr2[0] >= 1){
      num = Math.floor(m / arr2[0]);
      m -= (arr2[0] * num);
      arr.push(`${num}x${arr2[0]}c`);
    }
    else if (m / arr2[1] >= 1){
      num = Math.floor(m / arr2[1]);
      m -= (arr2[1] * num);
      arr.push(`${num}x${arr2[1]}c`);
    }
    else if (m / arr2[2] >= 1){
      num = Math.floor(m / arr2[2]);
      m -= (arr2[2] * num);
      arr.push(`${num}x${arr2[2]}c`);
    }
    else {
      num = m;
      arr.push(`${num}x${arr2[3]}c`);
      break;
    }  
  }
  
   console.log(arr.join('+')); //return arr.join('+');
}
```
* https://www.codewars.com/kata/smallest-pair-sum/train/javascript
```js
function smallestPairSum(number){
 
 number.sort((a,b)=>a-b);
 return number[0] + number[1];
}
```
* https://www.codewars.com/kata/holy-cats/train/javascript
```js
function holycats(input){
  let hollyCats = input.filter(el => el.split('').includes('_'));
  return hollyCats;
}
```
