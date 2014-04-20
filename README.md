FloatLabel.js
=============

A jQuery plugin for floating form labels.

Based on a UI concept by [Matt D. Smith](https://twitter.com/mds).

[FloatLabel.js demo](http://labs.mikemitchell.co.uk/FloatLabelJS/).

Usage
-----

Add jquery.FloatLabel.css to your websites stylesheets and jquery.FloatLabel.js to your scripts.

* Add jquery.FloatLabel.js to your scripts. Example -

```html
<script src="scripts/jquery.js"></script>
<script src="scripts/jquery.FloatLabel.js"></script>
<script src="scripts/main.js"></script>
```


* Add jquery.FloatLabel.css to your stylesheets. Example -

```html
<link rel="stylesheet" href="styles/normalize.css">
<link rel="stylesheet" href="styles/jquery.FloatLabel.css">
<link rel="stylesheet" href="styles/main.css">
```

* Wrap the fields you wish to effect with your chosen class. Example -

```html
<div class="js-float-label-wrapper">
    <label for="name">Name</label>
    <input id="name" type="text">
</div>
```

* Initialise FloatLabel.js, passing the plugin your input/label wrapper class. Example -

```js
$( '.js-float-label-wrapper' ).FloatLabel();
```

Customisation
-------------

As FloatLabel.js works by using CSS classes, the animations can be tweeked within `jquery.FloatLabel.css`.

If the default classes conflict with the rest of your CSS for whatever reason, you can change them by passing in paramaters when you initialise the plugin. Don't forget to update `jquery.FloatLabel.css` with your new class names if you need to make a change.

```js
$( '.js-float-label-wrapper' ).FloatLabel({
    populatedClass : 'custom-populated-class',
	focusedClass : 'custom-focused-class'
});
```
