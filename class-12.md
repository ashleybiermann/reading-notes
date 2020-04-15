### Topics
#### Assorted bits of documentation
#### Articles on the Canvas API

### [Chart.js docs: You’ll be needing these!](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)
- gives instructions on how to make a chart
- provides a demo and a written example script

### [Basic usage](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)
- `canvas` element  Used like this: `<canvas id='example' width='150' height ='150'></canvas>`
- the **canvas** is going to need **context** `canvas.getContext()`
- **body onload** goes *before canvas* element. `<body onload='draw();'>`

### [Drawing shapes with canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
- if current path is *empty* after calling `beginPath();`, first path constructor is treated as `moveTo();` no matter what. **FIX:** specifically set starting position after resetting a path
- paths can be closed with `closePath();`, but it's not required

### [Applying styles and colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)
- how to : **gradient** , **transparency** , **semi transparent - 'globalAlpha** , and many more!

### [Drawing text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)
- `.fillText();` to have solid. `.strokeText();` to have outlines.