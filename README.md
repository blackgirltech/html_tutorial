# BGT HTML Tutorial

## Why HTML?

### The World Wide Web

In order to understand HTML documents, it’s worth getting a basic understanding of how the web works. The web links documents to each other by using the infrastructure of the internet (the two should not be confused). These documents are stored on computers called servers and can be accessed by visiting the servers location through a web browser.

For example, when you visit google.com in your web browser, your computer (client) is asking a server which has the google.com document to send you a copy of the site. You then download the document and interact with it through your web browser.

This is why HTML is so important, it is the bedrock of the web.

### HyperText Markup Language

These documents are written in HyperText Markup Language, or HTML, which is used to structure and describe the content of your webpage. There are a number of HTML tags that you can use to structure and describe your content. For example, you’d use the `<title>` tag to indicate that whatever is inside this tag is the name of your site. More on that in the _Let’s Build_ section.

Websites are built up of HTML tags containing content.

## First Steps

So, let's grab our starter files:

- [Click here](https://github.com/blackgirltech/html_tutorial) to visit our html tutorial repo
- Click on the green `Clone or download` button and select `Download ZIP`
- Open this folder on your computer

The `index.html` file is essentially your website. Open this file in Chrome, Firefox or your web browser of choice. You’ll see a blank page, because you haven’t put any content into it yet, but this is essentially what you’ll get when you visit any other page on the web.

### Text Editor

Next we'll download a text editor for us to write code in. [Sublime Text](https://www.sublimetext.com/2) suits our needs just fine.

## Let’s Build

On the first line of our html document we’ll add the following:

```html
<!DOCTYPE html>
```

This tells the browser the HTML version the document is written in.

```html
<!DOCTYPE html>
<html> 

</html> 
```

This is our root HTML element, all other HTML tags will be added between the opening tag `<html>` and our closing tag `</html>`.

Take notice of the `/`. This needs to be included to signify the closing of a tag.

### Head and Body
The `head` of a HTML document is where information about the site is stored, such as the title and description of your site, and what other files the document is linked to.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>
            My portfolio site
        </title>
    </head>
</html> 
```

In our case, we’ll add the `<title>` of our web page. Name your site whatever you’d like.

Next is the body, which will contain all of the visible content on our site.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>
            My portfolio site
        </title>
    </head>

    <body>
    </body>
</html> 
```

Now let’s add to our document’s `body`.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>
            My portfolio site
        </title>
    </head>

    <body>
        <header>
        </header>

        <main>
        </main>
    </body>
</html>
```

Let’s break down the above. The `<header>` tag is where we’ll have the heading of the page and our site navigation. The `<main>` tag will contain, as the name would suggest, the main content of the site.

### Adding Content

#### Header

```html
<!DOCTYPE html>
<html>
    <head>
        <title>
            My portfolio site
        </title>
    </head>

    <body>
        <header>
            <h1>My portfolio site</h1>

            <nav>
            <nav>
        </header>

        <main>
        </main>
    </body>
</html>
```

The `h1` is a heading tag. They range from `h1` - `h6` and are ordered by importance.

The `<nav>` is where we’ll have our navigation menu which will link to different pages, although for this tutorial, we’ll just assume there are other pages to link to.

Next we’ll add the following mark up inside of the `<nav>`:

```html
<ul>
    <li>
        <a href=“about.html”>
            About
        </a>
    </li>
    <li>
        <a href=“work.html”>
            Work
        </a>
    </li>
    <li>
        <a href=“contact.html”>
            Contact
        </a>
    </li>
</ul>
```

Let’s break this down:

- `<ul>` unordered list - list items inside an unordered list will not be numbered
- `<li>` list item - Used to tag every item that appears in a list

The anchor tag turns it's content into a hyperlink, which can be used to link to other HTML documents as well as other elements on the page.

Supply the `anchor` with a `href` attribute and give it a web address to go to:

`<a href="https://www.google.com">This is a link to Google</a>`

In our case, we’re linking to three other HTML documents.

#### Main
This is where the main content of our HTML document will live.

To make things more organised, we'll use two `<div>` tags to separate our content into two sections. A `<div>` is a generic container and is used primarily for styling purposes.

```html
<main>
    <div>
    </div>

    <div>
    </div>
</main>
```

We'll add text inside the first `<div>` and an `image` in the other.

```html
<main>
    <div>
        <h2>Lorem ipsum</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam ullamcorper laoreet nunc, vel lobortis quam finibus nec. Ut ligula augue, lobortis in metus ac, commodo malesuada diam.</p>
    </div>

    <div>
    </div>
</main>
```

Notice we use a level 2 heading (`<h2>`) here which respects the heading heirarchy. The `<h1>` we added above remains the prominent heading.

The `<p>` tags are used to establish paragraphs.

```html
<main>
    <div>
        <h2>Lorem ipsum</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam ullamcorper laoreet nunc, vel lobortis quam finibus nec. Ut ligula augue, lobortis in metus ac, commodo malesuada diam.</p>
    </div>

    <div>
        <img src="assets/img/image.jpg" alt="a home office" />
    </div>
</main>
```

The `<img>` tag is a self closing tag, which means you don't need to write another `</img>` to indicate the end of the tag. Here we've given it two `attributes`:

- `src` points to the location of the image you want to display. In our case, we're telling the document to look inside the `assets` folder, then the `img` folder and grab our image.

- The `alt` attribute contains alternative text describing our image. This is important for people who use assistive technology such as screen readers. A screen reader will read out the `alt` text, which is invaluable for users who may have a visual impairment.

#### Footer

```html
<footer>
    <p>Nunc eros augue&copy;<p>
</footer>
```

The `<footer>` tag usually contains author details, related links and copyright information. We'll sign off with a copyright.

And that's it! That's our site.

## Finishing up

Open the `index.html` file in your web browser and admire your work, you've just built a website.

You'll see the site looks quite bare bones and that's where `CSS` (Cascading Style Sheets) comes in. You'll use CSS to style your site and make it more pleasing on the eye. More on that in the next tutorial.

## Bonus
Remember those extra pages we linked to in our `navigation`? Try creating those pages so our links work.

Above we're linking to `about.html`, so you can create that file and put it in the same folder as our `index.html`. Try using the tags in different ways to create your pages. You could even research other tags not covered in this tutorial and use those. Check our [HTML Cheatsheet](https://github.com/blackgirltech/cheatsheets/blob/master/html-cheat-sheet.md) for more.
