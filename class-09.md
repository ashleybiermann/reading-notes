### Topics
#### HTML/CSS
- Chapter 7: “Forms” (p.144-175)
- Chapter 14: “Lists, Tables & Forms” (pp.330-357)

#### HTML/CSS
- Chapter 6: “Events” (pp.243-292)

### HTML/CSS
Vocab
- **form** way to collect info from visitors, sent in *name/value pairs*

*Remember*
- can put a *border* on *empty cells*
- there are some CSS properties that are *specifially* use to *control appearance of **lists, tables, forms***
- *forms* are easier to use if *form controls* are *vertically aligned* using CSS

Noteworthy
- *bullet point styles*: list-style-type; list-style-image, list-style-position ... for more *examples p 333
- **Examples** of lists, tables, forms in HTML & CSS *p 352*


### JS
Vocab
- **binding** attaches an event to an ***element node***; states *which event* you are waiting to happen, and *which element* it will happen upon
- **event bubbling** event starts on the *most specific node* and *flows outward*
- **event capturing** events starts at the *least specifid node* and *flows inward*

*Remember*
- set **capturing***true* or **bubbling***false* with the **event flow boolean**

Noteworthy
- **Event Listener syntax** : `element.addEventListener('event', 'functionName, [Boolean]);`
  - the *Boolean* is the **Event Flow**, *usually* set to *false*
- the **event object** can tell you where the cursor was when the event triggered
