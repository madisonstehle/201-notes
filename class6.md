## 11/9/19

## Object Literals and the DOM

> Understanding the problem is the most critical piece to the equation. It is very difficult to solve a problem before you know the question.

### Objects

Objects group together a set of variables and functions to create a model of a something you would recognize from the real world.

In an object, variables become known as _properties_ and functions become known as _methods_

Properties have names and values. These combinations are called _key/value pairs_. To create an object, the **literal notation** (which is the easiest and most popular way) looks like this:

```javascript
var hotel = {
    name: 'Quay',
    rooms: 40,
    booked: 25,
    checkAvailability: function(){
        return this.rooms - this.booked;
    }
};
```

And objects can be accessed by **dot notation**:

```javascript
var hotelName = hotel.name;
var roomsFree = hotel.checkAvailability();
```

### Document Object Model (DOM)

Basically, the DOM is the model of a web page. This model, the **DOM Tree** consists of four main types of _nodes_:

- **Document Node** |  The top of the DOM tree. Represents the entire page. 
- **Element Node** | Describe the structure of an HTML page.
- **Attribute Node** | Part of the element.
- **Text Node** | Cannot have child elements

#### Accessing Elements

- `getElementById()` | uses the the value of the **id** attribute
- `querySelector()` | uses a CSS selector and returns first matching element
- `getElementsByClassName()` | selects all elements that have a specific value for their class attribute
- `getElementsByTagName()` | selects all elements thtat have the specified tag name
- `querySelectorAll()` | uses a CSS selector to select all matching elements
- `parentNode` | selects the parent of the current element node
- `previousSibling / nextSibling` | selects the previous or next sibling from the DOM tree
- `firstChild / lastChild` | selects the first of last child of the current element

#### Working with the Elements

- `nodeValue` | this property lets you access or update contents of a text node
- `innerHTML` | allows access to the child elements and text content
- `textContent` | just the text content

There are several methods that let you create nodes, add nodes, or remove nodes. This is called _DOM manipulation_:

- `createElement()`
- `createTextNode()`
- `appendChild() / removeChild()`

For attributes:

- `hasAttribute()` | checks if an attribute exists
- `getAttribute()` | gets its value
- `setAttribute()` | updates the value
- `removeAttribute()` | removes an attribute

## Examples

### HTML:
```html
<body>
    <ul id="firstAndPike"></ul>
    <script src="app.js"></script>
</body>
```

### JavaScript:
```javascript
// store the html point of contact
var firstAndPikeElement = document.getElementById('firstAndPike');

// create the element
var liEl = document.createElement('li');

// give the element content
liEl.textContent = 'proof of life';

// append to the DOM
firstAndPikeElement.appendChild(liEl);
```

### For Salmon Cookies:
```javaScript
var hours = ['6am', '7am', '8am', '9am', '10am', '11am', '12pm', '1pm', '2pm', '3pm', '4pm', '5pm', '6pm', '7pm', '8pm'];

var firstAndPikeShop = {
    minCustomersEachHour: 23,
    maxCustomersEachHour: 65,
    averageCookiesPerCustomer: 6.3,
    customersEachHour: [],
    cookiesEachHour: [],
    totalCookiesForTheDay: 0,

    render: function() {
        for (var i = 0; i < hours.length; i++) {
            // create element
            var liEl = document.createElement('li');
            // give element content
            liEl.textContent = `$hours[i] Cookies: 34`;
            // append to DOM
            firstAndPikeElement.appendChild(liEl);
        }
    }

    randomNumber: function() {
        return Math.floor(Math.random() * (max - min)) + min;
    }
};

// in browser console, test with:
firstAndPikeShop.render();
```

#### [Back to Home](index.md)

