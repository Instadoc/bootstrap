---
name: Interactive
category: Examples
---

Lodash
---
```reverse.html hidden
<script src="https://cdn.jsdelivr.net/npm/lodash@4.17.4/lodash.min.js"></script>
```
```reverse.html
<label>Input:</label>
<input class="in" type="text" value="Hello, world">

<label>Reverse:</label>
<input class="out" type="text" readonly></sum>
```
```reverse.js
var output = document.querySelector('.out');
var input = document.querySelector('.in');

reverse();
input.addEventListener('keyup', reverse);

function reverse() {
	output.value = _(input.value).split('').reverse().join('');
}
```
```reverse.css hidden
label { padding-top: 20px }
```
