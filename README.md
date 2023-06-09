# **_`Lecture-6`_**

# **`TABLE OF CONTENTS`**

- [Window](#window)
- [DOM](#dom)
- [BOM](#bom)
- [HTML Events](#html-events)
- [JavaScript DOM methods](#javascript-dom-methods)

# **`Window`**

![](/img/JavaScript-Window-Object.jpg)

## **`What is Window in JavaScript`**

---

In JavaScript, the window object represents the current browser window or tab. It is a global object that provides access to various properties and methods related to the browser window environment.

Some of the common properties and methods of the window object include:

**`Properties`**

- `window.document`: Represents the HTML document that is currently loaded in the browser window.

- `window.innerHeight`: Returns the height of the browser window viewport, in pixels.

- `window.innerWidth`: Returns the width of the browser window viewport, in pixels.

- `window.location`: Provides information about the URL of the current page, and allows you to navigate to a new URL if needed.

- `window.navigator`: Provides information about the user's browser and platform.

- `window.screen`: Provides information about the user's screen resolution and display settings.

- `window.localStorage`: Allows you to store data locally on the user's computer.

**`Methods`**

- `window.alert()`: Displays an alert box with a message and an OK button.

- `window.confirm()`: Displays a confirmation box with a message and OK/Cancel buttons.

- `window.prompt()`: Displays a prompt box with a message and an input field for the user to enter text.

- `window.open()`: Opens a new browser window or tab.

- `window.close()`: Closes the current browser window.

- `window.setTimeout()`: Sets a timer that will execute a function after a specified delay.

- `window.setInterval()`: Sets a recurring timer that will execute a function at a specified interval.

There are many more properties and methods available on the window object, but these are some of the most commonly used ones.

<br>
<br>
<br>

# **`DOM`**

![](/img/Javascript-DOM.jpg)

## **`What is the DOM in JavaScript`**

The Document Object Model (DOM) in JavaScript is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents an HTML or XML document as a tree structure where each node represents a part of the document, such as an element, attribute, or text.

With the DOM, programmers can modify the content and structure of a web page dynamically, after it has loaded in the browser. For example, you could use JavaScript to add new elements, change the styling of existing elements, or respond to user interactions like button clicks.

![](/img/what-is-document-object-model-in-JS-featured-image.jpg)

---

## **`The DOM tree structure`**

![](/img/image.png)

<br>
<br>
<br>

# **`JavaScript DOM methods`**

JavaScript DOM (Document Object Model) methods are built-in functions that can be used to perform operations on HTML or XML elements in a web page. These methods can be called on a DOM object to manipulate, modify, or retrieve information about the element or its children.

Some of the most commonly used DOM methods in JavaScript include:

1. `getElementById()`: returns the element with the specified ID.

2. `getElementsByClassName()`: returns a collection of elements with the specified class name.

3. `getElementsByTagName()`: returns a collection of elements with the specified tag name.

4. `querySelector()`: returns the first element that matches a specified CSS selector.

5. `querySelectorAll()`: returns a collection of all elements that match a specified CSS selector.

6. `appendChild()`: adds a new child node to an element.

7. `removeChild()`: removes a child node from an element.

8. `setAttribute()`: sets the value of an attribute on an element.

9. `getAttribute()`: gets the value of an attribute on an element.

10. `innerHTML`: sets or gets the content of an element as HTML.

These methods allow developers to create dynamic and interactive web pages by manipulating the content, structure, and styling of HTML and XML documents. By using these built-in functions, JavaScript developers can write code that interacts with the web page directly, without having to reload the entire page.

<br>

## **`innerHTML`**

`innerHTML` is a property of DOM elements in JavaScript that allows you to get or set the HTML content inside an element. This property can be used to dynamically update the contents of an HTML element on a web page.

Here's an example of how to use `innerHTML` to set the content of a `<div>` element:

![](/img/1ex.png)

In this example, we first retrieve the `<div>` element by its ID using the `getElementById()` method. We then set the `innerHTML` property of the element to a string containing some HTML code. The new HTML code will replace any previous content inside the `<div>` element.

You can also use `innerHTML` to get the current HTML content of an element:

![](/img/2.ex.png)

In this example, we get the `<div>` element again and then read the `innerHTML` property to get the current HTML content.

Note that when you use `innerHTML` to set the content of an element, be careful about possible security vulnerabilities such as cross-site scripting (XSS) attacks. It's important to sanitize any user-generated content before inserting it into the HTML with `innerHTML`.

<br>

## **`The createElement() Methods`**

`createElement()` is a built-in JavaScript method used to create a new element node in the Document Object Model (DOM). This method allows you to dynamically generate new HTML elements and add them to a web page.

Here's an example of using `createElement()` to create a new `<div>` element:

![](/img/3ex.png)

In this example, we use the `createElement()` method to create a new `<div>` element. We then set the `textContent` property of the new element to "This is a new div element!". Finally, we use the `appendChild()` method to add the new `<div>` element to the end of the `<body>` element on the page.

The `createElement()` method can be used to create any type of HTML element, such as `<p>`, `<img>`, `<button>`, or even custom elements that you have defined in your own JavaScript code. You simply pass the name of the element as a string argument to the `createElement()` method.

Once you have created a new element with `createElement()`, you can modify its properties and add it to the DOM using other methods like `setAttribute()`, `appendChild()`, `insertBefore()`, etc.

<br>

## **`The appendChild() Methods`**

`appendChild()` is a built-in JavaScript method used to add a new child node to the end of a DOM (Document Object Model) element. This method allows you to dynamically add HTML elements to an existing webpage.
`Here's an example of using`appendChild()` to add a new element to an existing DOM element:

![](/img/4.png)

In this example, we first retrieve the parent element using the `getElementById()` method. We then create a new `<div>` element using the `createElement()` method and set its text content to "This is a new element!". Finally, we use the `appendChild()` method to add the new element as a child of the parent element.

Note that `appendChild()` adds the new child element at the end of the list of existing child nodes. If you want to add the new element at a specific position, you can use the `insertBefore()` method instead.

<br>

## **`classlist()`**

`classlist()` is not a built-in JavaScript function. However, there is a built-in property in JavaScript called `classList` which is available on DOM elements. It is used to manipulate the class attribute of an element.

The `classList` property returns an object that represents the class attribute of an element as a collection of individual strings. The object has several methods which can be used to add or remove classes from the element's class attribute.

Here are some examples of how you can use `classList`:

To add a class to an element:

![](/img/5.png)

To remove a class from an element:

![](/img/6.png)

To toggle a class on an element:

![](/img/7.png)

Note that the `classList` property is only available on DOM elements and not on other types of objects.

<br>
<br>
<br>

# **`BOM`**

![](/img/Browser-Object-Model.jpg)

`BOM (Browser Object Model)` is a set of JavaScript APIs that allow for access and manipulation of the browser window. The BOM includes objects such as `window`, `screen`, `location`, `history`, and `navigator`, among others.

Here's an example of how you might use the BOM to open a new browser window:

![](/img/bom.png)

In this code, `window.open()` is used to create a new window with the URL "http://www.example.com". The second argument, `'_blank'`, specifies that the new window should be opened in a new tab or window. Finally, the third argument sets the size of the new window to 500 pixels by 500 pixels.

Other BOM APIs can be used for tasks such as manipulating the browser history, getting information about the user's device and browser, and more.

<br>
<br>
<br>

# **`HTML Events`**

![](/img/HTML-Event-2-main.png)

HTML events are actions or occurrences that take place in the HTML document, such as a button being clicked, a page loaded or refreshed, or user input entered into a form. These events can trigger JavaScript code to perform specific tasks, such as updating the content on the webpage or interacting with other web elements.

Some common HTML events include:

- `onclick`: triggered when an element is clicked

- `onsubmit`: triggered when a form is submitted

- `onload`: triggered when a webpage finishes loading

- `onmouseover`: triggered when the mouse pointer moves over an element

- `onkeydown`: triggered when a key is pressed down

HTML events can be added to an element using the "on" attribute followed by the event name and the code to execute within quotes. For example, to add an onclick event to a button element, you could write:

![](/img/11.png)

This would display an alert message when the button is clicked.
