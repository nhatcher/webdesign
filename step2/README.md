# A simple webpage with CSS and a image

In the HTML file we have a new line in the `head` part:

```html
<link rel="stylesheet" href="style.css">
```

This instructs the browser to load the file `style.css` and use it to style the document.
Note that the name of the file is entirely your coice.

The `link` tag uses two properties, the `rel` property is saying it is a style sheet and the `href` property.
This second one contains the route to the file.
Might be somewhere in your server or somewhere else. More on that later.

Note how I have surounded some text with `span` elements.

```html
<span class="jelena-it">NOT</span>
```

And here we are using a very important property of almos every tag: `class` property.

The class property of a tag is just a name. In this case `jelena-it`.
That is a name chosen by you. You can pick any name. By itself it doesn't do anything.
Doens't change anything, the page will look exactly the same with or without that.

It is used later in CSS. Someone will say:

Hey folks I want all the text contained in span elements of class "jelena-it" to be  red.

Or blue, or have a border or a background, or be upsidedown, or a padding, marging, or display in a new line.
Or change the color if you hover over them with the mouse. Posibilities are endless.

If you look at the file `style.css` you will see the code:

```css
.jelena-it {
    font-style: italic;
}
```

This means: hey browser find all elements of class `jelena-it` and show them in italic.
Note that it starts with a dot (".") as in `.jelena-it`.

There is another example:

```css
.jelena-bold {
    color: brown;
    font-weight: bold;
}
```

This finds anything in the page of class `.jelena-bold`, set it bold and uses a brown color.
We normally don't use color names for colors. There are way too many colors, so we need to use a better schema.
More on that later.
The power of this is that you might have hundreds of elements of the class `.jelena-bold`, you can change the look and feel of all of them at the same time.

Another example of css is also given here:

```css
div {
    background-color: #ffff00;
    width: 300px;
    padding: 20px;
    text-align: center;
}
```

It does not start with a dot. This says: 

In all `div`s in the page (all alements or tags called `div`), please set a background color of `#ffff00`,
make them of 300 pixels width set a padding around the elements of 20 pixels.
And align every text inside the `div` to the center. Thank your very much you are a doll!

Now, we can *select* elements by their tag name or we can *select* elements by their class.
Both are powerfull things, and both are used in every page.

You usually select by tag name to get some defaults for the whole page.

There is yet a third way to `select` an element, by the `id`. You see that in the html file there is:

```html
<img id="flynn" src="flynn.jpg">
```

The tag `img` is, no surprise including an image in the page. Has two properties.
And `src` property very simmilar to the `href` property of the `link` tag.
And a new property called `id`. This is short for *identifier*.
You can again put *any* name your want but it is unique to that element.

In this case the `id="flynn"` is telling the browser hey this is the only element whose identification is `flynn`.

Then in the css counter part we have the following code:

```css

#flynn {
    width: 200px;
    border: 2px solid red;
    border-radius: 7px;
}
```

Notice how it starts with a "#" (sharp, hash or pound sign). Its commands the browser:

Hey man, do me a favour and locate the single element whose `id` is `flynn`.
Now, once to find it, could you please make it 200 pixels wide, add a two pixel red solid border.
And since we are at that could you add a radiuos to the border. Thanks again, don't know what I would do without you.

You might think I am joking around with all the *please* and *thank your*.
Well I am not. CSS and HTML are very badly designed languages.
If you ask them to do something they don't understand or don't know how to do it,
they just won't do it or would do something they fit suits the occassion without telling you anything.
If you forget a `{` or a `;` everything is going to work, it jsut going to *silently* ignore your commands.
So don't forget to say please and thank you evrey time.

One last thing. You saw we used the color `#ffff00` for the background of the `div`'s.
That is the right way of specifying (one of the right ways, anyway) a color.
You can find more about it on the inernet.

Mozilla is always a good source of information: [color value](https://developer.mozilla.org/en/docs/Web/CSS/color_value)



