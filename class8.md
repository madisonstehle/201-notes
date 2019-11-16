## 11/16/19

## Forms

Information from a form is sent in name/value pairs. Each form control is given a name.

Forms use a `<form>` element, and will carry an `action`, `method`, and `id` attribute. The `action` attribute takes in the URL for the page on the server that will _receive_ the information in the form when it is submitted. 

The `method` attribute can have a value of `get` or `post`. The `get` method adds the value from the form are added to the end of the URL specified in the `action` attribute. It is ideal for _short forms_ and _when you are just retrieving data from the web server_. With the `post` method, the values are sent in what are know as HTTP headers. Best used for _allowing users to upload a tile_, _if the form is very long_, _contains sensitive data_, or _adds information to, or deletes information from a database_.

Forms can take in several types of input:
- **Text Input** (Single-line) | Used for a single line of text such as email addresses and names. This and other inputs can also have **form validation** by adding the `required` attribute. On any text input, you can also add placeholder text in the field by adding a `placeholder` attribute
```html
<input type="text" name="username" maxlength="30" placeholder="Enter username" />
```
- **Password Input** | Like a single line text box but it masks the characters entered.
```html
<input type="password" name="password" maxlength="30" required="required" />
```
- **Text Area** (Multi-line) | For longer areas of text, such as messages and comments
```html
<textarea name="comments">Write something here...</textarea>
```
- **Radio Buttons** | For use when a user must select one of a number of options. You can use the `checked` attribute to indicate which value, if any, should be selected when the page loads
```html
<input type="radio" name="genre" value="rock" />
```
- **Checkboxes** | When a user can select and unselect one or more options
```html
<input type="checkbox" name="service" value="spotify" checked="checked" />
```
- **Drop-down boxes** | When a user must pick one of a number of options from a list
```html
<select name="devices">
    <option value="ipod">iPod</option>
</select>
```
- **Multiple Select Box** | can be used by adding the `size` and `multiple` attributes to reflect the number of options you want to show at once. However, the way that browsers implement this isn't perfect and should be thoroughly tested.
- **Button** | gives more control as to how buttons appear. You can combine text and images.
```html
<button><img src="littleplussign.jpg" alt="add" width="10" height= "10" /> Add</button>
```
- **Date, Email, and URL Input** | by adding the `type` attribute and setting it equal to `date`, `email`, or `url`, the browser will expect those types of data.
- **Grouping Elements** | You can group related form controls together inside the `<fieldset>` element, and the `<legend>` element can caption that group.
```html
<fieldset>
    <legend>Contact Details</legend>
    <label>Email: <br />
    <input type="text" name="email" /></label>
</fieldset>
```

### Submitting Forms:
- **Submit Buttons** | To submit data from your form to another web page
```html
<input type="submit" name="subscribe" value="Subscribe" />
```
- **Image Buttons** | Similar to submit buttons but they allow you to use an image
```html
<input type="image" src="somethinghere.jpg" width="100" height="20" />
```
- **File Upload** | Allows users to upload files (e.g. images) to a website
```html
<input type="file" name="user_song" /><br />
```

#### [Back to Home](index.md)