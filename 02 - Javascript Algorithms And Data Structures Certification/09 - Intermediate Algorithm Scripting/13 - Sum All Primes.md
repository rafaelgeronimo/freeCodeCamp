# Sum All Primes

Sum all the prime numbers up to and including the provided number.

A prime number is defined as a number greater than one and having only two divisors, one and itself. For example, 2 is a prime number because it's only divisible by one and two.

The provided number may not be a prime.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `sumPrimes(10)` should return a number.

- `sumPrimes(10)` should return 17.

- `sumPrimes(977)` should return 73156.

---

## Solution

```js
function sumPrimes(num){
    var result = 0;
    function getPrimes(max) {
        var filter = [];
        var primes = [];
        for (let i = 2; i <= max; i++){
            if(!filter[i]){
                primes.push(i);
                for(let j = i << 1; j <= max; j += i){
                    filter[j] = true;
                }
            }
        }
        return primes;
    }

    var primes = getPrimes(num);
    for(let p = 0; p < primes.length; p++){
        result += primes[p];
    }
return result;
}

sumPrimes(10);
```