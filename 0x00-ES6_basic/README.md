JavaScript basics
•	Previous
•	Overview: Getting started with the web
•	Next
JavaScript is a programming language that adds interactivity to your website. This happens in games, in the behavior of responses when buttons are pressed or with data entry on forms; with dynamic styling; with animation, etc. This article helps you get started with JavaScript and furthers your understanding of what is possible.
What is JavaScript?
JavaScript is a powerful programming language that can add interactivity to a website. It was invented by Brendan Eich.
JavaScript is versatile and beginner-friendly. With more experience, you'll be able to create games, animated 2D and 3D graphics, comprehensive database-driven apps, and much more!
JavaScript itself is relatively compact, yet very flexible. Developers have written a variety of tools on top of the core JavaScript language, unlocking a vast amount of functionality with minimum effort. These include:
•	Browser Application Programming Interfaces (APIs) built into web browsers, providing functionality such as dynamically creating HTML and setting CSS styles; collecting and manipulating a video stream from a user's webcam, or generating 3D graphics and audio samples.
•	Third-party APIs that allow developers to incorporate functionality in sites from other content providers, such as Disqus or Facebook.
•	Third-party frameworks and libraries that you can apply to HTML to accelerate the work of building sites and applications.
It's outside the scope of this article—as a light introduction to JavaScript—to present the details of how the core JavaScript language is different from the tools listed above. You can learn more in MDN's JavaScript learning area, as well as in other parts of MDN.
The section below introduces some aspects of the core language and offers an opportunity to play with a few browser API features too. Have fun!
A "Hello world!" example
JavaScript is one of the most popular modern web technologies! As your JavaScript skills grow, your websites will enter a new dimension of power and creativity.
However, getting comfortable with JavaScript is more challenging than getting comfortable with HTML and CSS. You may have to start small, and progress gradually. To begin, let's examine how to add JavaScript to your page for creating a Hello world! example. (Hello world! is the standard for introductory programming examples.)
Warning: If you haven't been following along with the rest of our course, download this example code and use it as a starting point.
1.	Go to your test site and create a new folder named scripts. Within the scripts folder, create a new text document called main.js, and save it.
2.	In your index.html file, enter this code on a new line, just before the closing </body> tag:
HTMLCopy to Clipboard
<script src="scripts/main.js"></script>
3.	This is doing the same job as the <link> element for CSS. It applies the JavaScript to the page, so it can have an effect on the HTML (along with the CSS, and anything else on the page).
4.	Add this code to the main.js file:
JSCopy to Clipboard
const myHeading = document.querySelector("h1");
myHeading.textContent = "Hello world!";
5.	Make sure the HTML and JavaScript files are saved. Then load index.html in your browser. You should see something like this:
 
Note: The reason the instructions (above) place the <script> element near the bottom of the HTML file is that the browser reads code in the order it appears in the file.
If the JavaScript loads first and it is supposed to affect the HTML that hasn't loaded yet, there could be problems. Placing JavaScript near the bottom of an HTML page is one way to accommodate this dependency. To learn more about alternative approaches, see Script loading strategies.
What happened?
The heading text changed to Hello world! using JavaScript. You did this by using a function called querySelector() to grab a reference to your heading, and then store it in a variable called myHeading. This is similar to what we did using CSS selectors. When you want to do something to an element, you need to select it first.
Following that, the code set the value of the myHeading variable's textContent property (which represents the content of the heading) to Hello world!.
Note: Both of the features you used in this exercise are parts of the Document Object Model (DOM) API, which has the capability to manipulate documents.
Language basics crash course
To give you a better understanding of how JavaScript works, let's explain some of the core features of the language. It's worth noting that these features are common to all programming languages. If you master these fundamentals, you have a head start on coding in other languages too!

