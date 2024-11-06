# HTML Learning Kit

> *Click &#9733; if you like the project. Your contributions are heartily ♡ welcome.*

<br/>

<span style="color: red">SHORT NOTES</span> is provided in this [LINK](./short-notes/notes.md)

- [HTML Learning Kit](#html-learning-kit)
  - [HTML5 Features](#html5-features)
    - [1. Semantics tags](#1-semantics-tags)
    - [2. Form Inputs and attributes](#2-form-inputs-and-attributes)
    - [3. Multimedia Support:](#3-multimedia-support)
    - [4. HTML5 Api's](#4-html5-apis)
    - [5. Canvas and SVG for Graphics](#5-canvas-and-svg-for-graphics)
  - [HTML Document Structure](#html-document-structure)
    - [1. HTML Document Structure Basics](#1-html-document-structure-basics)
    - [2. DOCTYPE Declaration](#2-doctype-declaration)
    - [3. HTML Root Element](#3-html-root-element)
    - [4. Head Section](#4-head-section)
    - [5. Body Section](#5-body-section)
    - [6. HTML Document Structure Example](#6-html-document-structure-example)
    - [7. Best Practices for HTML Document Structure](#7-best-practices-for-html-document-structure)
    - [8. Key Elements to Know](#8-key-elements-to-know)
  - [SEO using HTML tags](#seo-using-html-tags)


## HTML5 Features

### 1. Semantics tags

- It provide meaningful structure to web documents, improving readability and accessibility.
  
1. `<header>`: Represents the introductory contents or a section for the site's title, logo, navigation links or menu, etc.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <header>
          <h1>My Website</h1>
          <nav>
            <ul>
              <li><a href="#">Home</a></li>
              <li><a href="#">About</a></li>
              <li><a href="#">Contact</a></li>
            </ul>
          </nav>
        </header>
        ```

      </details>

2. `<nav>`: Used for the navigation section containing links to other pages or parts of the website.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <nav>
          <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
          </ul>
        </nav>
        ```

      </details>

3. `<section>`: Represents a standalone section of content, typically with a heading.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <section>
          <h2>About Us</h2>
          <p>Information about our company.</p>
        </section>
        ```

      </details>

4. `<article>`: Represents self-contained content that can be independently distributable or reusable.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
       <article>
          <h2>Blog Post Title</h2>
          <p>Blog post content goes here.</p>
          <footer>Published on June 1, 2023</footer>
        </article>
        ```

      </details>

5. `<aside>`: Used for content related to the surrounding content (like sidebars).
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <aside>
          <h3>Related Links</h3>
          <ul>
            <li><a href="#">Link 1</a></li>
            <li><a href="#">Link 2</a></li>
          </ul>
        </aside>
        ```

      </details>

6. `<footer>`: Defines the footer section for a document or section.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <footer>
          <p>© 2023 My Website. All rights reserved.</p>
        </footer>
        ```

      </details>
7. `<main>`: Represents the main content of the body, excluding headers, footers, and sidebars.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <main>
          <h1>Article Title</h1>
          <p>Article content goes here.</p>
        </main>
        ```

      </details>
8. `<figure>` and `<figcaption>`: Use a `<figure>` element to mark up a photo in a document, and a `<figcaption>` element to define a caption for the photo:
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <figure>
          <img src="pic_trulli.jpg" alt="Trulli" style="width:100%">
          <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption>
        </figure>
        ```

      </details>



### 2. Form Inputs and attributes

1. `Input types`: new input types that provide better input validation and user experience. 
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <label for="email">Email:</label>
        <input type="email" placeholder="Email" required>

        <input type="date" placeholder="Date">

        <input type="number" placeholder="Number">

        <input type="range" min="0" max="100" step="5">

        <input type="url" id="website" name="website" placeholder="https://example.com">

        <input type="tel" id="phone" name="phone" placeholder="123-456-7890">

        <input type="color" id="favcolor" name="favcolor">
        ```

      </details>

2. `placeholder`: The placeholder attribute allows you to provide hints or example values within input fields. It disappears when the user starts typing.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <input type="text" placeholder="Enter your name">
        ```

      </details>
  
3. `required`: The required attribute specifies that an input field must be filled out before submitting the form.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <input type="text" required>
        ```

      </details>
  
4. `pattern`: The pattern attribute allows you to specify a regular expression pattern that the input value must match.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <input type="text" pattern="[A-Za-z]{3}">
        ```

      </details>
  

5. `autocomplete`: The autocomplete attribute specifies whether a form field should have autocomplete functionality enabled or disabled.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <input type="text" autocomplete="off">
        ```

      </details>
  
### 3. Multimedia Support:

- Native support for multimedia elements, eliminating the need for plugins like Adobe Flash. The `<audio>` and `<video>` elements allow developers to embed audio and video content directly into web pages. 

1. `<audio>`: Embeds an audio file on a web page.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <audio src="audiofile.mp3" controls="">
          Your browser does not support the audio element.
        </audio>
        ```

      </details>
  
2. `<video>`: Embeds a video file on a web page.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <video src="videofile.mp4" controls="">
          Your browser does not support the video element.
        </video>
        ```

      </details>

3. `<source>`: Specifies alternative media resources for `<audio>` and `<video>` elements.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <video controls="">
          <source src="" type="video/mp4">
          <source src="" type="video/webm">
          Your browser does not support the video element.
        </video>
        ```

      </details>
      
4. `<track>`: Specifies timed text tracks, such as captions or subtitles, for `<video>` and `<audio>` elements.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
          <video controls="">
            <source src="" type="video/mp4">
            <track src="" kind="captions" label="English" srclang="en">
            Your browser does not support the video element.
          </video>
        ```

      </details>

5. `<embed>`: Embeds external content, such as plugins or multimedia content, within an HTML document.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
          <video controls="">
            <source src="" type="video/mp4">
            <track src="" kind="captions" label="English" srclang="en">
            Your browser does not support the video element.
          </video>
        ```

      </details>

### 4. HTML5 Api's


1. Geolocation API: Retrieves the geographical location of the user.
    - <details>
        <summary style="padding: 4px; border: 1px solid black; ">Example</summary>

        ```javascript
        navigator.geolocation.getCurrentPosition(function(position) {
          console.log("Latitude: " + position.coords.latitude);
          console.log("Longitude: " + position.coords.longitude);
        });
        ```
      </details>

2. Web Storage API: Stores data on the client side.
     - **Local Storage**: Persistent storage until manually cleared.
        <details>
          <summary style="padding: 4px; border: 1px solid black">Example</summary>

          ```javascript
          localStorage.setItem('key', 'value');
          let data = localStorage.getItem('key');
          ```
        </details>

     - **Session Storage**: Data stored only for the session.
        <details>
          <summary style="padding: 4px; border: 1px solid black">Example</summary>

          ```javascript
          sessionStorage.setItem('key', 'value');
          ```

        </details>
3. Web Workers: Runs JavaScript in background threads, helping to offload tasks.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```javascript
        let worker = new Worker('worker.js');
        worker.postMessage('Hello');
        ```
      </details>

4. Drag and Drop API: Enables dragging and dropping of elements.
    - <details>
        <summary style="padding: 4px; border: 1px solid black">Example</summary>

        ```html
        <div draggable="true" ondragstart="drag(event)">Drag me</div>
        ```

      </details>
5. History API: Manipulates browser history.
    - <details>
        <summary style="padding: 4px; border: 1px solid black; background-color: gray; border-radius: 5px">Example</summary>
        
        ```javascript
        history.pushState({ page: 1 }, "title 1", "?page=1");
        ``` 

      </details>


### 5. Canvas and SVG for Graphics

- It supports drawing and animations directly on the web page.

   - **`<canvas>`**: Used for rendering 2D graphics via JavaScript.
     ```html
     <canvas id="myCanvas" width="200" height="200"></canvas>
     ```
   - **SVG (Scalable Vector Graphics)**: XML-based format for vector images.
     ```html
     <svg width="100" height="100">
       <circle cx="50" cy="50" r="40" fill="blue" />
     </svg>
     ```
 
## HTML Document Structure

### 1. HTML Document Structure Basics
   - Every HTML document follows a standard structure consisting of the `<!DOCTYPE>`, `<html>`, `<head>`, and `<body>` tags.
   - This structure provides the browser with the necessary information to render the page correctly.

### 2. DOCTYPE Declaration
   - The `<!DOCTYPE html>` declaration is the very first line of an HTML document.
   - It tells the browser the version of HTML being used (HTML5).
   - It is not a tag but an instruction to the browser for rendering mode.

   ```html
   <!DOCTYPE html>
   ```

### 3. HTML Root Element

   - `<html>`: The root element that contains all other elements of the HTML document.
   - Contains both the `<head>` and `<body>` sections.

   ```html
   <html lang="en">
       <!-- The rest of the document goes here -->
   </html>
   ```

### 4. Head Section

   - The `<head>` section contains meta-information about the document, which is not displayed on the page.
   - Common elements within the `<head>` include:

     - **Meta Tags**: Used to define the character set, viewport settings, author, and description of the document.

       ```html
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       ```

     - **Title**: Defines the title displayed on the browser tab.

       ```html
       <title>Document Title</title>
       ```

     - **Link Tags**: Links to external resources like stylesheets and icons.

       ```html
       <link rel="stylesheet" href="styles.css">
       <link rel="icon" href="favicon.ico">
       ```

     - **Script Tags**: Links to external JavaScript files, though it’s often recommended to place scripts at the end of the `<body>` for better performance.

       ```html
       <script src="script.js" defer></script>
       ```

### 5. Body Section
   - The `<body>` section contains the content that is rendered on the page, such as text, images, links, and forms.
   - This is where the primary structure and layout of the visible content is defined using HTML elements.

   ```html
   <body>
       <!-- Visible content goes here -->
   </body>
   ```

### 6. HTML Document Structure Example

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Basic HTML Document Structure</title>
       <link rel="stylesheet" href="styles.css">
       <script src="script.js" defer></script>
   </head>
   <body>
       <h1>Welcome to My Website</h1>
       <p>This is a sample HTML document structure.</p>
   </body>
   </html>
   ```

### 7. Best Practices for HTML Document Structure
   - **Use Semantic HTML**: Use tags like `<header>`, `<footer>`, `<article>`, `<section>`, and `<aside>` to give meaning to your content and improve accessibility.
   - **Organize the `<head>` Properly**: Ensure meta tags for character encoding and viewport settings are placed at the top of the `<head>` section.
   - **Load CSS Before JS**: Always load CSS files before JavaScript files to avoid blocking page rendering.
   - **Defer or Place Scripts at the End**: Use `defer` or `async` attributes for external JavaScript files, or place them just before the closing `</body>` tag for better page load performance.

### 8. Key Elements to Know
   - `<html lang="en">`: Sets the language attribute for accessibility and SEO.
   - `<meta charset="UTF-8">`: Defines the character encoding to support most languages.
   - `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Ensures responsiveness by setting the viewport width to the device width.
   - `<title>`: Defines the page title, which is important for SEO and bookmarking.
   - `<link rel="stylesheet" href="styles.css">`: Links to the CSS file.
   - `<script src="script.js" defer></script>`: Links to an external JavaScript file without blocking page rendering (using `defer`).

## SEO using HTML tags
