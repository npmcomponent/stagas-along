*This repository is a mirror of the [component](http://component.io) module [stagas/along](http://github.com/stagas/along). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/stagas-along`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

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
