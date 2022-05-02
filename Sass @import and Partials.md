
> Sass keeps the CSS code DRY (Don't Repeat Yourself). One way to write DRY code is to keep related code in separate files.


> The CSS @import directive has a major drawback due to performance issues; it creates an extra HTTP request each time you call it. However, the Sass @import directive includes the file in the CSS; so no extra HTTP call is required at runtime!

```scss
@import "filename";
```
> You do not need to specify a file extension, Sass automatically assumes that you mean a .sass or .scss file. You can also import CSS files

# Sass Partials

> Sass has a mechanism for this: If you start the filename with an underscore, Sass will not transpile it. Files named this way are called partials in Sass.
```scss
 _filename;
 ```
