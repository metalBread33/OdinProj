
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
