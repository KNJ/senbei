Senbei
======

## Introduction

Senbei is a jQuery plugin, which enables the browser to keep form controls' state of `value` or `checked` or `selected`, using localStorage, Cookie, or any other variable. Also, Senbei provides individual form controls with responsive functions.

## Tutorial

### Initialization

To experience Senbei easily and quickly, put the following in your application.

```html
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
</head>
<body>
	<input type="checkbox" class="senbei" name="example" value="1" checked>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
	<script src="jquery.senbei.js"></script>
</body>
</html>
```

```js
var app = senbei({
	name: 'app',
	read: 'localStorage',
	write: 'localStorage',
});
```

Then, go to the page, uncheck the checkbox, unfocus the element, close the page, and visit again.
If the checkbox is unchecked, Senbei works successfully.

Likewise, Senbei enables other types of control to hold the state. (e.g. `<input type="text">`, `<input type="radio">`, `<select>`, etc.) But don't forget to set the required attributions, `class="senbei"`, `name` and `value`.

### Attaching Senbei

To make Senbei work on specific elements, you should set the required attributions on the proper elements.

*Examples*

```
<input type="text" class="senbei" name="example-input-general" value="">
```

```
<input type="radio" class="senbei" name="example-input-radio" value="1" checked>
<input type="radio" class="senbei" name="example-input-radio" value="2">
<input type="radio" class="senbei" name="example-input-radio" value="3">
```

```
<select class="senbei" name="example-select">
	<options value="1">1</options>
	<options value="2">2</options>
	<options value="3" selected>3</options>
	<options value="4">4</options>
</select>
```
