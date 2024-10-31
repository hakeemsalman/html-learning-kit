# HTML SHORT NOTES

> *Click &#9733; if you like the project. Your contributions are heartily ♡ welcome.*

<br/>

[Back To Home](../README.md)

- [HTML SHORT NOTES](#html-short-notes)
  - [1. **New Semantic Elements**](#1-new-semantic-elements)
  - [2. **New Form Elements and Attributes**](#2-new-form-elements-and-attributes)
    - [New Input Types](#new-input-types)
    - [New Attributes](#new-attributes)
  - [3. **Media Elements (Audio and Video)**](#3-media-elements-audio-and-video)
  - [4. **Canvas and SVG for Graphics**](#4-canvas-and-svg-for-graphics)
  - [5. **HTML5 APIs**](#5-html5-apis)
    - [Geolocation API](#geolocation-api)
    - [Web Storage API](#web-storage-api)
    - [Web Workers](#web-workers)
    - [Drag and Drop API](#drag-and-drop-api)
    - [History API](#history-api)
  - [6. **Microdata and Accessibility Features**](#6-microdata-and-accessibility-features)
  - [7. **Progress and Meter Elements**](#7-progress-and-meter-elements)
  - [8. **Other Useful Elements**](#8-other-useful-elements)
  - [Interview Tips](#interview-tips)


## 1. **New Semantic Elements**
   HTML5 introduced new elements to provide meaningful structure to web documents, improving readability and accessibility.

   - **`<header>`**: Defines the header section for a document or section (usually contains introductory content or navigation links).
   - **`<nav>`**: Used for the navigation section containing links to other pages or parts of the website.
   - **`<section>`**: Represents a standalone section of content, typically with a heading.
   - **`<article>`**: Represents self-contained content that can be independently distributable or reusable.
   - **`<aside>`**: Used for content related to the surrounding content (like sidebars).
   - **`<footer>`**: Defines the footer section for a document or section.
   - **`<main>`**: Represents the main content of the body, excluding headers, footers, and sidebars.
   - **`<figure>` and `<figcaption>`**: Used to group media content, such as images, charts, and captions.

---

## 2. **New Form Elements and Attributes**
   HTML5 improved forms with new input types, attributes, and validation features, simplifying form creation.

   ### New Input Types
   - **`<input type="email">`**: Validates for correct email format.
   - **`<input type="url">`**: Accepts and validates URLs.
   - **`<input type="date">`**: Displays a date picker.
   - **`<input type="tel">`**: Accepts phone numbers.
   - **`<input type="number">`**: Allows only numbers with step increments.
   - **`<input type="range">`**: Creates a slider for selecting a range of values.
   - **`<input type="color">`**: Displays a color picker.

   ### New Attributes
   - **`placeholder`**: Specifies a hint within the input field.
   - **`required`**: Makes the field mandatory for form submission.
   - **`autofocus`**: Automatically focuses the input field when the page loads.
   - **`autocomplete`**: Allows the browser to suggest and fill in user details based on previous entries.
   - **`pattern`**: Defines a regex pattern for custom input validation.
   - **`min`, `max`, `step`**: Define numeric ranges for inputs.

---

## 3. **Media Elements (Audio and Video)**
   HTML5 introduced native support for audio and video elements without needing plugins like Flash.

   - **`<audio>`**: Embeds audio content with attributes like `controls`, `autoplay`, `loop`, and `muted`.
     ```html
     <audio controls>
       <source src="audio.mp3" type="audio/mpeg">
       Your browser does not support the audio element.
     </audio>
     ```

   - **`<video>`**: Embeds video content with attributes like `controls`, `autoplay`, `loop`, `poster` (preview image).
     ```html
     <video controls>
       <source src="video.mp4" type="video/mp4">
       Your browser does not support the video element.
     </video>
     ```

---

## 4. **Canvas and SVG for Graphics**
   HTML5 supports drawing and animations directly on the web page.

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

---

## 5. **HTML5 APIs**

   ### Geolocation API
   - Retrieves the geographical location of the user.
     ```javascript
     navigator.geolocation.getCurrentPosition(function(position) {
       console.log("Latitude: " + position.coords.latitude);
       console.log("Longitude: " + position.coords.longitude);
     });
     ```

   ### Web Storage API
   - Stores data on the client side.
     - **Local Storage**: Persistent storage until manually cleared.
       ```javascript
       localStorage.setItem('key', 'value');
       let data = localStorage.getItem('key');
       ```
     - **Session Storage**: Data stored only for the session.
       ```javascript
       sessionStorage.setItem('key', 'value');
       ```

   ### Web Workers
   - Runs JavaScript in background threads, helping to offload tasks.
     ```javascript
     let worker = new Worker('worker.js');
     worker.postMessage('Hello');
     ```

   ### Drag and Drop API
   - Enables dragging and dropping of elements.
     ```html
     <div draggable="true" ondragstart="drag(event)">Drag me</div>
     ```

   ### History API
   - Manipulates browser history.
     ```javascript
     history.pushState({ page: 1 }, "title 1", "?page=1");
     ```

---

## 6. **Microdata and Accessibility Features**
   - **Microdata**: Embeds structured data in HTML, improving SEO.
     ```html
     <div itemscope itemtype="https://schema.org/Person">
       <span itemprop="name">John Doe</span>
     </div>
     ```
   - **ARIA (Accessible Rich Internet Applications)**: Adds accessibility attributes.
     ```html
     <button aria-label="Close" onclick="close()">X</button>
     ```

---

## 7. **Progress and Meter Elements**
   HTML5 introduced new elements to visually represent values.

   - **`<progress>`**: Displays the completion progress of a task.
     ```html
     <progress value="70" max="100">70%</progress>
     ```
   - **`<meter>`**: Represents a scalar measurement within a known range.
     ```html
     <meter min="0" max="100" value="50">50%</meter>
     ```

---

## 8. **Other Useful Elements**
   - **`<datalist>`**: Provides an autocomplete feature for an input.
     ```html
     <input list="browsers" name="browser">
     <datalist id="browsers">
       <option value="Chrome">
       <option value="Firefox">
     </datalist>
     ```
   - **`<output>`**: Displays the result of a calculation or user action.
     ```html
     <output name="result" for="a b">0</output>
     ```

---

## Interview Tips
1. **Know When to Use Each Element**: Understand the purpose of each semantic element and when to apply it in layouts.
2. **Explain API Use Cases**: Be able to describe practical uses of APIs like Web Storage, Canvas, and Geolocation.
3. **Demonstrate Code Snippets**: Familiarize yourself with basic code snippets to quickly explain new input types and validation.
4. **Understand Accessibility**: Know how ARIA attributes and semantic HTML improve accessibility.
5. **Practice with Canvas and SVG**: Front-end roles often require basic graphics knowledge, so practice creating simple shapes.

These notes should serve as a solid foundation for your HTML5 knowledge!