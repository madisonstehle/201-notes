## 10/28/19

## HTML, CSS, JS

### Semantic HTML Tags Cheat Sheet: Beyond `<div>`

- `<sup></sup>` contains characters that should be superscript
- `<sub></sub>` contains characters that should be subscript
- `<br />` adds a line break
- `<hr />` adds a horizontal rule
- `<strong></strong>` indicates that the contents have strong importance (usually displays as bolded text)
- `<em></em>` indicates that the contents subtly change the meaning of a sentence (usually displays as italics)
- `<abbr></abbr>` used for abbreviations or acronyms
- `<cite></cite>` indicates where the citation is from
- `<dfn></dfn>` used to indicate the defining instance of a new term
- `<address></address>` contains contact details for the author of the page (physical address/phone number/email address/etc.)
- `<s></s>` indicates that something is no long relevant, but should not be deleted (rendered with a line through content)

### CSS: Cascading Style Sheets

In CSS Syntax, there are _selectors_ and _declarations_.
In the example below, `p` is the selector (targeting an element) and `{color: #665544;}` is the declaration. 

Declarations are made up of two parts: _properties_ (for example, `font-family`) and _values_ (`Arial`).
```css
body {
    font-family: Arial, Verdana, sans-serif;
    }
h1, h2 {
    color: #ee3e80;
    }
p {
    color: #665544;
    }
```
_See a table for types of CSS Selectors on page 238 of your book._

To link **external** CSS to your HTML, you put the link in your HTML `<head>` tag:
```html
<head>
 <title>Using External CSS</title>
 <link href="css/styles.css" type="text/css"
 rel="stylesheet" />
</head>
```
#### The _Cascading_ Part

If written CSS rules conflict:
>the more specific rule will take precedence over more general ones.

Some attributes can be 'inherited' by child elements from parent elements. Some examples are `font-family` and `color`.
Other attributes **do not** get inherited, such as `background-color` and `border` properties.

#### Browser Quirks

CSS can sometimes manifest differently on different computers, so instead of checking your site on a bunch of individual browsers, you can use some online tools to check what they look like!
- BrowserCam.com
- BrowserLab.Adobe.com
- BrowserShots.org
- CrossBrowserTesting.com

If you come accross a CSS bug, you can research and/or check these sites:
- PositionIsEverything.net
- QuirksMode.org

### JavaScript: The Interactive Layer

Oftentimes, when a user triggers an event, JS runs a script that makes something happen to make the website feel more interactive.

That being said, to make the thing happen, the computer needs a detailed script, or series of steps that tell it what to do and when to do it. So, before beginning to write your JS, it is good to know **what your goal is** and **make a flowchart of how to get there**.

**There are two types of expressions**:

1. Expressions that assign a value to a variable. For example, `var color = 'beige';`
2. Expressions that use two or more values to _return_ a single value, or `var area = 3 * 2;`

To make these expressions work, programmers use **operators**. Examples are:
- Assignment Operators (`color = 'beige';`)
- Arithmetic Operators (`area = 3 * 2;`), _pg 76_
- String Operators (`greeting = 'Hi ' + 'Molly';`)
- Comparison Operators (`buy = 3 > 5;`)
- Logical Operators (`buy = (5 > 3) && (2 < 4);`)

In other JavaScript news, you can create **functions** that let you groups statements together to perform a specific task. You can even REUSE the function by _calling_ it.

```js
function sayHello() {
    document.write('Hello!');
}
```
When functions require more information to run, you can do that with **parameters** and **arguments**. The parameters in the example below are `(width, height)`.
```js
function getArea(width, height) {
    return width * height;
}
```
When you _call_ the function, you fill in the required information or _parameters_: `getArea(3, 5);`.

#### An Array
Arrays are special types of variables that store a _list of values_. For example, a shopping list!

```javascript
var colors;
colors = ['white', 'black', 'custom'];
```

These values in the array are given a number called an **index**. The index starts at **0** with the first value in the array. So, in the example above, for the value `'black'`, the index is **1**. 

To retrieve a value, you call it with the variable name with the index. i.e. `colors[2];`.

#### Comparison Operators

- `==` _is equal to_ | Compares two values to see if they are the same.
- `===` _is strictly equal to_ | Compates two values to check that both the data type AND value are the same.
- `!=` _is not equal to_ | compares values to see if they are not the same.
- `=!` _strict not equal to_ | compares two values to check that both the data type and value are not the same.
- `>` _greater than_ | checks is the number on the left is greater than the number on the right.
- `<` _less than_ | checks if the number on the left is less than the number on the right.
- `>=` _greater than or equal to_ | checks if the number on the left is greater than or equal to the number on the right.
- `<=` _less than or equal to_ | checks if the number on the left is less than or equal to the number on the right.

#### Logical Operators

- `&&` _logical and_ | tests more than one condition
- `||` _logical or_ | tests at least one condition
- `!` _logical not_ | takes a single Boolean value and inverts it

#### [Back to Home](index.md)