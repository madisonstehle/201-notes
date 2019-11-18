## 11/18/19

## CSS Layout (Again)

### Block-Level _vs._ Inline

**Block-Level elements** start on a new line and act as the main building blocks of any layout. Some examples are `<h1>`, `<p>`, `<ul>`, `<li>`.

**Inline elements** flow between surrounding text. Some examples are `<img>`, `<b>`, `<i>`.

You can control how much space each box takes up by setting the width and/or height, and by adjusting the borders, margins, and padding.

### Grids & Frameworks

In many types of visual art composition, designers use a grid structure to help them position items on a page and maintain consistent proportions and spacing. _See examples in our book on pages 388-392_

One particular framework is the [960 Grid System](https://960.gs/). It contains stylesheet templates for maintaining such a grid system. Other resources are [Blueprint CSS](http://blueprintcss.org/) and [Less Framework](http://lessframework.com/).

Some devs will even split their style rules into separate style sheets. So, there might be one sheet to control layout, one to control font, etc. You can link these pages by using a `@import` or a `link` method.

### _A Flashback to Class 4. . ._

As we know, elements are in boxes. Boxes can be inside of other boxes (`<p></p>` tags inside of `<div></div>` tags). CSS has positioning schemes that allow you to control the layout of the page:

- **Normal Flow**
    - every block-level element appears on a new line. This is the default behavior. `position: static;`
- **Relative Positioning**
    - moves an element from the position it would normal be in and shifts it to the top, right, bottom, or left (_these are offset properties_) of where it would have been. Once this property has been declared, use the offeset properties to indicate how far to move the element from where it would have been. `position: relative;`
- **Absolute Positioning**
    - positions an element in relation to its containing element. It is taken out of normal flow. It does not affect the surrounding elements. Again, use the offset properties to determine where the box sits. `position: absolute;`
    - **Fixed Positioning**
        - a form of _absolute positioning_ where something is placed in relation to the browser window as opposed to the containing element. Does not affect the surrounding elements.`position: fixed;`
- **Floating Elements**
    - when you float an element, it is removed from the normal flow and becomes a block-level element around which other content can flow. When using this, it is best practice to indicate the width of the element, otherwise it might be inconsistent.`float: right;`

### More About Floating

The `clear` property allows you to say that no element within the same container should touch the left or right sides of a box. It can take the values:
- `left` | The left side of the box should not touch and other elements appearing in the same containing element
- `right` | The right side of the box will not touch elements appearing in the same containing element
- `both` | Neither the left nor right sides of the box will touch elements appearing in the same containing element
- `none` | Elements _can_ touch either side.

#### [Back to Home](index.md)