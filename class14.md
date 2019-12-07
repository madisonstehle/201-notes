## 12/7/19

## CSS Transitions

The `transition` property has three values that can be used to, well, transition an element.

### Fade In:

First, set intial state. Then, set the change. 
```css
.fade {
    opacity: 0.5;
}
.fade:hover {
    opacity:1;
}
```

### Change Color:
```css
.color:hover {
    background:#53a7ea;
}
```

### Grow & Shrink:
You can use `transform` to enlarge.
```css
.grow:hover {
    -webkit-transform: scale(1.3);
    -ms-transform: scale(1.3);
    transform: scale(1.3);
}
```

### Rotate:
```css
.rotate:hover {
     -webkit-transform: rotateZ(-30deg);
    -ms-transform: rotateZ(-30deg);
    transform: rotateZ(-30deg);
}
```

### Square to Circle:
You can transition a square element into a round one and vice versa with `border-radius`!
```css
.circle:hover {
    border-radius: 50%;
}
```

#### [Back to Home](index.md)