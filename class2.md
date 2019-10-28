## 10/28/19

## HTML, CSS, JS

### Semantic HTML Tags Cheat Sheet: Beyond <div>
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

#### [Back to Home](index.md)