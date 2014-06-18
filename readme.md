# Button

## Sass mixin for standard button w/ width, height, roundness, and color inputs

### Mixin syntax:

```
@mixin button-rounded($width, $height, $radius, $color, $percent-dark) {
  // [mixin code]
}
```
### Input variables:

- $width = button width
- $height = button height
- $radius = border-radius (roundness)
- $color = button background-color
- $percent-dark = percentage to darken background-color on hover (Ex: '10%')

## Example

```
.[class] {
  @include button-rounded(20em, 10em, 1em, #aaa, 5%)
}
```

## Output CSS

```
.button-rounded {
  box-sizing: border-box;
  margin: 1em;
  border-radius: 1em;
  width: 20em;
  background-color: #aaa;
  line-height: 10em;
  font-size: 1em;
  text-align: center;
  text-transform: uppercase;
  color: #fff;
}
  .button-rounded:hover {
    background-color: #9d9d9d;
    cursor: pointer;
  }
```

## Installation

### Using Bower

```
$ bower install button --save
```

In your Gruntfile.js (using Grunt-Sass):

```
sass: {
  dist: {
    files: {
      'application.css': 'sass/application.scss'
    },
    options: {
      includePaths: [
        './bower_components/button'
      ]
    }
  }
}
```

In your Sass manifest:

```
@import "button";
```

### Or just copy/paste...

## Creators

### Mark Palfreeman

[Twitter](https://twitter.com/markpalfreeman)

### Gabe Pelegrin

[Github](https://github.com/skilowg)
