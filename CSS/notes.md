# Box Model:

The CSS box model is essentially a box that wraps around every HTML element. It consists of: content, padding, borders and margins. The image below illustrates the box model:
Content - The content of the box, where text and images appear
Padding - Clears an area around the content. The padding is transparent
Border - A border that goes around the padding and content
Margin - Clears an area outside the border. The margin is transparent

![alt text](image.png)

# Cascading:

CSS stands for Cascading Stylesheets. The cascade is the algorithm for solving conflicts where multiple CSS rules apply to an HTML element. It's the reason that the text of the button styled with the following CSS will be blue.

button {
color: red;
}

button {
color: blue;
}

Understanding the cascade algorithm helps you understand how the browser resolves conflicts like this. The cascade algorithm is split into 4 distinct stages.

Position and order of appearance: the order of which your CSS rules appear
Specificity: an algorithm which determines which CSS selector has the strongest match
Origin: the order of when CSS appears and where it comes from, whether that is a browser style, CSS from a browser extension, or your authored CSS
Importance: some CSS rules are weighted more heavily than others, especially with the !important rule type

# Specificity:

Think of specificity as a hierarchy that determines which style declaration is ultimately applied to an element.

-> A universal selector (\*) adds no specificity, leaving its value at the initial specificity of (0,0,0).

-> An element (type) or pseudo-element selector adds element-like specificity which increments the C component by 1.

The following examples have an overall specificity of (0,0,1).

Type selector

div {
color: red;
}
Pseudo-element selector

::selection {
color: red;
}

-> ID selector
An ID selector adds id-like specificity which increments the A component by 1, as long as you use an ID selector (#myID) and not an attribute selector ([id="myID"]).

In the following example, the specificity is (1,0,0)

#myID {
color: red;
}

# Selectors:

Common selectors:
/_ Universal _/

- {
  box-sizing: border-box;
  }

/_ Type or Tag _/
p {
margin-block: 1.5rem;
}

/_ Classname _/
.class {
text-decoration: underline;
}

/_ ID _/
#id {
font-family: monospace;
}

/_ Relational _/
li:has(a) {
display: flex;
}

Common Combinators
/_ Descendant _/
header h1 {
/_ Selects all Heading 1 elements in a Header element. _/
}

/_ Child _/
header > h1 {
/_ Selects all Heading 1 elements that are children of Header elements. _/
}

/_ General sibling _/
h1 ~ p {
/_ Selects a Paragraph as long as it follows a Heading 1. _/
}

/_ Adjacent sibling _/
h1 + p {
/_ Selects a Paragraph if it immediately follows a Heading 1 _/
}

/_ Chained _/
h1, p {
/_ Selects both elements. _/
}

# Pseudo-Classes and Pseudo-Elements

A pseudo-class is a selector that selects elements that are in a specific state, for example, they are the first element of their type, or they are being hovered over by the mouse pointer. They tend to act as if you had applied a class to some part of your document, often helping you cut down on excess classes in your markup, and giving you more flexible, maintainable code.

Pseudo-classes are keywords that start with a colon. For example, :hover is a pseudo-class.

article p:first-child {
font-size: 120%;
font-weight: bold;
}

Pseudo-elements behave in a similar way. However, they act as if you had added a whole new HTML element into the markup, rather than applying a class to existing elements.

Pseudo-elements start with a double colon ::. ::before is an example of a pseudo-element.

article p::first-line {
font-size: 120%;
font-weight: bold;
}

# z-index

The z-index property in CSS controls the vertical stacking order of elements that overlap. As in, which one appears as if it is physically closer to you. z-index only affects elements that have a position value other than static (the default).
div {
z-index: 1; /_ integer _/
}
