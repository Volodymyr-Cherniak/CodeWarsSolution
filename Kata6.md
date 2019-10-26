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


