---
Index: "[[The Internet and Web Development]]"
---
### What is HTML
Alejandra knows that the first step to building a website is learning HTML. Why? _HTML_ is the skeleton of all web pages. It provides structure to the content on a website, including text, images, buttons, videos, and more.

HTML is a practical place to start learning to code. You can build basic websites after learning just a little HTML, with text, images, and videos. You can always open up your work-in-progress website with your browser and see what you’re building.

HTML stands for **h**yper**t**ext **m**arkup **l**anguage. In the next few exercises, we will look at the HTML acronym word-by-word to unpack what HTML really means.

Instructions:
Take a peek at the HTML code to the right. Some parts of the language are pretty intuitive, see if you can figure out how anything works.

If not, don’t worry! We’ll explain it soon.

```
<h1>Why learn HTML?</h1>

<p>HTML provides the skeleton for websites, and it is a great place to start when learning to code!</p>

<img src="https://content.codecademy.com/programs/code-foundations-path/web-dev-survey/programming.jpeg" alt="" height="100" width="100">

<p>HTML is used by:</p>

<ul>

  <li>Web developers</li>
  <li>Marketers</li>
  <li>Content creators</li>
  <li>Entrepreneurs</li>
  <li>and many more!</li>

</ul>
```

### HTML Markup
The _ML_ in HTML stands for _markup language_. Markup refers to a way of annotating text that is distinguishable from the text itself. The same way that a teacher might “markup” a student essay by underlining topic sentences and circling spelling errors, HTML annotates the content within a web page.

A teacher might use a red pen to make sure that their comments are easy to distinguish from the student’s own work. HTML separates content and annotation by using HTML tags, which are denoted by angle brackets (also known as less-than and greater-than signs).

Instructions

Compare the markup for the essay to the markup in the HTML diagram. How do they compare?

Open the following dropdowns to see some sample comparisons:

- Comparison 1 
	- Both the HTML markup and the essay have sections of text. The HTML markup is separated by new lines and tags with `<>`. The essay has the text separated by new lines.

- Comparison 2
	- Both documents include a title near the top. The HTML markup is titled “HTML Tutorial,” marked with `<title>` tags. The essay has “My Autobiography” as the title, which is annotated as “Title” with an arrow.

- Comparison 3
	- Similar to the essay’s body text, the HTML has the tag `<body>` for the body text.

- Comparison 4
	- In the essay, portions of the body text are annotated to indicate what purpose they serve in the text, such as “Hook,” “Thesis Statement,” and “Conclusion.”
	- In the `<body>` of the HTML, individual portions are annotated with HTML tags like `<p>` and `<h1>` to indicate the function that the text will serve on the web page. We’ll learn more about these tags in subsequent exercises!

