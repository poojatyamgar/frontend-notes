---
marp: true

---

# Day 4

---

+ Arrays
+ for...loop  vs forEach
+ Object
+ Array of Objects
+ Dynamic element | innerHTML
+ Ajax call

---

## Dynamic Element
HTML
```html
<div id="container"> </div>
```
JS
```javascript
const newDiv = `<div> This is a new div </div>`;

document.getElementById('container).innerHTML = newDiv;
```
---

## Ajax call

const url = 'https://gist.githubusercontent.com/bhupendraparihar/b65bebc8bfda4d8b436743dcb5e9d417/raw/6f46b0d1d782e034249b5ceadab25ccf6731da04/products.json'

```javascript
fetch(url)
    .then(data => data.json())
    .then(data => {
        console.log(data);
    });
```

