### Topics Covered
#### JS book:
- Chapter 3: “Object Literals” (pp.100-105)
- Chapter 5: “Document Object Model” (pp.183-242)

Vocab
- **object literal** creating an object without the keyword *new*
- **object** contains properties, methods, and keys
- **property** variable in an object
- **method** function in an object
- **key** name of a property in an object
- **value** what is contained in the key

- **D**ocument **O**bject **M**odel  model of a webpage ***DOM***
- **DOM Queries** methods that find elements in a **DOM tree**
- **node** location of something on **DOM tree**
  - 4 types:
    - 1. document
    - 2. element
    - 3. attribute
    - 4. text
- **NodeList** collection of element nodes, each is given an *index number* start with 0
  - *look* like an array, but are **not**
  - type of **object** called a **collection**

*Remember*
- Need to use an *element* more than once? Store it in a variable!
  - *example*  var itemOne = getElementById('one');
  - *best* to **store elements** using **array syntax** *example p199* ... var firstItem = elements[0];
- Need to *repeat actions* for an *entire* nodelist? **loop** through the node. *example p 204/5*
- **No two** elements can *share the same value* for their **id attribute**
- **element nodes** can be selected by *id* or *class* attributes, *tag name*, or by using *CSS selector syntax*git


Noteworthy
- *example*  var variableName = object.propertyName; ____ *or*____ var variableName =object.methodName();
  - **.**   is the *member operator*
- *example*  var anotherVariable = object['propertyName']; *or* var anotherVariable = object['methodName']();
- *example using **DOM** to **select individual element*** document.getElementById('one'); ____ *document* is the **object**
- Good *example p195* to show how getElementById() is used in JS
- **Adding / Removing HTML Contnent** 2 ways: 1) *innerHTML* - best for updating entire fragments; 2) *DOM manipulation* - best for targeting individual nodes in DOM tree
- Once you have an element node, you can use other properties and methods to access and change its attributes *example p232*
