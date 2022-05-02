# SCSS => CSS-3
# SASS => CSS

> Sass is a CSS pre-processor.
> Sass stands for Syntactically Awesome Stylesheet
> Sass reduces repetition of CSS and therefore saves time.

# declare the Variables : $variablename: value;
```scss
$bgcolor: cyan;
$textcolor: red;
$fontsize: 10px;

## using the variables 
body {
  background-color: $bgcolor;
  color: $textcolor;
  font-size: $fontsize;
}
```

# global variables
```scss
$myColor: red;

h1 {
  $myColor: green !global;
  color: $myColor;
}

p {
  color: $myColor;
}
```

>  Global variables should be defined outside any rules. It could be wise to define all global variables in its own file, named "_globals.scss", and include the file with the @include keyword.

# nesting 
```scss
nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }
  li {
    display: inline-block;
  }
  a {
    display: block;
    padding: 6px 12px;
    text-decoration: none;
  }
}
```
### way2
```scss
font: {
  family: Helvetica, sans-serif;
  size: 18px;
  weight: bold;
}

text: {
  align: center;
  transform: lowercase;
  overflow: hidden;
}
```
