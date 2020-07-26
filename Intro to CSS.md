[Home page](https://cfjalos.github.io/cfJalos.github.io-reading-notes-/)


## INTRO TO CSS ##


### What is CSS? ###

* Cascading Style Sheets

### The General Rule ###

```css
selector {
  property: value;
  anotherProperty: value;
}
```
### Where do we write our styles? ###

* Inline

```css
<h3 style="color: pink;">blah blah blah </h3>
<h3 style="color: pink;">knock knock </h3>
<p style="color: yellow;">blah blah blah </p>
```

* Style

```css
<html>
<head>
    <title>About Rusty</title>
    <style type="text/css">
        li {
      color: red;
  }
    </style>
</head>
```

*CSS in a separate CSS file
Using the <link> tag

```css
<!DOCTYPE html>
<html>
<head>
    <title>Demo Page</title>
    <link rel="stylesheet" type="text/css" href="app.css">
</head>
<body>
  
</body>
</html>
```

In our app.css file:

```css
h1 {
  color: purple;
}

h3 {
 color: pink;
}
```

### Closing Tags ###
```html
<h1>I need a closing tag </h1>

<p>Me too!</p>
```

### Self-Closing Tags ###

```html
<!-- No closing tag or inner text needed -->

<img src="corgi.png">

<link href="style.css">

<!-- Don't worry about what these tags do yet -->
```

### Attributes ###

```html
<tag name="value"></tag>

<img src="corgi.png">

<p class="selected">woof woof</p>

<a href="www.google.com">Click me to go to Google</a>

<link rel="stylesheet" type="text/css" href="style.css">
```


