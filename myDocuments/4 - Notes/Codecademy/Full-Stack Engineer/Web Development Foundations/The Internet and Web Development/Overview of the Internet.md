---
Index: "[[The Internet and Web Development]]"
---
# Overview of the Internet
### Hello, Internet
It is nearly impossible to overstate how much the internet has changed how we consume information and communicate with one another. More than four billion people around the world are internet users and the total number of websites on the world wide web is nearing two billion.

Despite the presence of the internet in our lives, very few internet users understand how it works. You don’t need to be an engineer to benefit from understanding how the internet works. However, understanding the internet’s infrastructure will help you decide if learning web development is right for you.

In this lesson, you will learn how the internet works behind the scenes. After finishing this lesson, you’ll be able to answer questions like:

- How is data sent from one computer to another?
- What is the relationship between a browser and a server?
- How is code turned into the experience that users see in their browsers?
- How has the web and web development changed from its invention to today?

By the end of this lesson, you will have the knowledge that you need to collaborate more effectively with engineers and jump into your own career in web development.

Instructions

Check out the graph on the right that shows the number of websites on the internet since 2000. When you’re ready, move to the next exercise.
![[Total Number of Websites.png]]
### The Ever-Expanding Network

So how did the internet start? In 1969, the United States Department of Defense funded the creation of _ARPANET_, a precursor network to the internet. ARPANET stands for Advanced Research Projects Agency Network. ARPANET connected supercomputing centers run by government agencies and universities.

These institutions wanted to connect their individual networks for large-scale information transfer. However, many of them followed different standards and technical implementations. In the 1970s, the _transmission control protocol_ and _internet protocol_, otherwise known as TCP/IP, were created to provide standards around the transfer of data that would allow these early networks to communicate with each other.

TCP/IP was researched and specified throughout the 1970s and adopted in the early 1980s. As different networks adopted TCP/IP, the interconnected global network of networks that is today known as the internet was formed.

Instructions:
Check out the map of early ARPANET supercomputers. When you’re ready, move to the next exercise.
![[Early ARPANET Instituitions.png]]

### The World Wide Web

While people today often use the terms internet and world wide web interchangeably, they actually refer to quite different things.

_The internet_ refers to the actual network of connected computing devices. Although the internet was around in the 1980s, there was not an intuitive way for most people to browse the internet. The internet just sent messages produced by one computer and presented them to another computer.

Engagement with the internet changed in 1989 when [[Tim Berners-Lee]] invented the _world wide web_. The world wide web is a collection of interlinked websites and other web resources. The world wide web, in combination with the rise of web browsers in the 1990s, introduced a user-friendly interface that enabled users to browse multimedia content and interact with other users.

The invention of the world wide web led to the use of the internet in wider society through the 1990s and the creation of a variety of websites that are still in use today.

Instructions:
The diagram to the right demonstrates how different pages on the World Wide Web are linked to one another. Move to the next exercise when you are ready to continue.
![[Diagrama WWW.png]]
### Browsers and Servers
As we’ve seen, the internet is a network that links computer devices worldwide, enabling people to share information with one another despite vast distances. But how is information sent from one device to another?

One way of understanding this process is to look at the _client-server_ model. In this model, the _client_ refers to the user’s device or program that is making a request for data. A client can be a browser or application running on a user’s laptop, smartphone, or tablet.

The [[server]] is the device or program in that network that waits for incoming requests and sends back data. This might be an in-house server, a rented server at a data center, or cloud server. At Codecademy, we have servers that store lesson data and our servers are sending this lesson data to your client device.

Instructions:
Watch the video to learn about the importance of browsers and servers, then move to the next exercise when you are ready to proceed.
https://youtu.be/oJ8NzLGMrSA

### 404 Status Code
Let’s take a deeper dive into the client-server model through exploring a part of HTTP that you’ve probably seen before: _HTTP status codes_.

When a server responds to a client, the server specifies a status code as a part of the response. Status codes indicate whether or not the HTTP request was successfully completed and if there was an error, they contain some information about the type of error that happened. The status code helps the browser know how to handle the data that was sent back with the response.

Review the HTTP statuses below and see if any of them seem familiar.


| Code                        | Explanations                                                    |
| --------------------------- | --------------------------------------------------------------- |
| 200 - OK                    | The request has suceeded                                        |
| 301 - Moved Permanently     | The resource has been moved and the client is being redirected. |
| 404 - Not Found             | The requested resource was not found                            |
| 500 - Internal Server Error | The server encountered an unexoected error                      |


Instructions

1. The browser is currently displaying a website that Alex has created to show photos and descriptions of her pets. If you click on the links for `Dogs` or `Cats`, you can see more information about Alex’s dogs and cats.
2. Next, click on the file icon in the upper left corner of the text editor. You’ll see the different HTML files that the server is ready to send to the browser whenever those links are clicked. These HTML files correspond to the different web pages that are displayed in the browser. When the `Dogs` link is clicked, the server will send the `dogs.html` file to the client.
3. Try out the `Dogs` and `Cats` links now!
4. Let’s create a 404 status response by making a request for a non-existent resource. Alex hasn’t built a webpage to list her turtles! Click on the link for `Turtles` to see the browser display the 404 status code.

```
<body>

  <img src='https://content.codecademy.com/programs/code-foundations-path/web-dev-survey/pets.jpg' width='400px'/>

  <p>Hi, I'm Alex. Welcome to my website dedicated to my pets! They are the cutest buckets of joy you'll ever lay your eyes on! Check them out here:</p>

  <ul>

    <li><a href="dogs.html">Dogs</a></li>

    <li><a href="cats.html">Cats</a></li>

    <li><a href="turtles.html">Turtles</a></li>

  </ul>
  
</body>
```

