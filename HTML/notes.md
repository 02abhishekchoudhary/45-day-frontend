# HTML:

-> It is the most basic building block of the web. It defines the meaning and structure of web content.
-> Hypertext refers to links that connect web pages to one another, either within a single website or between websites.
-> HTML uses "markup" to annotate text, images and other content for display in a web browser.

# ELEMENT:

-> An html element is set off from other text in a document by "tags", which consists of the element name surrounded by <>.
-> The name of an element inside a tag is case-insensitive. That is, it can be written in uppercase, lowercase, or a mixture.
-> For example the <title> tag can be written as <Title>, <TITLE>, <TiTlE> or in any other way.
-> However, the convention and recommended practice is to write tags in lowercase.

# HTML ELEMENT:

-> Opening tag + content + closing tag
-> VOID ELEMENTS: Not all elements follow the pattern of an opening tag, content, and a closing tag. Some elements consist of a single tag, which is typically used to insert/embed something in the document. e.g. <img>
-> HTML is very, very forgiving. For example, if we omit the closing </li> tags, the closing tags are implied.
-> Non-replaced elements: The paragraph, header, and lists are all non-replaced. Non-replaced elements have opening and (sometimes optional) closing tags that surround them and may include text and other tags as sub-elements. These enclosing tags can turn a phrase or image into a hyperlink, can make a sentence into a header, can give emphasis to words, and so on.
-> Replaced and void elements: Void elements cannot contain text content or nested elements. Void elements include <br>, <col>, <embed>, <hr>, <img>, <input>, <link>, <meta>, <source>, <track>, and <wbr>, among others. => Most replaced elements are void elements, but not all. The video, picture, object, and iframe elements are replaced, but aren't void. They can all contain other elements or text, so they all have a closing tag. => Most void elements are replaced; but again, not all, as we saw with base, link, param, and meta. Why have a void element, which can't have any content, that isn't replaced and thereby doesn't render anything to the screen? To provide information about the content! The information is provided by the elements' attributes.

# Attributes

-> Attributes provide information about the element. The attribute, like the rest of the opening tag, won't appear in the content, but they do help define how the content will appear to both your sighted and non-sighted (assistive technologies and search engines) users. => Attributes only appear in the opening tag. The opening tag always starts with the element type. The type can be followed by zero or more attributes, separated by one or more spaces. Most attribute names are followed by an equal sign equating it with the attribute value, wrapped with opening and closing quotation marks.

# Document structure:

# QUIRKS MODE:

-> In the old days of the web, pages were typically written in two versions: One for Netscape Navigator, and one for Microsoft Internet Explorer. When the web standards were made at W3C, browsers could not just start using them, as doing so would break most existing sites on the web. Browsers therefore introduced two modes to treat new standards compliant sites differently from old legacy sites.
-> There are now three modes used by the layout engines in web browsers: quirks mode, limited-quirks mode, and no-quirks mode. In quirks mode, layout emulates behavior in Navigator 4 and Internet Explorer 5. This is essential in order to support websites that were built before the widespread adoption of web standards. In no-quirks mode, the behavior is (hopefully) the desired behavior described by the modern HTML and CSS specifications. In limited-quirks mode, there are only a very small number of quirks implemented.
-> The limited-quirks and no-quirks modes used to be called "almost-standards" mode and "full standards" mode, respectively. These names have been changed as the behavior is now standardized.

<!DOCTYPE html>
<html lang="en-US">
  <head>
  </head>
  <body>
  </body>
</html>

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Machine Learning Workshop</title>
    <meta name="viewport" content="width=device-width" />
  </head>
  <body>

  </body>
</html>

# CSS

-> There are three ways to include CSS: <link>, <style>, and the style attribute.
-> <link> tag used for linking external css file
-> <script> tag used for linking external js file.

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Machine Learning Workshop</title>
    <meta name="viewport" content="width=device-width" />
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
  <script src="script.js"></script>
  </body>
</html>

# Features of HTML5:

1. Introduction to Audio and Video
   <!DOCTYPE html>
   <html lang="en">

<head>
    <title>
        Example of Video and Audio Tags
    </title>
</head>

<body>
    <h2>Example of video and audio tag</h2>

    <video width="300" height="200" controls autoplay>
        <source src="/html5/foo.ogg" type="video/ogg" />
        <source src="/html5/foo.mp4" type="video/mp4" />
        Your browser does not support the video element.
    </video>

    <audio controls autoplay>
        <source src="/html5/audio.ogg" type="audio/ogg" />
        <source src="/html5/audio.wav" type="audio/wav" />
        Your browser does not support the audio element.
    </audio>

</body>

</html>

2. Vector Graphics
   <svg id="svgelem" height="200" 
       xmlns="http://www.abc.org/2000/svg">
   <circle id="redcircle" cx="50" cy="50" 
           r="50" fill="red" />
   </svg>

