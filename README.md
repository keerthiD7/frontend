HTML Core Concepts - Definitions, Attributes, and Examples

1. HTML (HyperText Markup Language)
Definition: HTML is the standard markup language used to create and structure content on web pages. It defines elements like headings, paragraphs, links, images, and more, telling the browser how to display them.
Example:
<!DOCTYPE html>
<html>
  <head>
    <title>My Page</title>
  </head>
  <body>
    <p>Hello, world!</p>
  </body>
</html>


2. HTML Element
Definition: An HTML element is a basic building block of HTML that typically includes a start tag, content, and an end tag. Some elements can be self-closing.
Example:
<p>This is a paragraph.</p>
<img src="logo.png" alt="Logo">


3. HTML Tag
Definition: A tag in HTML marks the beginning or end of an element. Tags are enclosed in angle brackets (< >).
Opening Tag: <h1>


Closing Tag: </h1>


Self-closing Tag: <br>



4. HTML Attribute
Definition: Attributes provide extra information about an HTML element. They appear inside the opening tag as name="value" pairs.
Example:
<a href="https://example.com" target="_blank">Visit</a>

href: Specifies the URL.


target: Defines where to open the link (e.g., _blank for new tab).



5. HTML Document Structure
Definition: The basic structure of any HTML document, which includes metadata and content.
Example:
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>Document</title>
  </head>
  <body>
    Content goes here.
  </body>
</html>

<!DOCTYPE html>: Declares HTML5 version


<html>: Root element


<head>: Metadata like title, styles


<body>: Main visible content



6. Headings (<h1> to <h6>)
Definition: Define the headings of a web page, with <h1> as the highest level and <h6> as the lowest.
Example:
<h1>Main Title</h1>
<h2>Subheading</h2>


7. Paragraph (<p>), Line Break (<br>), Horizontal Rule (<hr>)
Definition:
<p>: Defines a paragraph


<br>: Inserts a line break


<hr>: Creates a horizontal line across the page


Example:
<p>Hello<br>World</p>
<hr>


8. Text Formatting (<strong>, <em>, Comments)
Definition: These elements provide emphasis and importance to text or include developer notes.
<strong>: Bold and strong importance


<em>: Italic and emphasized meaning


<!-- comment -->: Adds comments to the HTML


Example:
<p>This is <strong>important</strong> and <em>highlighted</em>.</p>


9. Lists
Definition: Lists are used to group a set of related items.
Unordered List (<ul>):
Displays items with bullet points.


Used when item order is not important.


Ordered List (<ol>):
Displays items with numbers.


Used when item order matters.


List Item (<li>):
Defines an item in a list.


Example:
<ul>
  <li>Item A</li>
  <li>Item B</li>
</ul>

<ol>
  <li>First Step</li>
  <li>Second Step</li>
</ol>


10. Links (<a>)
Definition: Used to create hyperlinks that navigate to another page or section.
Example:
<a href="https://google.com" target="_blank">Google</a>

href: Destination URL


target: Controls where the link opens



11. Images (<img>)
Definition: Embeds images into the webpage.
Example:
<img src="pic.jpg" alt="A picture" width="300" height="200">

src: Image file path


alt: Alternate text for accessibility


width, height: Image dimensions



12. Tables
Definition: Used to organize and display data in rows and columns.
Example:
<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Alice</td>
    <td>24</td>
  </tr>
</table>

<table>: Table element


<tr>: Table row


<th>: Header cell


<td>: Data cell



13. Forms
Definition: Used to collect user input and submit it to a server.
Example:
<form action="/submit" method="post">
  <label for="name">Name:</label>
  <input type="text" id="name" name="username">
  <button type="submit">Submit</button>
</form>

action: Submission URL


method: POST or GET


type: Specifies input control


name, id: Identify the element



14. Semantic Tags
Definition: Tags that clearly describe their meaning, improving readability and SEO.
Example:
<header>
  <h1>My Blog</h1>
</header>
<nav>
  <a href="#">Home</a>
</nav>
<main>
  <article>
    <h2>Post Title</h2>
    <p>Post content here.</p>
  </article>
</main>

<header>: Introductory section


<nav>: Navigation links


<main>: Primary content


<article>: Independent content unit


<section>: Generic standalone section


<aside>: Tangential content (sidebar)


<footer>: Footer of the section/page



15. CSS Integration (HTML + CSS)
Definition: CSS is used to style HTML elements. It can be applied in different ways.
Inline CSS: Styling inside an HTML element.
<p style="color: red;">Red text</p>

Internal CSS: Styling within a <style> tag in the HTML head.
<head>
  <style>
    body { background-color: lightblue; }
  </style>
</head>

External CSS: Linking a separate .css file.
<head>
  <link rel="stylesheet" href="styles.css">
</head>


Let me know if you want tasks or questions based on this document!


1. What is the difference between an HTML tag and element?
Tag is the markup syntax like <p> or </p>.


Element is the complete structure including the opening tag, content, and closing tag.


👉 Example: <p>Hello</p> → here, the element is <p>Hello</p>, and <p> is the opening tag.



2. Why do we use the alt attribute in images?
The alt attribute gives a text description of an image.


It’s helpful when the image doesn't load or for screen readers used by visually impaired users.


👉 Example: <img src="pic.jpg" alt="A beautiful sunset">



3. What does the href attribute do in the <a> tag?
The href attribute defines the destination URL of a hyperlink.


Without href, the <a> tag won’t navigate anywhere.


👉 Example: <a href="https://google.com">Visit Google</a>



🧠 Intermediate Level
4. What are the differences between inline, internal, and external CSS?
Type
Where it's written
Usage
Inline
Inside the element using style
Quick styling for single elements
Internal
Inside <style> in <head>
Styling for one page
External
In a separate .css file
Reusable across multiple pages

👉 Example:
Inline: <p style="color:red;">Hello</p>


Internal: <style> p { color: red; } </style>


External: <link rel="stylesheet" href="style.css">



5. Explain the purpose of semantic tags like <section> and <article>
Semantic tags describe the meaning of content, not just its appearance.


<section>: Groups related content (like a chapter).


<article>: Independent content (like a blog post or news story).


Improves SEO, readability, and accessibility.



🚀 Advanced Level
6. What happens if you forget to include <!DOCTYPE html> at the beginning of your HTML document?
The browser may enter quirks mode, where it behaves like older versions.


Layout and CSS rendering might break.


<!DOCTYPE html> tells the browser to use standard mode (HTML5 rules).



7. How is <label> important for accessibility in forms?
The <label> tag connects text descriptions to form controls (like <input>).


Screen readers can read labels aloud, helping visually impaired users.


Also improves click usability — clicking the label will focus the input.


👉 Example:


html
CopyEdit
<label for="name">Name:</label>
<input type="text" id="name" name="name">


