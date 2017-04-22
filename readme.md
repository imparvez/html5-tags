## HTML 5 Features

__________

#### 1. HTML Doctype

```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>Hello World</title>
    </head>
    <body>
        <h1>Hello World</h1>
    </body>
</html>
```
doctype is required for all browsers, without it you are forcing the browsers to act in quirks mode.
doctype specifiec how the browsers should read HTML.

**Note: ** In quirk mode, browser will ignore parts of HTML and CSS standard abd tries to emulate the behaviour of older, broken browsers.

#### 2.```types``` attribute removed for Script and Links tag
Initially, we used to define type attributes for script and link tags
```
<link rel="stylesheet" href="style.css" type="text/css" />
<script type="text/javascript" src="script.js"></script>
```

Now, in HTML5 javascript and css are referred as default scripting and css language.
```
<link rel="stylesheet" href="style.css" />
<script src="script.js"></script>
```

#### 3. Semantic Tags
```div```s have not be that semantic when it comes to structuring HTML layout, this confusion is now removed with ```header``` and ```footer``` tags

```
<header>
    <h1>This is header</h1>
</header>
```
```
<footer>
    <h2>This is footer</h2>
</footer>
```

#### 4. ```<small>```  tags have been refined
```small``` tags have been refined from being used as to create sub-headings to be defined for small print text like one for copyright section.
```
<body>
  <p>This is a paragraph and <small>smaller text goes here</small></p>
</body>
```

#### 5. Figure Element
```
<img src="pic.png" alt="pic" />
<p>This is a pic</p>
```
Above code is not semantic what it is now in HTML5 using ```figure``` element
```
<figure>
    <img src="pic.png" alt="pic" />
    <figcaption>
        <p>This is a pic</p>
    </figcaption>
</figure>
```