## 12/7/19

## Google Teams

> The researchers eventually concluded that what distinguished the ‘‘good’’ teams from the dysfunctional groups was how teammates treated one another. The right norms, in other words, could raise a group’s collective intelligence, whereas the wrong norms could hobble a team, even if, individually, all the members were exceptionally bright.

Teamwork and collaboration is becoming more and more important to success in the workplace. The stereotypical image of "dudebro in a hoodie in a dark basement hacking away on his computer" is so far from what we see IRL. Because of the drastic need for _effective_ teams, the study of what makes a good team has risen to the forefront of some corporate research - in particular, Google. 

One thing that's found, over and over again, is that group norms can really have an impact on a group dynamic, and by extent, the groups effectiveness and productivity. The two norms that played into this the most (whether explicitly discussed as a group or not) are:
- equal distribution in speaking
- social sensitivity

> As the researchers studied the groups, however, they noticed two behaviors that all the good teams generally shared. First, on the good teams, members spoke in roughly the same proportion, a phenomenon the researchers referred to as ‘‘equality in distribution of conversational turn-taking.’’ [...] Second, the good teams all had high ‘‘average social sensitivity’’ — a fancy way of saying they were skilled at intuiting how others felt based on their tone of voice, their expressions and other nonverbal cues. 

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