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