3. Header and Footer
   <!DOCTYPE html>
   <html>

<head>
    <title>HTML Header</title>
</head>

<body>
    <article>
        <header>
            <h1>This is the heading.</h1>
            <h4>This is the sub-heading.</h4>
            <p>This is the metadata.</p>
        </header>
    </article>
</body>

</html>

<!DOCTYPE html>
<html>

<head>
    <title>HTML Footer</title>
    <style>
        a {
            font-size: 25px;
            text-decoration: none;
        }

        p {
            font-size: 25px;
        }
    </style>

</head>

<body>
    <footer>
        <nav>
            <p>
                <a href=
"https://www.geeksforgeeks.org/about/">About Us</a>|
                <a href=
"https://www.geeksforgeeks.org/privacy-policy/">Privacy Policy</a>|
                <a href=
"https://www.geeksforgeeks.org/careers/">Careers</a>
            </p>
        </nav>
        <p>@geeksforgeeks, Some rights reserved</p>
    </footer>
</body>

</html>

4. Figure and Figcaption
<figure>
    <img src=
"https://media.geeksforgeeks.org/wp-content/cdn-uploads/20190710102234/download3.png" 
        alt="GFG" style="width:50%">
    <figcaption>Fig.1 - Geeksforgeeks.</figcaption>
</figure>

5. HTML Nav Tag
<h1> HTML Nav tag</h1>
<nav>
    <a href="/html/">HTML</a>
    <a href="/css/">CSS</a>
    <a href="/js/">JavaScript</a>
    <a href="/jquery/">jQuery</a>
</nav>

6. HTML Progress Tag
<h1>The progress element</h1>

<label for="file">Downloading progress:</label>
<progress id="file" value="32" max="100"> 32% </progress>

7. Form Enhancements
   <!DOCTYPE html>
   <html>

<body> 
    <center> 
        <h1 style="font-size:25px;font-style:italic;"> 
            HTML FORM 
        </h1> 
        <h2 style="font-size:25px;font-style:italic;"> 
        Placeholder Attribute in Input Element 
        </h2> 
        <form action=" "> 
            <input type="text" name="fname" placeholder="First name"> 
            <br> 
            <input type="text" name="lname" placeholder="Last name"> 
            <br> 
            <input type="submit" value="Submit"> 
        </form> 
</center> 
</body>

</html>

-> EMAIL ATTRIBUTE

<!DOCTYPE html>
<html>

<head>
    <title>
        HTML input type email
    </title>
</head>

<body style="text-align:center;">

    <h1 style="color:green;">
        GeeksForGeeks
    </h1>

    <h2>HTML <input type="email"></h2>

    <form>
        Email: <input type="email"
            value="manaschhabra499@gmailo.com">
    </form>

</body>

</html>

8. Web Storage

9. Offline Web Applications

10. WebSockets

# Forms (Input types, attributes, validations)

After submitting the form:

<form method="GET">
  <label for="student">Pick a student:</label>
  <select name="student" id="student">
    <option value="hoover">Hoover Sukhdeep</option>
    <option>Blendan Smooth</option>
    <option value="toasty">Toasty McToastface</option>
  </select>
  <input type="submit" value="Submit Form">
</form>

Radio buttons:

<fieldset>
  <legend>Who is your favorite student?</legend>
  <ul>
    <li>
      <label>
        <input type="radio" value="blendan" name="machine"> Blendan Smooth
      </label>
    </li>
    <li>
      <label>
        <input type="radio" value="hoover" name="machine"> Hoover Sukhdeep
      </label>
    </li>
    <li>
      <label>
        <input type="radio" value="toasty"  name="machine"> Toasty McToastface
      </label>
    </li>
  </ul>
</fieldset>

CSS:
/_ One radio button per line _/
label {
display: block;
cursor: pointer;
line-height: 2.5;
}

/_ the basic, unchecked style _/
input[type="radio"] {
appearance: none;
display: inline-block;
width: 2em;
height: 2em;
border-radius: 50%;
border: 0.25em solid #000;
}

[type="radio"]:focus {
background: lightgreen;
border-color: white;
box-shadow: 0 0 0 3px black;
}
/_ the checked style using the :checked pseudo class _/
[type="radio"]:checked {
background: blue;
border-color: white;
box-shadow: 0 0 0 3px black;
}

/_ never forget focus styling _/

/_ Nothing to see here. _/
body {
margin: 3em auto;
max-width: 30em;
font-family: comic-sans;
font-size: 1.5rem;
font-family: sans-serif;
}
li {
list-style-type: none;
}

fieldset {
border: 2px solid #000;
padding: 2em;
border-radius: 0.5em;
}

legend {
color: #fff;
background: #000;
padding: 0.25em 1em;
border-radius: 1em;
}

Labels and fieldsets
<label for="full_name">Your name</label>
<input type="text" id="full_name" name="name">

