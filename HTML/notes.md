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
