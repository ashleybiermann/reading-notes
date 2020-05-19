## EJS Partials
[EJS Partials](https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433)
[Watch EJS tutorial from WalkThroughCode on YouTube, Video 7, Partials](https://www.youtube.com/watch?v=3_xEEH4fTEk&t=0s&index=7&list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

### [EJS Partials](https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433)
- **Partials** reusable bundle of code contained in a file
- native to EJS
- makes it easier to maintain large sites with repetative info
- *same 'something'* from page to page? Make it a partial! ex: nav bar or footer
- goes in `views/partials/` directory, make it an `.ejs` file
  - *Remember* EJS included in HTML-ish places is surrounded by `<% %>` delimiters 
- `<%- include( PARTIAL_FILE ) %>` ***this** goes in the .ejs file!*
