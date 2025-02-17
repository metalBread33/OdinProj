
# Intro to HTML and CSS

- 2 languages that work to create everything you see on the internet
- HTMl is the raw data; CSS is the stlye it is presented in
- Not used to program logic, not technically "programing" languages

## HTML vs CSS vs JS

### HTML

- HTML == Hypertext Markup Language
- Uses tags
  - `<h1></h1>`
- HTML files must end in .html

### CSS

- CSS == Cascading Style Sheet
- Used to style HTML
- Can be used to make HTML responsive
  - **Responsive** means the page can be displayed on different types of screens (phones, desktop, etc.)
- Can write CSS inline with the HTML or in a .CSS file and link it to the HTML

### Javascript (JS)

- Programming language of the web
- Used to add behavior to the web page
- Javascript code stored in a .JS file

## Elements and Tags

- Almost all element on an HTML page are just pieces of content wrapped in opening and closing HTML tags
  - Opening tags tell browser it is the start of an HTML element `<>`
  - Closing tags tell browser where the element ends `</>`
- `<p>This is a paragraph tag</p>`
- Text in between tags are what is displayed
- Vast list of predefined tags; need to use the best one
- Some HTML elements fo not have a closing tag
  - Called **void** or **self-closing** elements
  - Use a '/' at the end of the tag
    - `<br/>`
  - Can be rendered fine, but their use is discouraged

## HTML Boilerplate

- All HTML documents have the same basic structure/boilerplate that needs to be in place before anything useful can be done
- Homepage of the website should always be called **index.html**
  - Web servers look for an index.html page by default when users land on websites

### DOCTYPE

- Tells browser what version of HTML it should render
  - Latest is HTML5
  - `<!DOCTYPE html>`

### HTML element

- Root element of the document
  - More important when learning about manipulating HTML with JS
- Every element should be within the html element
- `<html lang = "en"></html>`
  - **lang** attribute specifies the language of the text im element
    - Improves accessibillity of webpage

### Head element

- Where all the important meta-infomation about webpages go
- Do not use any element that displays content on the webpage

```html
  <html lang = "en">
    <head>
      <meta charset="UTF-8">
      <title>WebPage</title>
    </head>
  </html>
```

- Meta element specifies the charset encoding of the webpage
  - Important because it ensures the webage will display special symbols and chars from different languages correctly in the browser
- Title element gives webpage a human readable title

### Body element

- Where all content that needs to be displayed to the user goes
- `<body> </body>`

### Viewing HTML files in the browser
  
1) Drag and drom HTML file into browser
2) Double click HTML file in system
3) Use terminal

### VS Code shortcut

- ! in a blank html file
- Fills out all boilerplate

## Working with Text

### Paragraphs

- When browser encounters new lines in HTML, it will compress them down into 1 space
- `<p>` is the paragraph element
- Used for standard text

### Headings

- Displayed larger and bolder than regular text
- 6 different levels of headings
  - `<h1>` is largest and boldest
  - `<h6>` is the lowest level

### Other

- `<strong>` makes text bold
- `<em>` makes text italic
  - These 2 are mainly nested in other tags
  - Ex) `<p>This is an <strong>bolded</strong> word <p>`
- HTML comments are not redenered but are used to provide context
  - `<!-- This is a comment -->`

## Lists

- 2 types of lists: ordered and unordered

### Unordered lists

- Created with the `<ul>` element
- Items in the list are created with `<li>` element
  - Displayed as bullet points

### Ordered lists

- Created with the `<ol>` element
- Items also created with `<li>` element
  - Displayed as a numbered list

## Links and Images

- **Anchor** elements (`<a>`) are used to create links
- Need to use the **href** attribute to determine where the link should go

  ```html
  <a href = "a.link.to.somewhere">Click this link to go somewhere</a>
  ```

- **target** attribute specifies where the linked resource will be opened
  - Default value is *_self*
    - Opens link in current tab
  - Can be changed to *_blank* which opens link in a new tab
- **rel** attribute describes the relation between the current page and linked document
  - *noopener* ensures that a link opened in a new tab or window cannot interact with or accesss original page
    - Without it new page can use JS to manipulate the original page which is a security risk
  - *noreferrer* provides both privacy and security
    - prevents the page from knowing wher ethe user came from and includes the behavior or noopener

### Absolute links

- Links to pages on other websites
  - `scheme://domain/path`
  - `https://www.theodinproject.com/about`

### Relative links

- Links to pages within our own website
  - Relative file path from page you are already on

## Images

- `<img>` elemnt allows us to display images
  - Void element - does not need a closing tag
- *src* attribute determines where the image file is located
- *alt* attribtue used to describe an image if the image cannot be loaded
