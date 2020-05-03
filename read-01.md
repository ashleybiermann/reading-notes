### Topics
- [Shay Howe’s intro to RWD](https://learn.shayhowe.com/advanced-html-css/responsive-web-design/)
- [All About Floats](https://css-tricks.com/all-about-floats/)

#### Skim/Bookmark
- [Don’t Overthink It Grids](https://css-tricks.com/dont-overthink-it-grids/)
- [CSS Floats Explained By Riding An Escalator ](https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/)
- [SMACSS Official Documentation](http://smacss.com/)

***

## [Shay Howe’s intro to RWD](https://learn.shayhowe.com/advanced-html-css/responsive-web-design/)
- **Responsive Web Design** practice of building a website suitable to work on every device and every screen size
  - A combination of *responsive* and *adaptive* and *mobile* web design is ideal
- Three Main Components: 
  - **Flexible Layout** building a grid capable of dynamic resizing. Uses ***relative units***: *percentages* and `em` units for `width`, `margin`, ` padding`, etc.
    - target size you want in pixels/ context of parent unit in pixels = result
  - **Media Queries** built as an extension to media types commonly found when targeting and including styles, they provide the *ability to specify different styles for individual browser and device circumstances*
    - **Best way** to use media inquiry: `@media` inside of existing style sheet
    - > **types** (common): `all`, `screen` (default if none specified), `print`, `tv`, `braille`, `3d-glasses`
    - **Media expression** follows type, may include features and values, which allocate to be *true* or *false*. When media feature and value  are **true**, **styles are applied**. If false, they are ignored.
    - **Logical operators**: `and`, `not`, `only`
    - When using `not` and `only`, media type may be left off. Media type is defaulted to *all*.
    - > **features** identify what attributes or properties will be targeted within the media query expression
    - most commonly used features include `min-width` and `max-width`
    - `orientation; ` `landscape` or `portrait`
    - `aspect-ratio` and `device-aspect-ratio` specifies **width/height** pixel ratio of the targeted area or output device. `min` and `max` available
    - example: @media all and (min-device-aspect-ratio: 16/9) < width/height
    - `pixel-ratio` feature, great for *identifying high definition devices*
    -  `resolution` specifies the resolution of the output device in *pixel density* dpi dppx dpcm
  - **Mobile First** technique of using styles targeted at *smaller viewports as the default styles*, then use media queries to add styles as the viewport grows
    - Generally speaking, *avoiding CSS3 shadows, gradients, transforms, and animations within mobile styles isn’t a bad idea either*
    - `viewport` meta tag, either the `height` or `width` values will define the height or width of the viewport 
    - example, with defaults <meta name="viewport" content="width=device-width">
    - `user-scalable` value to `yes` will turn on zooming <meta name="viewport" content="user-scalable=yes">
    - **Viewport Values** `viewport` meta tag will accept *individual values* as well as *multiple values*. Setting multiple values *requires comma separating* them within the `content` attribute value <meta name="viewport" content="width=device-width, initial-scale=1">
    - **CSS Viewport Rule** make it an @ rule in CSS `@viewport { }`
- **Flexible Media** make media scalable
  - `iframe` and embedded media (such as YouTube) cannot use `max-width` > use a work-around
  - Use **absolute positioning** within parent element, parent element needs `width` of `100%` and `height` of `0`to trigger `hasLayout` mechanism ... for more details, see website

***

## [All About Floats](https://css-tricks.com/all-about-floats/)
- `Absolute`ly positioned page elements are removed from the flow of the webpage
  > will *not* affect the position of other elements, and other elements will *not* affect them
- **`Float`ed elements** remain a *part of the flow* of the web page
- **4 float values** Left, Right, None, Inherit (*assumes same value as parent*)
- Float’s sister property is **`clear: `** *clears* floats coming from a direction
- **4 clear values** both, left, right, none (none is default and typically unnecessary)
- **The Great Collapse** If parent element contained *nothing but floated elements*, the height of it would *literally collapse to nothing*
> **Collapsing** *almost always* needs to be **dealt with** to prevent strange layout and cross-browser problems
  - fix it by clearing the float **after** the floated elements in the container but **before** the close of the container

**Techniques for clearning floats**
- **`clear: both;`** in situations where you always know that the succeeding element will be
- **Empty Div Method** `<div style="clear: both;"> </div>`
- **Overflow Method** relies on setting the `overflow` property on a parent element
- **Easy Clearing Method** uses pseudo selector `:after` to clear floats. *example* on website `.clearfixorwhatever:after { }`

**Problems with Floats**
- **pushdown** symptom of an *element inside a floated item* being *wider* than the float itself (typically an image)
> Quick fix: `overflow: hidden`
- **double margin bug** if you apply a margin in the same direction as the float
> Quick fix: set `display: inline` on the float
- **3px job** when text that is up next to a floated element is mysteriously kicked away by 3px like a weird forcefield around the float
> Quick fix: set a width or height on the affected text
- **bottom margin bug** when, if a floated parent has floated children inside it, bottom margin on those children is ignored by the parent. 
> Quick fix: use bottom padding on parent instead