# docstrings

> Interpret a string literal at the beginning of a function as its
> documentation.


## Usage

```js
var doc = require('docstrings')

function foo () {
  "returns foo"
  return 'foo'
}

console.log(doc(foo))
```

This will output

```
returns foo
```

## API

```js
var doc = require('docstrings')
```

### doc(func)

Returns a string matching the string literal at the beginning of a function.
Matches `""` and `''` literals as well as template strings.

## Install

With [npm](https://npmjs.org/) installed, run

```
$ npm install docstrings
```

## Acknowledgments

docstrings was inspired by clojure's approach to documenting functions.

## License

ISC

