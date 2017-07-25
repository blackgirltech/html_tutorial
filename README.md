# BGT HTML Tutorial

## Why HTML?
- Explain briefly how the internet works and what HTML documents are used for

### The Web
In order to understand HTML documents, it’s worth getting a basic understanding of how the web works. The web links documents to each other by using the infrastructure of the internet (the two should not be confused). These documents are stored on computers called servers and can be accessed by visiting the servers location through a web browser.

For example, when you visit google.com in your web browser, your computer (client) is asking a server which has the google.com document to send you a copy. You then download that document to your web browser in order for you to see and interact with the page (search bar, links etc).

This is why HTML is so important, it is the bedrock of the web.

### HyperText Markup Language

These documents are written in HyperText Markup Language, or HTML, which is used to structure and describe the content of your webpage. There are a number of HTML tags that you can use to structure and describe your content. For example, you’d use the `<title>` tag to indicate that whatever is inside this tag is the name of your site. More on that in the _Let’s Build_ section.

Websites are built up of HTML tags containing content.

## First Steps
- include any set up here

So you’re probably wondering “how do I make a HTML document” or have wondered how to make a website. It’s less complicated than you think:
- On your computer create a folder and name it `my_site` (or something else, the name doesn’t matter)
- Inside this folder create a file called `index.html`

This is your HTML document. Open this file in Chrome, Firefox or your web browser of choice. You’ll see a blank page, because you haven’t put any content into it yet, but this is essentially what you’ll get when you visit any other page on the web.

	
## Let’s Build
On the first line of our html document we’ll add the following:
```html
<!DOCTYPE html>
```

This informs the browser of the HTML version the document is written in.

```html
<!DOCTYPE html>
<html> 

</html> 
```

This our root HTML element all other HTML tags will be added between the opening tag `<html>` and our closing tag `</html>`.

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
        <header>
        </header>

        <main>
        </main>
    </body>
</html> 
```

No let’s add to our document’s `body`.

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

Let’s break down the above. The `<header>` tag is where we’ll have the heading of the page and our site navigation. The `<main>` tag will contain, you guessed it, the main content of the site.

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
            <h1>My portfolio site<h1>

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
- `<ul>` unordered list - list elements inside this an unordered list will not be numbered
- `<li>` list item - Used to tag every item that appears in a list

The anchor tag turns whatever content inside into a hyperlink which can be used to link to other HTML documents and other elements on the page.

Supply the anchor with a `href` attribute give it a web address to go to:

`<a href="https://www.google.com">This is a link to Google</a>`

In our case, we’re linking to three other HTML documents.

#### Main



## Next Steps
- Mention styling and adding more HTML elements