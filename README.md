# jest

## Installation
### CLI
```
yarn add --dev jest babel-jest
```

## Configuration
### `.eslintrc.json`
```
"env": {
  "jest": true
}
```
## Troubleshooting
### Integration with `Flow`
#### Error message
```
FAIL  src/dog.test.js
  ● Test suite failed to run

    /path/to/dog.js: Unexpected token (4:6)
        2 |
        3 | class Dog {
      > 4 |   name: string;
```
#### Solution
##### `CLI`
```
yarn add babel-preset-flow -D
```
##### `.babelrc`
```
{
  "presets": ["flow"]
}
```
