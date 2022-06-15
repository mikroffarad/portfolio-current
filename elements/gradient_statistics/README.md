# gradient_statistics
https://mikroffarad.github.io/gradient_statistics/


```javascript
function digital_root(n) {
  var sum;

  var digit_sum = function(num) {
    sum = 0;
    for (i = 0; i < `${num}`.length; i++) {
      sum += +`${num}`[i]
    }
    console.log(sum)
    return sum
  }
  digit_sum(n)

  for (let i; `${sum}`.length !== 1; i++) {
    digit_sum(sum)
  }
  return sum
}

digital_root(493193)  
```
