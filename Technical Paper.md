# How a Browser Renders HTML, CSS, and JavaScript to DOM. What is the mechanism behind it ?

## What Does Browser Rendering mean?
Rendering in a browser refers to the process of converting webpage code (HTML, CSS, and JavaScript) into the visual content displayed on the user's screen.
When a user opens a webpage, the browser requests and downloads HTML, CSS, and JavaScript files from a server. 
The browser then processes these files and converts them into a visual page that users can see and interact with. This entire process is known as **browser rendering**.

## What is DOM?
**DOM (Document Object Model)** is a structured representation of an HTML document created by the browser.  
Each HTML element becomes an object (node) arranged in a tree-like structure.

## What Does the DOM Do?
The DOM acts as a bridge between the webpage and JavaScript. It allows scripts to dynamically update the page without reloading it.

Using the DOM, JavaScript can:

- Change text and content on the page
- Modify styles and appearance
- Add or remove HTML elements
- Respond to user actions like clicks or typing
- Update page structure dynamically

Because of the DOM, modern websites can update content interactively without refreshing the entire page.

## Rendering Mechanism 

### 1. HTML Download and Parsing
The browser first downloads the HTML file and parses it to build the **DOM (Document Object Model)**, which represents the structure of the webpage.

### 2. CSS Parsing
Next, the browser downloads CSS files and converts them into the **CSSOM (CSS Object Model)**, which stores style rules for page elements.

### 3. JavaScript Execution
JavaScript files are then executed. JavaScript can modify the DOM and update styles dynamically, allowing interaction and dynamic content changes.

### 4. Render Tree Creation
The browser combines the DOM and CSSOM to build a **Render Tree**, which contains only the elements visible on the page along with their computed styles.

### 5. Layout Calculation
The browser calculates the size and position of each visible element on the page. This step determines where elements appear on the screen.

### 6. Painting
After layout calculation, the browser draws text, images, colors, and borders onto the screen.

### 7. Compositing
Finally, different visual layers are combined and displayed as the complete webpage seen by the user.

## Conclusion
In summary, the browser converts webpage code into visible content by creating the DOM and CSS structures, calculating layout, and painting elements onto the screen. 
JavaScript further enhances the page by dynamically updating content and behavior.

## References
- MDN Web Docs – How Browsers Work  
  https://developer.mozilla.org/en-US/docs/Web/Performance/How_browsers_work

- Medium – How the Browser Renders a Web Page: DOM, CSSOM, and Rendering  
  https://medium.com/jspoint/how-the-browser-renders-a-web-page-dom-cssom-and-rendering-df10531c9969