![An example of HTML code for a website side by side with an imagined autobiography page, demonstrating the similarities in structure.](https://content.codecademy.com/programs/code-foundations-path/html%20annotation.svg)
### HTML Elements

HTML tags are the “markup” for HTML. They are annotations that provide information about the type of content they contain. Let’s take a close look at the syntax for how HTML tags surround content to create an HTML element.

The diagram displays an HTML paragraph element. As we can see, the paragraph element is made up of one opening tag (`<p>`), the content (“Hello World!” text), and a closing tag (`</p>`).

Let’s quickly review each part of the element pictured:

- HTML element — a unit of content in an HTML document formed by HTML tags and the text or media it contains.
- Opening Tag — the element name used to start an HTML element. The tag type is surrounded by opening and closing angle brackets.
- Content — The information (text or other elements) contained between the opening and closing tags of an HTML element.
- Closing tag — the second HTML tag used to end an HTML element. Closing tags have a forward slash (/) inside of them, directly after the left angle bracket.

Instructions:
Study the diagram to the right to learn about the anatomy of HTML syntax. When you’re done, continue to the next exercise.
![[HTML Anaotmy.png]]
### Common Tags

Okay, let’s practice using HTML elements by writing a few different tags.

Here are a few common tags that you can start getting familiar with:
```
<h1>This is a heading, it emphasizes text.</h1>

<p>This is a paragraph, it is the most common tag for larger chunks of text.</p>

<a>This is an anchor tag, used to specify the text that is the "anchor" for a link.</a>

<button>This is a button.</button>

```

Instructions:
1. Checkpoint 1 Enabled
    1.    Let’s make the heading stand out! Put an opening and closing `h1` tag around the text that says `Jetsetter Travel Agency`.

```
<h1>Jetsetter Travel Agency</h1>

<p>With over 25 years of experience in concierge, high-end travel planning, we'll provide you with the highest quality services. Every vacation is unique, custom, and tailored to your tastes.

</p>

<button>Click here!</button>
```

### Hypertext and the World Wide Web

The H and T in HTML stands for **h**yper**t**ext. Hypertext is text that is linked to other text. This diagram shows different websites that are connected to each other through links, which are represented by arrows.

What’s so hyper about hypertext? The prefix _hyper_ indicates that the text expands beyond the traditional constraints of the written word. Instead of reading documents from beginning to end, like you would read a book, someone going through hypertext can _browse_. By clicking on links from one document to another, the user can navigate to whatever page they find the most interesting and carve their own unique path through the web.

Many modern websites provide rich user experiences, with features like embedded videos, animations, and interactivity, so it doesn’t necessarily feel like you are just navigating from one HTML page to the next. But despite all of the advances that have taken place with the growth of the web, at its core the web is still just a collection of hyperlinked documents.

Instructions:Review the structure of links shown in the diagram, then continue to the next exercise when you are ready.

![[Diagrama WWW.png]]
### Adding Hyperlinks

Let’s explore how hypertext works by adding a link to a basic website!

Reading and modifying code is an essential first step in learning to build things for the web. This practice can take you a long way while you’re learning to build websites from scratch.

An _attribute_ in HTML provides additional information about an HTML element. It comes in a name and value pair with the structure `name="value"`. For example, you can specify the width of an HTML element with the attribute `width="500"`.

Links are created in HTML with something called the `href` attribute, which stands for **h**yperlink **ref**erence. The `href` attribute allows us to specify the URL, or address on the web, that a link should take users to. See below for an example of the `href` attribute in action.

When we set the `href` attribute on an anchor tag (abbreviated to `<a>`) we can specify both the text that should be rendered for the user (the text within the anchor tag) and the URL that the browser should navigate to.

With this code, we’re assigning the value `www.codecademy.com` to the `href` attribute. When a user clicks on the text of this link (Learn to code!), they will be directed to [www.codecademy.com](http://www.codecademy.com/).

```
<a href="www.codecademy.com">Learn to code!</a>
```

Instructions:
1. Alejandra has begun to build out her business’s website. She wants to link from her homepage to a different page that contains her resume. 
 To start, look in **index.html** for the text that says `25 years of experience` — it should be near line 20. Put an anchor tag (`<a>`) around this text.

2. Add a `href` attribute to this anchor tag, and give it the value `/resume.html`.
This URL is called a _relative path_ and it looks a little different from the full URLs you’re used to seeing. That’s because it’s actually a link to another page on the same website, so we can omit the first part. Instead of `www.jetsetter.com/resume.html` we can abbreviate the link to just `/resume.html`.
Open the hint if you need a reminder on how to set attributes for html tags.


3. Click on the link that you just made to navigate to see Alejandra’s resume!
Click **Run** one more time when you are ready to move on to the next lesson.


### What is CSS?

Using just HTML, Alejandra was able to build a website that contains all of the content that she wants. But it doesn’t look very impressive—Alejandra knows that a basic black and white website won’t give her business the credibility she needs to find new customers.

That’s where CSS comes in! _CSS_ is the language that provides _style_ to the content of an HTML page. This includes colors, fonts, positioning, layout, and more!

Why do we need a separate language for content and presentation? This is an example of the computer science principle _separation of concerns_. Large codebases are kept maintainable when each section has clearly differentiated problems that it is trying to solve.

Since the styling rules are described separately from the content itself, if Alejandra adds more paragraphs, images, or other forms of content, she can expect them to be styled the same way as her existing content. This will save Alejandra time in the long run, especially as her website gets more and more complex.

Instructions

After you’ve reviewed the diagram to compare the uses of HTML and CSS, continue to the next exercise.

Community Support

Still have questions? Get help from the [Codecademy community](https://community.codecademy.com/c/start-here/).

### What is CSS?

Using just HTML, Alejandra was able to build a website that contains all of the content that she wants. But it doesn’t look very impressive—Alejandra knows that a basic black and white website won’t give her business the credibility she needs to find new customers.

That’s where CSS comes in! _CSS_ is the language that provides _style_ to the content of an HTML page. This includes colors, fonts, positioning, layout, and more!

Why do we need a separate language for content and presentation? This is an example of the computer science principle _separation of concerns_. Large codebases are kept maintainable when each section has clearly differentiated problems that it is trying to solve.

Since the styling rules are described separately from the content itself, if Alejandra adds more paragraphs, images, or other forms of content, she can expect them to be styled the same way as her existing content. This will save Alejandra time in the long run, especially as her website gets more and more complex.

Instructions: After you’ve reviewed the diagram to compare the uses of HTML and CSS, continue to the next exercise.
![](https://content.codecademy.com/programs/code-foundations-path/web-dev-survey/House-Blue-Print-Diagram.svg)
### Applying CSS

Alejandra has learned CSS and created the desired visual rules to make her website look sleek and polished. 

Navigate to the **style.css** file to take a look at the CSS code that she’s written.

In this file, you will recognize many of the HTML tags that you have been working with — and maybe a few that you haven’t seen yet! CSS contains _selectors_ that specify the HTML elements to which the style should be applied as well as _visual rules_ that specify how that content should be displayed.

Now it’s time to use the HTML link element to apply the CSS file to her existing website. This is done with an HTML link tag. An HTML link tag is often used to create a connection between an HTML file and the CSS file and tells the browser to apply the CSS styles to the HTML.

Instructions
    1. On line 6 of **index.html**, copy and paste the code below to apply the CSS file to the existing HTML.
    Use your knowledge of HTML attributes to figure out what this code specifies, and check out extra information in the hint if you want to learn more.
    ```
```
<link rel="stylesheet" href="style.css">
```

2. Awesome! Alejandra’s site is looking good! Just a little CSS can make the difference between a website that looks like a skeleton and portfolio-ready site. 
	Now let’s tweak the CSS just a little bit, to see how the visual rules specified in CSS can change the way that a website is displayed.
	Navigate to the **style.css** and scroll down to line 37 where you will see the `h1` selector. This section defines the styles for the `h1` element on the page, which is the most prominent heading.
	Just for practice, change the `color` property from `white` to `black` and press Run to see what changes!

### What is JavaScript?

Now that Alejandra has her website looking polished, she’s realized that she wants the site to be more interactive. She would like to build a shopping cart feature that allows her users to buy travel packages directly from her website.

To accomplish this, Alejandra is going to need to learn JavaScript. Any website that provides more than just static information probably utilizes JavaScript in some way. Here are some familiar examples of website features most often built with JavaScript:

- popup ads
- animated graphics (2D or 3D)
- interactive audio and video
- maps and other features access the user’s geographic location
- and much more!

One of the defining features of JavaScript is its ability to respond to browser events. These events happen in real time and can be triggered by a wide variety of user interactions, including:

- the user clicking on a button
- the user pressing enter on their keyboard
- a video file finishing loading
- the user re-sizing their window
- the user hovering over text on the webpage

Instructions:
1. One of the classic browser events that JavaScript can respond to is the position of the mouse. When a user puts the mouse near an HTML element, the `onmouseover` event is fired.
	Hover over the text in the browser to see how it responds to the `onmouseover` event.
	Once you have observed the effect of `onmouseover`, click the **Run** button to move on to the next Checkpoint.
2. What else is happening here?
	JavaScript uses functions, which are reusable blocks of code designed to perform a specific task. 
	`drawText` is a function that is being run on line 2. Change the text that says `'hello world'` to `'JavaScript'` to pass a different value into this function.
	Check out the browser to see what changed! One of the benefits of functions is that they are _reusable_. The `drawText` function allows us to take advantage of the reusability of functions because it can render any input text without us needing to rewrite the logic of the function.
	Confused? Don’t worry, we’ll cover functions more thoroughly in the next exercise.

### JavaScript Functions
In the last exercise, you started to think about two key building blocks of JavaScript: functions and events. Let’s review:

- Functions allow us to write a chunk of code once that can be reused over and over.
- Events allow JavaScript to respond to user behaviors, like the user hovering their mouse over an HTML element or resizing their window.

Events and functions combine to give JavaScript the ability to create interactive experiences. When an event is fired, a function is executed. This pattern is used again and again in web development to create interactive websites.