### How Do Browsers Work?
So far we’ve seen how a single request and response are handled between a client and a server. But most of the time, our devices aren’t making a single request. Every time we load a webpage, our device sends a request for each file that makes up that page. So even when we’re just loading _one_ webpage, that page can make multiple requests in order to retrieve different pieces of content, like images.

So how does this process work when we’re making multiple requests simultaneously?

All of the following steps happen in a split second:

1. When a user types in a URL and presses enter, the server processes the request and sends the HTML file back to the client. _HTML_ files hold the content of a website and they also contain links for any additional assets or code that are needed to display the site properly.
2. The browser will begin to search for elements in the HTML file and it will start to make additional HTTP requests for any other external resources used by the HTML file. This often includes:  
- One or more CSS stylesheets. _CSS_ stands for cascading style sheets; CSS creates the style and layout of a web page. The browser will request the CSS stylesheet, and when the server sends it back, the browser analyzes the CSS and starts applying the visual styles to the content of the site.  
- The request-response cycle also sends website assets, like images and videos, from the server to the browser. If these files are large, there might even be a noticeable delay before they are rendered by the browser.  
- One or more JavaScript files. _JavaScript_ makes the webpage interactive. This programming language functions as the “behavior” of the web page. A webpage that does not use JavaScript is known as a _static_ webpage.

In most modern browsers, these additional requests are made in parallel. This means that these requests are initiated at the same time, and the browser does not wait to receive one resource before requesting the next resource.

All of the resources are typically displayed as soon as possible. The HTML will be displayed even if some of the other assets have not been received by the browser.

Voila! The user can now interact with the website that they requested to see. This whole process typically happens in about a second or less, depending on the speed of the user’s connection, the size of the website, and even the physical distance between the browser and the server.

Instructions:
The animation to the right shows the different languages that work together to display a webpage. When you’re ready, move on to the next exercise.
![[Website Behavior.png]]
### Web 2.0
Now that we’ve covered some of the basics of how the internet works, let’s check out some trends that are fundamental to the emergence of modern web development and modern JavaScript.

The earliest static websites were composed of text, images, and links, with very little interactivity beyond browsing from one page to another. These websites are called _static_, which means lacking in movement because they do not change based on user behavior. As internet connection speeds and web technologies progressed, more complex interactions became possible on the web.

A collection of advances in the early 2000s created a cluster of web applications that are often called “Web 2.0”. In comparison to early static websites, Web 2.0 applications are often defined by:

- Providing a dynamic user experience by offering content that responds to user input without forcing the page to reload. In the early web, user input would typically take the user to a new page — and they would have to wait for the new page to load. In Web 2.0, websites could just update selected regions of the page, avoiding the interruption caused by reloading.
- Emphasizing user-generated content and social sharing. In the early web, content was generally authored by a single source. The rise of blogging, social media, and wikis in web 2.0 meant that users could generate content and share it with their friends.

There were important technical advances that enabled each of these advances in the user interface of the internet. For example:

- _jQuery_ was the first JavaScript [[framework]] that could fetch data while the web page is running.
- The rise of _web frameworks_ that connected to databases, like Spring, Django, and Ruby-on-Rails, enabled user-generated content to effectively be created, stored, and displayed.

Instructions:
What are the differences between Web 1.0 and Web 2.0 pages? The answers are in these screenshots.

On the left, the Web 1.0 page is _static:_ it does not respond to user behavior and the content is the same for all users.

On the right, the Web 2.0 page is:

- Interactive — you can Like and Comment on the page
- Dynamic — the time since posting (currently “12 hrs”) updates without reloading the whole page
- Allows social interaction — a lot of friends liked this image!

Move to the next exercise when you’re ready to continue.

### Current Internet Trends
The rise of internet-connected smartphones has profoundly changed how users interact with the internet. Mobile internet traffic now accounts for more than half of all internet traffic and web development practices have evolved in order to provide a good user experience regardless of device type.

##### Responsive Web Design

The rise of _responsive web design_ has changed how websites are built. Responsive web design was enabled by additions to the CSS language, like media queries and relative units. These additions allow the presentation of websites to adjust based on the size of the window in which they are displayed.

##### Mobile Applications and Devices

The rise of internet-connected _mobile applications_ has changed the way that we think about browsing the internet. Users accessing the internet on smartphones are likely to spend much more time with specific applications, rather than using their phone’s browser.

Though most mobile applications are internet connected, they are not part of the world wide web. The web is built out of links, whereas mobile applications are designed to keep the user’s attention.

If you want to learn about mobile development, web development is a great place to start! While the majority of mobile applications are built in programming languages, like Swift for iOS, it is increasingly common to see developers using JavaScript frameworks to build new apps.

Instructions:
Check out the basic responsive website shown here. Try resizing the screen—you’ll notice the font size adjusting as the screen width changes.

Move to the next exercise when you’re ready to proceed.

### Review
Congratulations! You should now have a general understanding of how the internet works, including:

- The growth of the internet as a network
- The difference between the internet and the world wide web
- The relationship between browsers and servers
- Preview: Docs Loading link description
- HTTP status codes, like 404 Not Found
- Big trends in web development, from static websites to Web 2.0 and the rise of mobile

If you work with engineers, this information will help you talk about websites and web applications at a more technical level. Or if you’re interested in becoming a web developer yourself, you now have the important context to start building your own website or web application!
