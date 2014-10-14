Senbei
======

## Introduction

Senbei is a jQuery plugin, which enables the browser to keep form controls' state of value or 'checked' or 'selected', using localStorage, Cookie, or any other variable. Also, Senbei provides individual form controls with responsive functions.

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
