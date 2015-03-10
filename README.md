# DST Apple Safari Bug Test

This repo exists to test a bug in Safari exhibited by the following code:

```js
var d1 = new Date("2015-03-08T10:59:44.000Z");
var d2 = new Date(d1.getTime());
d1.setHours(d1.getHours());
document.write(d1.getTime() === d2.getTime() ? '<h1>PASS</h1>' : '<h1>FAIL</h1>');
```

Go to https://eventualbuddha.github.io/dst-apple-safari-bug-test to try it in your browser.