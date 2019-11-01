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
