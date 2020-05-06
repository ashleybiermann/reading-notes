##  jQuery, Events, and The DOM
- JavaScript and jQuery p. 293-301, 306-331, 354-357
- [6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)
Bookmark/Skim
- JavaScript and jQuery book by Jon Duckett pages 332-335
- JavaScript and jQuery book by Jon Duckett pages 302-305

### jQuery, Events, and The DOM
- **jQuery** JS file you include in webpages. Lets you *find elements using CSS-style selectors* and manipulate them. Stores a **reference** to corresponding node, does not copy them.
- **matched set** or **jquery selection** a *jQuery object* that is returned when you select one or more elements
  - Each node has an **index number**
- jQuery can **get** and **set** information
  - Trying to **get** information from a jQuery *selection that holds more than one element*? It will ***retrieve only the info from the first** element* in the matched set
  - Trying to **set** information from a jQuery *selection that holds more than one elemetn*? It will ***update all** of the elements* in the matched set
  > **implicit iteration** ability to update all of the elements in the jQuerty selection *looping*
- A variable reference to the jQuery object (holding a reference to nodes) can be used `$someNameHere`
- **chaining** using dot notation to have *multiple methods* act on the same selection of elements
> methods that **update** can be chained
> methods that **retrieve** *cannot* be chained
- `.ready()` method checks that te page is ready for code to work with
- `$(function() { //script here});` shorthand 
- **CDN** Content Delivery Network. series of servers spread out around the world designed to serve static files (HTML, CSS, JS, images, audio, video) very quickly
  - **fallback** including a stored version of jQuery on your own servers in case it doesn't load from another remote server
- **protocol relative URL** when a script starts with two forward slashed `script src="//...`
- **CDN script placement** *before the `/body` tag n