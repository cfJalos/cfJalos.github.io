[Home page](https://cfjalos.github.io/cfJalos.github.io-reading-notes-/)


## Colors in CSS ##

### Built in Colors ###

```html
h1 {
  color: red;
}

h2 {
  color: cornflowerBlue;
}

h3 {
  color: darkOrchid;
}
```
### Hexadecimal ###

* # + String of 6 hexadecimal numbers(from 0-F)

```html
h1 {
  color: #000000;
}

h2 {
  color: #4B0082;
}

h3 {
  color: #FF1493;
}
```

### RGB ###

* 3 channels: Red, Green, and Blue.  Each ranges from 0 - 255

```css
h1 {
  color: rgb(0,255,0);
}

h2 {
  color: rgb(100, 0, 100);
}

h3 {
  color: rgb(11, 99, 150);
}
```

### RGBA ###
* Just like RGB, but with an alpha(transparency) channel.  Ranges from 0.0 - 1.0

```css
h1 {
  color: rgba(11, 99, 150, 1);
}

h2 {
  color: rgba(11, 99, 150, .6);
}

h3 {
  color: rgba(11, 99, 150, .2);
}
```
### Color and Background ###

* Use 'color' to set text color and 'background' for background color

```css
body {
  background: #95a5a6;
}

div{
  background: #3498db;
}

p {
  color: #ecf0f1;
}
```
### Background Image ###
* The background property can also set a background image

```css
body {
  background: url(http://3dprint.com/wp
   -content/uploads/2014/11/-
   Rainbow_Ocean__by_Thelma1.jpg);
}

div{
  background: rgba(0,0,0,.7);
}

p {
  color: #ecf0f1;
}
```