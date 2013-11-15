# sass-triangle

Simple mixin for creating triangles arrows using the [cross-browser CSS
triangles method](http://davidwalsh.name/css-triangles). 

## Syntax

    @mixin arrow($direction, $size, $color)

## Usage

To create a simple 10px tooltip with triangle on top:

    $size: 10px

    .tooltip
      background: white
      color: black
      position: relative

      &:before
        position: absolute
        top: -$size
        left: 50%
        margin-left: -($size / 2)
        +arrow(top, 10px, white)
