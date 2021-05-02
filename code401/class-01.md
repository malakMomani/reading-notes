# Node Ecosystem, TDD, CI/CD

1. `Array.map()` : loop method looping inside array methods and do some processing then return somthing.

2. `Array.reduce()` : array is looping in array element and make some specific operation then return the result.

3. code:

```
const superagent = require('superagent');

superagent.get(url).then(result =>{
  console.log(result);
});

async fetch(){
  let result = await superagent.get(url);
  console.log(result);
}
```

4. promise said to the function do somthing and I will waiting the result then I'll handle it.

5. No , it can be synchoronus or Asynchoronus based on where you invoke it.
