# A dead simple webpage

The simplest web page in the world consists of a single file.

It doesn't need to be called `index.html`, you can call it anything you want. But that is the comon lore.

It is a text file, mening you can see the content with any text editor you want.
It is written in a language called HTML, in particular HTML5.

That is a markup language. Other markup languages you might have heard of are markdown (this very readme is written in markdown) and Latex.

As you can see it is compsed of something called *tags* or *elements*. Such as `<body>` or a paragraph `<p>`.

Some of these tags you need to explicitly close like the above mentioned `<body>` or `<p>`, but you will see that not all of them need to be closed that way.
For instance the rule for including an image is:

`<im src="my_image.png">`

There are many tags you will need to learn. But some comon tags:

* `body` and `head`, they are present in all documents
* `p` indicates a paragraph
* `div` and `span` are some of the most used tags to indicate a generic element.
* `h1`, ..., `h6` they are called header elements
* `im` to insert a immage.

The first declaration in the document `<!DOCTYPE html>` is a special tag telling the browser what version of HTML we will be using.
In the past that used to be a mess, nowadays, the one and only is HTML5 and is here to stay.
That needs to be in any single webpage.

The second tag `<html lang="en">` is where the HTML code for the page begins.
Note that is has a *property*, `lang`. Tags in HTML may have properties. We will see that that is very useful.
Is this case is telling the browser or client to use the English language.

Then we have the `head` tag. Everything in there is somehow metainformation.
Like what is the title of the webpage, or what kind of simbols do I what to use.
In this case, for example, we say the title is "Our first webpage" and we say that the set of characters we want to use is "UTF8".

Do you perhaps remember the ASCII code? UTF8 is simply an anhancement of it.
For now we will always use utf8 encoded unicode characters. this include manythings on the face of the earth, from arabic and hindi characters to the € sign.


