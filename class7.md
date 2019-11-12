## 11/11/19

## Tables

As one would think, creating a table in HTML begins with a `<table>` tag. The contents are then written out row by row using `<tr>` and `<td>` tags. Table column and row headers are demonstrated by the `<th>` tag and using the `scope` attribute to indicate whether it is a column or a row header.

```html
<table>
    <tr>
        <th scope="col">Monday</th>
    </tr>
    <tr>
        <th scope="row">Today's Total</th>
        <td></td>
    </tr>
</table>
```
If you need to span rows or columns, then use the `rowspan` and `colspan` attributes and indicate with a number how many to span.

The table should be further broken into sections such as head, body, and footer using:
- `<thead>`
- `<tbody>`
- `<tfoot>`

#### [Back to Home](index.md)
