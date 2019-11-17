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
