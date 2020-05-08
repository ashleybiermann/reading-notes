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
Setting up a grid size `grid-template-columns: ` `grid-template-rows: `can use percentages `%`, pixels `px`, ems `em`, fractionals `fr` *and mix them together, too*
> example `grid-template-columns: 100px 3em 40% 2fr;` **no commas**
- `grid-template` combines template-rows and template-columns
  > `grid-template: 50% 50% / 200px;` will create a grid with two rows that are 50% each, and one column that is 200 pixels wide
- **fractional unit** 1fr and 3fr gives 4 total units, 1/4 and 3/4 a piece
> if other units are also used, fr will divvy up what's left
-can also use a `repeat: ;` function `grid-template-columns: repeat(5, 20% );`
**columns** movement here affects ***horizontal*** movement on page
**rows** movement here affects ***vertical***
- `grid-column-start: 3;` starts at 3rd vertical gride line
- `grid-column-end: 4;` ends at the **beginning** of the 4th **grid line** *doesn't fill the 4th grid square!*
- `-start: ` does *not* need to be a larger value than `-end: ` 
- **Negative vales** to start *from the right*
  - **`-end: `** 
  > makes `: -1;` the rightmost grid line 
  - **`-start: `**
  > makes `: -2;` (yes, 2) start at the rightmost grid line 
  > -1 starts at the right but keeps going right... off the grid
- `-span: ` only accepts positive values
>`-end: 2;` spans a width of 2 units
>`-start: 2` references end and spans 2 units back
- `grid-column: ` shorthands start and end `grid-column: 2 / 4;`
All those ways to use columns? Go ahead and do it for rows, too!
- `grid-area: 1 / 2 / 3 / 4;` combines `row` and `column` 
> 1 = row-start
> 2 = column-start
> 3 = row-end
> 4 = column-end
**Order** by default, grid items have an `order: ;` value of '0', automatically placed according to their order in the source code
- can be changed, set to positive or negative, similar to `z-index`
