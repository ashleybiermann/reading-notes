### Topic
#### Web 
[“The Past, Present, and Future of Local Storage for Web Applications”](http://diveinto.html5doctor.com/storage.html)

- 'If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.'
- **Cookies** 'to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.'
- HTML5 storage stores key/values locally within client browser that persists, but is never transmitted over the web
  - the named **key** is always a **string**, but can actually hold any datatpe supported by JS
  - use `parseInt()` or `parseFloat()` or etc. to return a different data type
  - `localStorage.setItem()` and `.getItem()` to interact