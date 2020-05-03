### Topics
- [Shay Howe’s intro to RWD](https://learn.shayhowe.com/advanced-html-css/responsive-web-design/)
- [All About Floats](https://css-tricks.com/all-about-floats/)

#### Skim/Bookmark
- [Don’t Overthink It Grids](https://css-tricks.com/dont-overthink-it-grids/)
- [CSS Floats Explained By Riding An Escalator ](https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/)
- [SMACSS Official Documentation](http://smacss.com/)

***

- [Shay Howe’s intro to RWD](https://learn.shayhowe.com/advanced-html-css/responsive-web-design/)
- **Responsive Web Design** practice of building a website suitable to work on every device and every screen size
  - A combination of *responsive* and *adaptive* and *mobile* web design is ideal
- Three Main Components: 
  - 1. **Flexible Layout** building a grid capable of dynamic resizing. Uses ***relative units***: *percentages* and `em` units for `width`, `margin`, ` padding`, etc.
    - target size you want in pixels/ context of parent unit in pixels = result
  - 2. **Media Queries** built as an extension to media types commonly found when targeting and including styles, they provide the *ability to specify different styles for individual browser and device circumstances*
    - **Best way** to use media inquiry: `@media` inside of existing style sheet
    - >> **types** (common): `all`, `screen` (default if none specified), `print`, `tv`, `braille`, `3d-glasses`
    - **Media expression** follows type, may include features and values, which allocate to be *true* or *false*. When media feature and value  are **true**, **styles are applied**. If false, they are ignored.
    - **Logical operators**: `and`, `not`, `only`
    - When using `not` and `only`, media type may be left off. Media type is defaulted to *all*.
    - >> **features** identify what attributes or properties will be targeted within the media query expression
    - most commonly used features include `min-width` and `max-width`
    - `orientation; ` `landscape` or `portrait`
    - `aspect-ratio` and `device-aspect-ratio` specifies **width/height** pixel ratio of the targeted area or output device. `min` and `max` available
    - example: @media all and (min-device-aspect-ratio: 16/9) < width/height
    - `pixel-ratio` feature, great for *identifying high definition devices*
    -  `resolution` specifies the resolution of the output device in *pixel density* dpi dppx dpcm
  - 3. **Mobile First** technique of using styles targeted at *smaller viewports as the default styles*, then use media queries to add styles as the viewport grows
    - Generally speaking, *avoiding CSS3 shadows, gradients, transforms, and animations within mobile styles isn’t a bad idea either*
    - `viewport` meta tag, either the `height` or `width` values will define the height or width of the viewport 
    - example, with defaults <meta name="viewport" content="width=device-width">
    - `user-scalable` value to `yes` will turn on zooming <meta name="viewport" content="user-scalable=yes">
    - **Viewport Values** `viewport` meta tag will accept *individual values* as well as *multiple values*. Setting multiple values *requires comma separating* them within the `content` attribute value <meta name="viewport" content="width=device-width, initial-scale=1">




