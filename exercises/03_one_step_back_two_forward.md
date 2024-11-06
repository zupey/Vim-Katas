### One step back, two forward

Change this text:

```javascript
var foo = "method("+argument1+","+argument2+")";
```

to this:

```javascript
var foo = "method(" + argument1 + "," + argument2 + ")";
```

Steps:

1. find "+" with `f+`
2. Go into insert mode with `a`
3. Type `<bs> + `
4. Leave insert mode
5. find the next "+" with `;`
6. Repeat with `.`
