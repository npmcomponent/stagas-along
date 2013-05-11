
# along

a with-alike selective method importer

basically an alternative api for [injectable](https://github.com/stagas/injectable)

## example

```js
var math = {};

math.add = function(a, b){ return a+b; }
math.sub = function(a, b){ return a-b; }
math.mul = function(a, b){ return a*b; }

along(math, function(add, sub, mul){
  var res = mul(2,add(4,sub(10,5)));
  console.log(res); // 18
});
```

## License

MIT
