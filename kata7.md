# My works in CodeWars
## Kata 7
* https://www.codewars.com/kata/sum-of-a-sequence/train/javascript

```js
const sequenceSum = (begin, end, step) => {
  let result = 0;

  for (let i = begin; i <= end; i += step){
    result = result + i;
  }
  return result;
};
```
* https://www.codewars.com/kata/stop-worrying/train/javascript
### beta
```````js
function worries(str){
  let arr = ["Making last-minute changes","Sitting in a dark room and shaking","Crying","Laughing hysterically","Not eating"];
  if (arr.includes(str)) return "Stop worrying, everything will be all right!";
  return "Do you really care?";
}
```````
* https://www.codewars.com/kata/sort-out-the-men-from-boys-1/train/javascript
```js
function menFromBoys(arr){
  let arr2 = [],
      arr3 = [],
      arr8 = [];
  
  arr.forEach(el =>{
    if(!arr8.includes(el)) arr8.push(el);
  });
    
  arr8.forEach(el => {
    if(el % 2) arr3.push(el);
    else arr2.push(el);
  })
 
  arr2.sort((a,b)=>a-b);
  arr3.sort((a,b)=>b-a);
  return arr2.concat(arr3);
}
```
* https://www.codewars.com/kata/v-a-p-o-r-c-o-d-e/train/javascript
```js
const vaporcode = s => s.toUpperCase().replace(/\s/g,'').split('').join('  ');
```
* https://www.codewars.com/kata/find-the-middle-element/train/javascript
```js
var gimme = function (inp) {
 let arr = [];
 let num = 0;
 inp.forEach(el => arr.push(el))
 arr.sort((a,b)=> a-b);
 for (let i in arr){
   if(arr[1] === inp[i]) num = inp[i];
 }
 return inp.indexOf(num);
};
```
* https://www.codewars.com/kata/testing-1-2-3/train/javascript
```js
var number=function(array){
  let arr1 = [];
  if (array.length === 0) return [];
  for(let i = 0; i < array.length; i++){
     arr1.push(`${i + 1}: ${array[i]}`);
   }
 return arr1;
}
```
* https://www.codewars.com/kata/simple-fun-number-176-reverse-letter/train/javascript

```js
const reverseLetter = str => str.replace(/\d/gi,'').replace(/\W/gi,'').replace(/_/gi,'').split('').reverse().join('');
```
* https://www.codewars.com/kata/lost-number-in-number-sequence/train/javascript

```js
function findDeletedNumber(arr, mixArr) {
 mixArr.sort((a, b) => a - b);
 for(let i in arr){
   if(arr[i] !== mixArr[i]) return arr[i];
 }
 return 0;
}
```
* https://www.codewars.com/kata/beginner-series-number-3-sum-of-numbers/train/javascript

```js
function getSum(a, b){
  if (a === b) return a;
  let arr = [];
  let num = 0;
  if(a < b){
   for(let i = a; i <= b; i++){
     arr.push(i);
   }
  }
  else {
    for(let i = b; i <= a; i++){
     arr.push(i);
    } 
  }
  num = arr.reduce((a, b) => a + b);
  return num;
}
```
* https://www.codewars.com/kata/sort-by-last-char/train/javascript
```js
function last(x){
   return x.split(' ')
           .map(el => el.split('').reverse().join(''))
           .sort(Comparator)
           .map(el => el.split('').reverse().join(''));
}
function Comparator(a, b) {
   if (a[0] < b[0]) return -1;
   if (a[0] > b[0]) return 1;
   return 0;
 }
```
* https://www.codewars.com/kata/predict-your-age/train/javascript
```js
const predictAge = (a1,a2,a3,a4,a5,a6,a7,a8) => Math.floor((Math.sqrt(a1*a1 + a2*a2 + a3*a3 + a4*a4 + a5*a5 + a6*a6 + a7*a7 + a8*a8))/2);
```