<fieldset>
  <legend>Who is your favorite student?</legend>
  <ul>
    <li>
      <label>
        <input type="radio" value="blendan" name="machine"> Blendan Smooth
      </label>
    </li>
    <li>
      <label>
        <input type="radio" value="hoover" name="machine"> Hoover Sukhdeep
      </label>
    </li>
    <li>
      <label>
        <input type="radio" value="toasty" name="machine"> Toasty McToastface
      </label>
    </li>
  </ul>
</fieldset>

Input types and dynamic keyboard:
<input type="tel">
<input type="email">

Accessing the microphone and camera:
<label for="avatar">A recent photo of yourself:</label>
<input type="file" capture="user" accept="image/*" name="avatar" id="avatar">

Built-in validation:
There are some CSS selectors that match form controls based on the presence of HTML attributes including :required and :optional if the boolean required is set or not; :default if checked is hard-coded; and :enabled or :disabled, depending on whether the element is interactive and if the disabled attribute is present. The :read-write pseudoclass matches elements with contenteditable set and form controls that are by default editable, such as number, password, and text input types (but not checkbox, radio buttons, or the hidden type, among others). If a normally writable element has the readonly attribute set, it will match :read-only instead.

As the user enters information into form controls, the CSS UI selectors, including :valid, :invalid, :in-range, and :out-of-range will toggle on and off depending on the state. When the user exits a form control, either the not-yet fully supported :user-invalid or :user-valid pseudo-class will match.

You can use CSS to provide cues about whether form controls are required and valid as the user interacts with the form. You can even use CSS to prevent users from being able to click the submit button until the form is valid:

form:invalid [type="submit"] {
opacity: 50%;
pointer-events: none;
}

<dialog open aria-labelledby="dialogid">
  <form action="thankyou.php">
    <button type="submit" aria-label="close" formmethod="dialog" formnovalidate>X</button>
    <h2 id="dialogid">Application</h2>
    <p>All fields are required</p>
    <p>
       <label>Name: 
         <input type="text" name="name" required />
      </label>
    </p>
    <p>
      <label>Warranty: 
        <input type="number" min="0" max="10" name="warranty" required />
       </label>
    </p>
    <p>
      <label>Power source:
        <select name="powersoure">
          <option>AC/DC</option>
          <option>Battery</option>
          <option>Solar</option>
        </select>
      </label>
    </p>
    <p>
      <button type="submit" formmethod="post">Submit</button>
    </p>
  </form>
</dialog>

body {
background:lightpink;
font-family: sans-serif;
}
[aria-label="close"] {
float: right;
appearance: none;
border-radius: 5rem;
margin: -1em;
}
p {
margin-top: 1em;
}
h2 + p {
margin-top: -1em;
}
label {
display: flex;
flex-direction: column;
}

# Semantic HTML:

-> With over 100 HTML elements, and the ability to create custom elements, there are infinite ways to mark up your content; but some ways—notably semantically—are better than others.
-> Semantic means "relating to meaning". Writing semantic HTML means using HTML elements to structure your content based on each element's meaning, not its appearance.

The first code snippet uses <div> and <span>, two elements with no semantic value.:

<div>
  <span>Three words</span>
  <div>
    <a>one word</a>
    <a>one word</a>
    <a>one word</a>
    <a>one word</a>
  </div>
</div>
<div>
  <div>
    <div>five words</div>
  </div>
  <div>
    <div>three words</div>
    <div>forty-six words</div>
    <div>forty-four words</div>
  </div>
  <div>
    <div>seven words</div>
    <div>sixty-eight words</div>
    <div>forty-four words</div>
  </div>
</div>
<div>
   <span>five words</span>
</div>

code with semantic elements:

<header>
  <h1>Three words</h1>
  <nav>
    <a>one word</a>
    <a>one word</a>
    <a>one word</a>
    <a>one word</a>
  </nav>
</header>
<main>
  <header>
    <h1>five words</h1>
  </header>
  <section>
    <h2>three words</h2>
    <p>forty-six words</p>
    <p>forty-four words</p>
  </section>
  <section>
    <h2>seven words</h2>
    <p>sixty-eight words</p>
    <p>forty-four words</p>
  </section>
</main>
<footer>
  <p>five words</p>
</footer>

# Accessibility object model (AOM):

As the browser parses the content received, it builds the document object model (DOM) and the CSS object model (CSSOM). It then also builds an accessibility tree. Assistive devices, such as screen readers, use the AOM to parse and interpret content. The DOM is a tree of all the nodes in the document. The AOM is like a semantic version of the DOM.

The role attribute:

<div role="banner">
  <span role="heading" aria-level="1">Three words</span>
  <div role="navigation">
    <a>one word</a>
    <a>one word</a>
    <a>one word</a>
    <a>one word</a>
  </div>
</div>
