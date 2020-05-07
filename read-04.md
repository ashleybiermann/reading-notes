### Responsive Web Design and Regular Expressions
-[CSS Grid Garden](https://cssgridgarden.com/)

#### Bookmark/Skim
-[RegExr](https://regexr.com/)
-[Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)
-[Regex 101](https://regex101.com/)
-[CSS Grid Reference](https://css-tricks.com/snippets/css/complete-guide-grid/)
-[Responsive design with CSS Grid](https://medium.com/samsung-internet-dev/common-responsive-layouts-with-css-grid-and-some-without-245a862f48df)

* * *

### [CSS Grid Garden](https://cssgridgarden.com/)
- `grid-column-start: 3;` starts at 3rd vertical gride line
- `grid-column-end: 4;` ends at the **beginning** of the 4th **grid line** *doesn't fill the 4th grid square!*
- `-start` does *not* need to be a larger value than `-end` 
- Negative vales to start from opposide side
  - **`-end`** use a **negative** to start the grid count *from the right* 
  > makes `: -1;` the rightmost grid line 
  - **`-start`** use a **negative** to start the grid count *from the right*
  > makes `: -2;` (yes, 2) start at the rightmost grid line (*-1 starts at the right but keeps going right... off the grid)