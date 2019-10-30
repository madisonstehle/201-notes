## 10/30/19

## Lists & Boxes

### Lists

In HTML, there are three main types of lists:
- **Ordered Lists** | `<ol></ol>` and `<li></li>` | Each item is numbered
- **Unordered Lists** | `<ul></ul>` and `<li></li>` | Each item begins with a bullet point
- **Definition Lists** | `<dl></dl>`, `<dt></dt>` - for the item being defined, and `<dd></dd>` - for the definition | Made up of a set up terms along with the definitions of those terms

_Note:_ you can nest lists inside of lists.

### Boxes

Every HTML Element has a "box" around it. That box has _three_ properties that can be adjusted through CSS to control its appearance:

1. **Border** | Separates the edge of one box from another.
2. **Margin** | Sit outsite the edge of the border.
3. **Padding** | Space between the border of a box and the content within it.

_illustration on page 307_

#### CSS Properties about Borders:

- `border-width`
- `border-style` 
- `border-color`

_pages 309-312_

Block-level components can be made to act like inline boxes and elements can be hidden with `display` and `visibility` properties.

### Loop d'Loop

#### For Loop
When you need to run code a specific number of times, use a **for** loop. The condition is usually a counter which is used to tell how many times the code should run.

```javascript
for (var i = 0; i < 10; i++) {
    document.write(i);
}
```
In the code above, the condition is a counter that that counts to ten. The result would be 0123456789.

Parts to a for loop are:
- **Initialization** (`var i = 0`): Tells the counter where to start
- **Condition** (`i < 10`): Tells it when to stop
- **Update** (`i++`): when thing loop, how do change

#### Do While dilly dilly dum While Loop

If the number of times code should run is unknown, use a **while** loop. The condition is something other than a counter and the code will loop for as long as the condition is `true`.

the **do...while** loop is similar to the **while** loop. The difference is: it will always run the statements inside the braces _at least once_, even if the condition evaluates to `false`.

#### [Back to Home](index.md)