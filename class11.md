## 11/25/19

## Flash, Audio, and Video

When you create a Flash file, it is saved with the extension, `.fla`; however, to use it in a website, it needs to be saved as a `.swf`.

For someone to be able to view the flash media, they need to have the Flash Player software. _Statistics commonly indicate that 98% of browsers on desktop computers have the Flash plugin installed_.

> Flash is becoming less popular. Resources like JavaScript have libraries for animations, and HTML5 has `video` and `audio` tags.

## Images

You can indicate size of images in CSS using `height` and `width` properties, and have a size-corresponding class attribute in the HTML (`small`, `medium`, `large`).

Some common image sizes:
- Small portrait | 220 x 360
- Small landscape | 330 x 210
- Feature photo | 620 x 400

You can use the `background-image` property in CSS to select an image as the background on any HTML element. By default, the image will repeat to fill the space. Some ways to work with background images are:

- `background-repeat` | can have four values:
    - `repeat` | the background image is repeated both horizontally and vertically
    - `repeat-x` | the image is repeated horizontally only
    - `repeat-y` | the image is repeated vertically only
    - `no-repeat` | the image is only shown once
- `background-attachment` | specifies whether the image should stay in one position or move as the user scrolls up and down the page. It can have values of:
    - `fixed` | stays in the same position on the page
    - `scroll` | moves up and down as the user scrolls up and down the page
- `background-position` | when the image is not being repeated, you can specify where in the browser window the image should be placed. It usually carries a pair of values:
    1. a combination of `left`, `right`, or `center` with `top`, `center`, or `bottom`
    2. a pair of pixels or percentages. Top left corner is `0% 0%`.

All of these properties' values can be shorthanded _into_ the `background` property. However, they must appear in the following order:
1. `background-color`
2. `background-image`
3. `background-repeat`
4. `background-attachment`
5. `background-position`



#### [Back to Home](index.md)