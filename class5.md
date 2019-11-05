## 11/4/19

## Images

### Adding Images

The element `<img>` is the beginnings of inserting an image. It should carry the attributes `src` - which is where the pointing URL sits, `alt` - which provides a text description of the image if the image cannot be seen, and `title` - which can provide additional information about the image and is usually seen when the user hovers over the image.

Other attributes you can add to an `<img>` tag are:
- `height` specifies the height of the image in pixels
- `width` specifies the width of the image in pixels

Images can be placed before paragraphs, inside the start of a paragraph, or in the middle of paragraph. Each of which changes how the browser renders the position of the image.

### Rules for Creating Images

1. Save Images in the Right Format
2. Save Images at the Right Size
3. Use the Correct Resolution

As your website grows, it is a good idea to make a separate folder for all the images that your site uses.

On a big site, you might even want to add subfolders within the images folder.

### Stock Image Websites:
- [iStock](https://www.istockphoto.com/)
- [Getty Images](https://www.gettyimages.com/)
- [Veer](https://www.veer.com/)
- [FreeImages](https://www.freeimages.com/)
- [Fotolia](https://us.fotolia.com/)
- [Unsplash](https://unsplash.com/)
- [Lorem Ipsum](https://loremipsum.io/21-of-the-best-placeholder-image-generators/)

## Color

There are several ways to indicate colo in your CSS:
- **RGB Values** | expresses color in terms of how much red, green, and blue are used | `rgb(100, 100, 90);`
- **Hex Codes** | six-digit codes that represent the amount of red, green, and blue that are in a color | `#ee3e80;`
- **Color Names** | there are 147 predefined color names that are recognized by browsers | `DarkCyan;`

There are some good color picking tools online, like [Color Scheme Designer](https://colorschemedesigner.com/csd-3.5/) and [Adobe Color Wheel](https://color.adobe.com/create).

### Properties of Color
- **Hue** | near to the colloquial idea of a color
- **Saturation** | the amount of gray in a color
- **Brightness** | aka "value", how much black is in a color
- **Lightness** | different from brightness in that it is how much black or white is in a color
- **Alpha** | represents the transparency

In CSS3, these can be represented like this:
```css
p {
    background-color: #ffffff;
    background-color: hsla(0, 100%, 100%, 0.5);
}
```

## Text

Some quick notes about **typefaces**:
- _serif_ = has extra details on the ends of the main strokes of the letters | common ones include **Georgia**, **Times**, and **Times New Roman**
- _sans-serif_ = have straight ends to letters | common ones include **Arial**, **Verdana**, and **Helvetica**
- _monospace_ = every letter is the same width | common ones include **Courier** and **Courier New**
- _cursive_ = have joining strokes or handwriting characteristics | common ones include **Comic Sans MS** and **Monotype Corsiva**
- _fantasy_ = usually decorative fonts and are often used for titles, not designed for long bodies of text | examples include **Impact** and **Haettenschweiler**
- _weight_ = can be light, medium, bold, or black
- _style_ = can be normal, italic, or oblique
- _stretch_ = can be condensed, regular, or extended

_Link styling: Page 290-291_

## Forking vs. Branching

When a repo is _forked_, the copy of the repo exists in a separate repo that the person who forked it owns.

When repos are _branched_, then all the changes must be merged with the master. They are just "branches" of the original.

```
git checkout -b "feature1"
Switched to a new branch 'feature1'

// after changes
git checkout master
git pull origin master
```

#### [Back to Home](index.md)