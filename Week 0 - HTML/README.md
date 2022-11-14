# WEEK 0 - HTML

- [WEEK 0 - HTML](#week-0---html)
  - [Intro](#intro)
  - [What's HTML](#whats-html)
    - [Let's look at an example](#lets-look-at-an-example)
        - [Exhibit 0.1](#exhibit-01)
        - [Exhibit 0.2](#exhibit-02)
        - [Fun Activity 0.1](#fun-activity-01)
        - [Fun Activity 0.2](#fun-activity-02)
    - [HTML is pretty simple](#html-is-pretty-simple)
    - [Stages of Website Evolution](#stages-of-website-evolution)
  - [Homewerk](#homewerk)
  - [MORE??](#more)

## Intro

You will start the same way I started. On codecademy. It's free. It's fun. It's the best bang for your buck for learning coding stuff. And lessons can be done in itty bitty chunks of time if you need to.

I've assigned you just the HTML course to start (see: [Homewerk](#homewerk)).

Our journey begins with **HTML**, "the building block of the Web":tm:. Once we understand how to build a website with HTML we can then:
- make it pretty with **CSS**
- make it interactive with **JavaScript**
- make it process data from forms with **Python** on the backend
-  unify your HTML, CSS, and JavaScript and do it all in **React**
- fire all your developers and switch to a [no-code](https://www.superblocks.com/) solution

## What's HTML

> HTML (HyperText Markup Language) is the most basic building block of the Web. It defines the meaning and structure of web content. Other technologies besides HTML are generally used to describe a web page's appearance/presentation (CSS) or functionality/behavior (JavaScript).
>
> "Hypertext" refers to links that connect web pages to one another, either within a single website or between websites. Links are a fundamental aspect of the Web. By uploading content to the Internet and linking it to pages created by other people, you become an active participant in the World Wide Web.
>
>HTML uses "markup" to annotate text, images, and other content for display in a Web browser. HTML markup includes special "elements" such as `<head>, <title>, <body>, <header>, <footer>, <article>, <section>, <p>, <div>, <span>, <img>, <aside>, <audio>, <canvas>, <datalist>, <details>, <embed>, <nav>, <output>, <progress>, <video>, <ul>, <ol>, <li>` and many others.
>
>An HTML element is set off from other text in a document by "tags", which consist of the element name surrounded by "<" and ">". The name of an element inside a tag is case insensitive. That is, it can be written in uppercase, lowercase, or a mixture. For example, the `<title>` tag can be written as `<Title>`, `<TITLE>`, or in any other way. However, the convention and recommended practice is to write tags in lowercase.

*Source: https://developer.mozilla.org/en-US/docs/Web/HTML*

### Let's look at an example

When you go to example.com in your internet browser, you are making a backend request to example.com's server. And example.com's server is sending you back HTML code.

That HTML code looks like this:

##### Exhibit 0.1
```
<div>
    <h1>Example Domain</h1>
    <p>This domain is for use in illustrative examples in documents. You may use this
    domain in literature without prior coordination or asking for permission.</p>
    <p><a href="https://www.iana.org/domains/example">More information...</a></p>
</div>
```
*Source: [example.com](https://example.com)*

But your internet browser is super smart. So it doesn't just show you that plain text. The browser knows how to render it into something visual.

##### Exhibit 0.2
<p align="left">
  <img src="./examplecom.png" width="300" >
</p>

But at the end of the day, all that's getting sent to the browser from example.com's server is like a kilobyte of plaintext data.

I know. This is all hard to believe. A website is just like, what, all letters and numbers? Yeah pretty much.

Don't believe me? See for yourself!!!!!

##### Fun Activity 0.1
- [ ] Open up your **Terminal** application
    - I'm not sure if you've used the command line before. If you haven't, you're in for a treat. Get ready to get all Mr. Robot with it.
    - I don't know how this works on Windows. Here, look at this. https://www.lifewire.com/how-to-open-command-prompt-2618089
- [ ] type in `curl example.com`
    - then press `Enter` on your keyboard

What you've just done is make a `GET` request to `example.com` - the same thing your internet browser does when you enter `example.com` into the address bar.

In the response on your terminal, you should be seeing the exact same HTML instructions that your internet browser received.

Isn't that neat! A website is just made up of a bunch of letters and numbers. There are even those who believe in the mystic arts and say that it's all just *1's and 0's* all the way down. Personally, I've never seen it. And I would prefer to keep religious conjecture out of my school.

If you want to see those raw instructions that go into making a website, you can even access it from your browser.

##### Fun Activity 0.2
- [ ] Go to [example.com](https://example.com)
- [ ] Open up the *inspector*
    - This can also be accomplished by right-clicking on a page and selecting "Inspect."

    <p align="left">
        <img src="./inspector.png" width="300" >
    </p>

    - Or you can learn the [shortcut](https://www.codeleaks.io/shortcut-inspect-element-browsers/) for your browser + operating system of choice.
- [ ] Behold. More information than you ever wanted to know.
    <p align="left">
        <img src="./inspected.png" width="300" >
    </p>

You can even play around with the inspector to change things about your website. This is a tool that every frontend dev uses.
<p align="left">
    <img src="./turtles.png" width="300" >
</p>

### HTML is pretty simple

Let's look back at our HTML code example from [Exhibit 0.1](#exhibit-01). 
```
<div>
    <h1>Example Domain</h1>
    <p>This domain is for use in illustrative examples in documents. You may use this
    domain in literature without prior coordination or asking for permission.</p>
    <p><a href="https://www.iana.org/domains/example">More information...</a></p>
</div>
```
Even without really knowing any HTML, we can still read it and kinda see what's going on. All the main content is nested inside a `<div>` container. The main title is inside Header1 `<h1>` tags. Content is inside `<p>` tags. The Codecademy course will give you a deeper breakdown, but HTML is pretty straightforward.

If you look on Codecademy, you will notice that there is no class for "Beginner HTML" or "Intermediate HTML" or "Advanced HTML". It's just "Learn HTML". That's all there is to it. You can get 99% of what you need to know from just that one class.

So then what's so hard about web development?

The catch is that HTML ([for the most part](https://html.com/html5/#What_is_HTML5)) is totally static. It can't change once it's been loaded. There's no interactivity.

### Stages of Website Evolution

That being said, you could still make a website using HTML alone. example.com comes pretty close, but even that has some CSS styling. Here's a great example of website that's about as bare-bones as it gets: https://motherfuckingwebsite.com/

Paul Graham's [personal website](http://www.paulgraham.com/articles.html) takes it about 1 step further. There is some minimal CSS styling and color. There are a couple images. But this can all be accomplished without any JavaScript. 

Now go to [SquareSpace](https://www.squarespace.com/) and start scrolling down. Whoa! Look at all those things popping in and out and flying around! So neat! So trendy! A lot of that fancy dynamic stuff was accomplished thanks to JavaScript. Nowadays some of that fancy stuff can be accomplished with advanceed HTML and CSS, but in general moving elements and interactivity and calculations will be handled by javascript.

But there are other uses for JavaScript that may be more pertinent to your web app needs. Try going to https://www.airbnb.com and searching for a rental in `Hot Springs, Arkansas`. Pay special attention to each step along the way. There are a ton of tiny micro-interactions that you may not have appreciated before. Things to click, settings to adjust, new DOM elements getting loaded in. This is a serious JavaScript application.

However, your fishing web application may not even need JavaScript. You can make web forms and display submission results using HTML alone. And if you don't need JavaScript, why bother?

## Homewerk

Take as much time as you need, but doing this course is a prerequisite to doing anything else webdev-related. I can 100% guarantee you that codecademy will teach these concepts in a better and more time efficient manner than I can.

- [ ] Learn HTML
    - https://www.codecademy.com/learn/learn-html

## MORE??

The next thing I'm going to have you learn is Python. If you finish your HTML course before we meet again, you can get started on your next homework assignment.

- [ ] Learn Python 3
    - https://www.codecademy.com/learn/learn-python-3

*(FYI, it's not "Learn Python" + "3", it's "Learn" + "Python 3". It's Python v3. As opposed to Python v2. The update from v2 to v3 had major breaking changes in the core Python language a few years ago. Yeah. Let's not worry about that. https://xkcd.com/1987/)*

And yeah, you'll be learning Python for backend, not Javascript. Python is where you want to start. It's simpler, it's clearer, it's more transferable. When you understand Python, you'll understand how every other OOL (Object-Oriented Language) works (GO, Java, Python, Ruby, JavaScript, COBOL, etc.).

Alternatively, if you want to continue on the frontend path and learn how to make your website pretty, you can learn CSS. I'm on the fence about how much I want to make you learn this. We can discuss next week.

- [ ] Learn CSS
    - https://www.codecademy.com/learn/learn-css
