 
 # mixin
 
  Hyphens and underscores are considered to be the same. This means that @mixin important-text { } and @mixin important_text { } are considered as the same mixin!
 
 ```scss
 @mixin important-text {
  color: red;
  font-size: 25px;
  font-weight: bold;
  border: 1px solid blue;
}

.danger {
  @include important-text;
  background-color: green;
}
 ```
 
 # passing variable to a mixin
 
 ```scss
 /* Define mixin with two arguments */
@mixin bordered($color, $width) { //you can also define the default values 
  border: $width solid $color;
}

.myArticle {
  @include bordered(blue, 1px);  // Call mixin with two values
}

.myNotes {
  @include bordered(red, 2px); // Call mixin with two values
}
 ```
 
 # Using a Mixin For Vendor Prefixes
 
 ````scss
 @mixin transform($property) {
  -webkit-transform: $property;
  -ms-transform: $property;
  transform: $property;
}

.myBox {
  @include transform(rotate(20deg));
}
 ```
