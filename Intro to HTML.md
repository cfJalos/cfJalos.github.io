
[Home page](https://cfjalos.github.io/cfJalos.github.io-reading-notes-/)

## Intro to HTML ##



### History of HTML ###



* Created in 1989/1990
* Allowed publishing and exchanging of scientific  and technical documents
* Allowed electronic linking of documents via hyperlinks

### The General Rule ###



//<tagName> Some Content </tagName>

### Every HTML document we create will start with this boilerplate ###



//<!DOCTYPE html>
//<html>
//<head>
//<!-- Our metadata goes here -->
//  <title></title>
//</head>
//<body>

//<!-- Our content goes here -->

//</body>
//</html>

### Comments ###


//<!-- This is a comment.  It doesn't do anything! -->

### Common Tags ###



> //<h1>I'm a header </h1>
> //<h2>I'm a slightly smaller header </h2>
> //<h6>I'm the smallest header </h6>

> //<p>I'm a paragraph</p>

> //<button>I'm a button!</button>

> //<ul>
> //	<li>List Item 1</li>
> //	<li>List Item 2</li>
> //</ul>

> //<ol>
> //	<li>List Item 1</li>
> //	<li>List Item 2</li>
> //</ol>

* [HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

### Attributes ### 
Adding Additional Information To Tags

> //<tag name="value"></tag>
> //<img src="corgi.png">

> //<p class="selected">woof woof</p>

> //<a href="www.google.com">Click me to go to Google</a>

> //<link rel="stylesheet" type="text/css" href="style.css">

### Grouping text and Elements in a block ###



The <div> element allows you to group a set of elements together in one block level box.

The <span> element acts like an inline equivalent of the <div> element.


### NAVIGATION ###



The <navy> element is used to contain the major navigational blocks on the site such as the primary site navigation.

### Article ###



The <article> element act as a container for any selection of a page that could stand alone and potentially be syndicated.

### Aside ##



The <aside> element has two purposes, depending on whether it is inside an <article> element or not.

### Sections ###



The <section> element groups related content together and typically each section would have its own heading.

### Heading group ###

The purpose of the <hgroup> element is to groyp together a set of one or more heading through <h6> elements so that they are treated as one single heading.


### MDN Attribute Reference ###



### Images ###



> //<img src="corgi.png">

### Links ###



//<a href="url">Link Text</a

### Iframes ###



> <iframe>

An iframe is like a little window that has been cut into your page and in that window you can see another page. The term iframe is an abbreviation of inline frame.