## 11/2/19

## Links

Links are created using the `<a></a>` tag. In the opening anchor tag, you create an `href` attribute containing the link itself.

Linking to a different website, the value of href would be the full web address for the site. This is known as the **absolute** URL.

When you are linking to other pages in the same site, you can use a shorthand **relative** URL, because you do not need to specifify the domain name.

_By the way_, URL stands for **Uniform Resource Locator**.

To create a link that starts up the user's email and addresses an email to a specified address, instead of using an href attribute, you would use a `mailto:` attribute.

If you want a link to open a new window on the browser, then you would add a another attribute and value to the link: `target="_blank"`.

To link sections on the same page, give those sections `id`s and reference the id in the `href`.

Likewise, you can add a link that takes you too a specific section in an external website. the `href` attribute just needs to include a section `id` at the end of the URL.

## Layout

As we know, elements are in boxes. Boxes can be inside of other boxes (`<p></p>` tags inside of `<div></div>` tags). CSS has positioning schemes that allow you to control the layout of the page:

- Normal Flow
    - every block-level element appears on a new line. This is the default behavior. `position: static;`
- Relative Positioning
    - moves an element from the position it would normal be in and shifts it to the top, right, bottom, or left (_these are offset properties_) of where it would have been. Once this property has been declared, use the offeset properties to indicate how far to move the element from where it would have been. `position: relative;`
- Absolute Positioning
    - positions an element in relation to its containing element. It is taken out of normal flow. It does not affect the surrounding elements. Again, use the offset properties to determine where the box sits. `position: absolute;`
- Fixed Positioning
    - a form of _absolute positioning_ where something is placed in relation to the browser window as opposed to the containing element. Does not affect the surrounding elements.`position: fixed;`
- Floating Elements
    - when you float an element, it is removed from the normal flow and becomes a block-level element around which other content can flow. When using this, it is best practice to indicate the width of the element, otherwise it might be inconsistent.`float: right;`

When you move an element from normal flow, boxes can overlap. You can control which box appears on top with the propert `z-index`. This property is assigned a number value. A box with a value of 5 would sit under one with a value of 10. 

Another thing to keep in mind is the `clear` property. It allows you to say that no element (within the same containing element) should touch the left or right-hand sides of a box. It can take the values `left`, `right`, `both`, or `none`.

There is a problem that sometimes happens with floating elements. If a containing element _only_ contains floated elements, some browsers, will treat it as if it is zero pixels tall. This can be fixed using the `overflow` and `width` properties!

## Function Examples

Example 1:
```JavaScript
function makeSandwich (meat, cheese, bread) {
    var newSandwich = 'Here is your ' + meat + ' and ' + cheese + ' on ' + bread + ' sandwich!';
    return newSandwich;
}
var mySandwich = makeSandwich('tempeh', 'daiya', 'sourdough');
console.log(mySandwich);
```

Example 2:
```JavaScript
// cat html pseudocode:
// inputs (parameters): name, image, description
// work: insert name, image, description into the text.
// outputs (return values): an html article w/ name, image, description.

function createCatArticle(name, image, description) {
    var catArticle = '<article>' + 
        '<h3>' + name + '</h3>' +
        '<img src="' + image + '">' +
        '<p>' + description + '</p>' +
        '</article>';
    return catArticle;
}

var wantsToAdd = prompt('Hey there! Do you want to add a cat?');
if (wantsToAdd === 'yes') {
    var catName = prompt('What is the name of the cat?');
    var catImage = prompt('What is the name of the file containing the iamage?');
    var catDescription = prompt('What is the description of the cat?');
    var newCat = createCatArticle(catName, catImage, catDescription);
    document.write(newCat);
}
```

Example 3:
```JavaScript
// Red Light Loop
var lightColor = prompt('What color is the light?');

while (lightColor === 'red') {
    console.log('Stop the car!');
    lightColor = prompt('What color is the light?');
} 

console.log('Goooooo!');
```

Examples 4 and 5:
```JavaScript
// Push Up Loop
var pushupCounter = 0;

while (pushupCounter < 10) {
    console.log('Do a pushup!');
    // pushupCounter = pushupCounter + 1;
    // pushupCounter += 1;
    pushupCounter++;
}

console.log('You did the pushups!')

// Shorthand: For Loops!
for (var pushupCounter = 0; pushupCounter < 10; pushupCounter++) {
    console.log('Do a pushup!');
    console.log('I have done ' + pushupCounter + ' pushups!');
    }

for (var i = 0; i < 10; i++) {
    console.log('Do a pushup!');
    console.log('I have done ' + i + ' pushups!');
}
```

#### [Back to Home](index.md)