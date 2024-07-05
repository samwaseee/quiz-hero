Interview Questions


### JavaScript Questions

1. **What is the difference between `==` and `===` in JavaScript?**
   - `==` compares values for equality after converting both values to a common type (type coercion), while `===` compares both value and type without performing type conversion.

2. **Explain closures in JavaScript.**
   - A closure is a function that retains access to its lexical scope even when the function is executed outside that scope. This allows functions to access variables from an enclosing scope, even after that scope has finished executing.

3. **What is the `this` keyword and how is it used?**
   - `This` refers to the object that is executing the current function. Its value is determined by how a function is called:
     - In a method, `this` refers to the owner object.
     - In a function, `this` refers to the global object (or `undefined` in strict mode).
     - In an arrow function, `this` retains the value of the enclosing lexical context's `this`.

4. **What are Promises and how do you use them?**
   - Promises are objects that represent the eventual completion (or failure) of an asynchronous operation and its resulting value. They have three states: pending, fulfilled, and rejected. Use `.then()`, `.catch()`, and `.finally()` to handle the results.

5. **Explain the difference between `var`, `let`, and `const`.**
   - `var` h has globally scoped or function scoped and is hoisted to the top of its scope. they are available for use throughout the entire window. can re-declare and update.
   - `let` has block scope and is not hoisted.
   - `const` has block scope and is not hoisted; it also cannot be reassigned after its initial assignment.

6. **What are higher-order functions in JavaScript?**
   - Higher-order functions are functions that can take other functions as arguments or return functions as their result. Examples include `map()`, `filter()`, and `reduce()`.

7. **Explain the event loop in JavaScript.**
   - The event loop is a mechanism that handles asynchronous callbacks. It allows JavaScript to perform non-blocking operations by offloading operations to the system kernel whenever possible.

8. **What is hoisting in JavaScript?**
   - Hoisting is JavaScript's behavior of moving declarations (functions, variables) to the top of their containing scope during compilation. Only the declarations are hoisted, not the initializations.

9. **Explain the concept of prototypal inheritance.**
   - Prototypal inheritance is a feature in JavaScript where objects can inherit properties and methods from other objects. Each object has a `__proto__` property that points to its prototype object.

10. **What are modules in JavaScript and how do you use them?**
    - Modules are reusable pieces of code that can be imported and exported between files. They help in organizing code and avoiding global scope pollution. ES6 introduced `import` and `export` syntax for modules.

11. **What are arrow functions, and how do they differ from regular functions?**
    - Arrow functions are a concise syntax for writing functions using the `=>` syntax. They differ from regular functions in that they do not have their own `this`, `arguments`, `super`, or `new.target` bindings. They are best suited for non-method functions.

12. **Explain the concept of asynchronous programming in JavaScript.**
    - Asynchronous programming allows JavaScript to perform long-running tasks without blocking the main thread. This is achieved using callbacks, Promises, async/await, and event-driven APIs.

13. **What is the difference between `null` and `undefined`?**
    - `undefined` means a variable has been declared but not assigned a value.
    - `null` is an assignment value that represents no value or no object.

14. **How does JavaScript handle errors?**
    - JavaScript uses `try...catch` blocks to handle exceptions. The `try` block contains code that might throw an error, and the `catch` block contains code to handle the error.

15. **What is event delegation?**
    - Event delegation is a technique where a single event listener is added to a parent element to manage events from its child elements. This is efficient because it reduces the number of event listeners and takes advantage of event bubbling.

16. **What is the difference between `apply()`, `call()`, and `bind()`?**
    - `call()` invokes a function with a given `this` value and arguments provided individually.
    - `apply()` is similar to `call()`, but arguments are provided as an array.
    - `bind()` returns a new function, permanently bound to the provided `this` value and arguments.

17. **What are JavaScript data types?**
    - JavaScript has the following data types: Primitive types (Number, String, Boolean, Null, Undefined, Symbol, and BigInt) and Reference types (Object, Array, Function, Date, RegExp, etc.).

18. **What is the `new` keyword in JavaScript?**
    - The `new` keyword creates an instance of a user-defined object type or one of the built-in object types. It sets up the prototype chain so that the new object inherits from the constructor's prototype.

19. **Explain the `Object.create()` method.**
    - `Object.create()` creates a new object with a specified prototype object and properties. It allows for more precise control over the properties that will be added to the new object.

20. **What is a promise chain?**
    - A promise chain is a sequence of `.then()` methods chained together to handle multiple asynchronous operations in a sequence. Each `then` receives the result of the previous promise.

21. **What are template literals?**
    - Template literals are string literals that allow embedded expressions. They are enclosed by backticks (`) and can contain placeholders indicated by `${expression}`.

22. **What is destructuring assignment?**
    - Destructuring assignment is a syntax that allows you to unpack values from arrays or properties from objects into distinct variables.

23. **What is the spread operator and how is it used?**
    - The spread operator (`...`) allows an iterable (like an array) to be expanded in places where zero or more arguments or elements are expected.

24. **Explain the concept of 'hoisting'.**
    - Hoisting is JavaScript's default behavior of moving declarations (not initializations) to the top of their scope before code execution. This means that variables and function declarations can be used before they are declared.

25. **What is the difference between `undefined` and `undeclared` variables?**
    - `undefined` variables are those that have been declared but not assigned a value.
    - `undeclared` variables are those that have not been declared in the accessible scope.

26. **Explain the difference between synchronous and asynchronous functions.**
    - Synchronous functions are executed in sequence, blocking subsequent code until they finish.
    - Asynchronous functions are executed without blocking subsequent code, often using callbacks, Promises, or async/await.

27. **What is event bubbling and event capturing?**
    - Event bubbling and event capturing are two phases of event propagation in the DOM.
      - Event bubbling: The event starts from the target element and bubbles up to the root.
      - Event capturing: The event starts from the root and captures down to the target element.

28. **How can you prevent event propagation?**
    - Use `event.stopPropagation()` to prevent further propagation of the current event in the capturing and bubbling phases.

29. **What is AJAX?**
    - AJAX (Asynchronous JavaScript and XML) is a technique for creating fast and dynamic web pages. It allows web pages to be updated asynchronously by exchanging data with a web server behind the scenes.

30. **What is the purpose of the `strict mode` in JavaScript?**
    - Strict mode is a way to opt into a restricted variant of JavaScript. It makes debugging easier by throwing errors for silent mistakes, preventing the use of certain syntax, and improving performance.

31. **What are immediately-invoked function expressions (IIFE)?**
    - An IIFE is a JavaScript function that runs as soon as it is defined. It is a design pattern used to avoid polluting the global scope.

32. **How do you check if a variable is an array in JavaScript?**
    - Use `Array.isArray(variable)` to check if a variable is an array.

33. **What are generator functions?**
    - Generator functions are functions that can be exited and later re-entered. Their context (variable bindings) will be saved across re-entrances. They are defined with an asterisk `*` and use the `yield` keyword.

34. **Explain the concept of memoization in JavaScript.**
    - Memoization is an optimization technique used to speed up function calls by caching the results of expensive function calls and returning the cached result when the same inputs occur again.

35. **What is the difference between localStorage, sessionStorage, and cookies?**
    - `localStorage`: Stores data with no expiration date. Data is not sent to the server with every request.
    - `sessionStorage`: Stores data for the duration of the page session. Data is not sent to the server with every request.
    - `cookies`: Store data that is sent to the server with every request. Can have expiration dates.

### React Questions

1. **What is React?**
   - React is a free and open-source front-end JavaScript library for building user interfaces based on components. It is maintained by Meta and a community of individual developers and companies.

2

. **What are components in React?**
   - Components are the building blocks of a React application. They are reusable, isolated pieces of code that represent parts of the user interface.

3. **What is JSX?**
   - JSX is a syntax extension for JavaScript that looks similar to XML or HTML. It allows you to write HTML elements in JavaScript and place them in the DOM.

4. **What is the virtual DOM?**
   - The virtual DOM is a lightweight in-memory representation of the actual DOM. React uses it to optimize updates by comparing the virtual DOM with the real DOM and updating only the changed elements.

5. **What is state in React?**
   - State is an object that holds data or information about the component. It can change over time and is used to create dynamic and interactive components.

6. **What is props in React?**
   - Props (short for properties) are read-only attributes passed from parent components to child components. They allow data to be passed between components.

7. **What is the difference between state and props?**
   - State is local to a component and can change over time, while props are passed from parent to child components and are read-only.

8. **What are hooks in React?**
   - Hooks are functions that let you use state and other React features in functional components. Examples include `useState`, `useEffect`, and `useContext`.

9. **What is the `useState` hook?**
   - The `useState` hook allows you to add state to functional components. It returns a state variable and a function to update it.

10. **What is the `useEffect` hook?**
    - The `useEffect` hook allows you to perform side effects in functional components, such as data fetching, subscriptions, or manually changing the DOM. It runs after the first render and after every update.

11. **What is the difference between class components and functional components?**
    - Class components are ES6 classes that extend `React.Component` and can have state and lifecycle methods. Functional components are simpler functions that can use hooks to manage state and lifecycle.

12. **What is the React context API?**
    - The React context API allows you to share state across the entire app (or part of it) without passing props down through multiple levels of the component tree.

13. **What is a higher-order component (HOC)?**
    - A higher-order component is a function that takes a component and returns a new component with additional props or behavior. It is used to reuse component logic.

14. **What is the purpose of keys in React?**
    - Keys are used to identify elements in lists. They help React identify which items have changed, are added, or are removed, which improves performance during re-renders.

15. **What are controlled components?**
    - Controlled components are form elements whose values are controlled by React state. Their value is set by the state and updated via an onChange event handler.

16. **What are uncontrolled components?**
    - Uncontrolled components are form elements that manage their own state internally. They use a ref to access the DOM elements directly for their current values.

17. **What is React Router?**
    - React Router is a library for routing in React applications. It allows you to create navigation and routes for different components.

18. **What is Redux?**
    - Redux is a state management library for JavaScript applications. It provides a central store for the entire application's state and enforces a predictable state management pattern.

19. **What are the main principles of Redux?**
    - Single source of truth: The state of your whole application is stored in an object tree within a single store.
    - State is read-only: The only way to change the state is to emit an action, an object describing what happened.
    - Changes are made with pure functions: To specify how the state tree is transformed by actions, you write pure reducers.

20. **What is the purpose of middleware in Redux?**
    - Middleware in Redux provides a way to extend Redux with custom functionality. It allows you to handle asynchronous actions, perform logging, dispatch multiple actions, and more.

21. **What is the `useReducer` hook?**
    - The `useReducer` hook is an alternative to `useState` for managing complex state logic. It takes a reducer function and an initial state and returns the current state and a dispatch function.

22. **What is the difference between `useEffect` and `useLayoutEffect`?**
    - `useEffect` runs after the render is committed to the screen, while `useLayoutEffect` runs synchronously after all DOM mutations but before the browser paints. Use `useLayoutEffect` for reading layout and synchronously re-rendering.

23. **What is React.memo?**
    - `React.memo` is a higher-order component that memoizes a component, preventing unnecessary re-renders if the props have not changed.

24. **What is the `useContext` hook?**
    - The `useContext` hook allows you to access the value of a context directly in functional components without using a consumer.

25. **How do you handle forms in React?**
    - Forms in React can be handled using controlled components, where form inputs are tied to the component state, or using uncontrolled components with refs to access input values directly.

26. **What is PropTypes in React?**
    - PropTypes is a type-checking library for React props. It ensures that props passed to a component are of the correct type and can provide warnings during development.

27. **What is the difference between `componentDidMount` and `componentWillMount`?**
    - `componentDidMount` is invoked immediately after a component is mounted and can be used for side effects such as fetching data.
    - `componentWillMount` is deprecated and was used to perform tasks just before mounting, but it is not safe for async code.

28. **What is reconciliation in React?**
    - Reconciliation is the process by which React updates the DOM with the minimal number of changes by comparing the current virtual DOM with the previous one and applying the necessary updates.

29. **What is the difference between `React.createElement` and JSX?**
    - `React.createElement` is the function that creates React elements, whereas JSX is a syntactic sugar that simplifies the process of writing these elements.

30. **How do you optimize performance in a React application?**
    - Performance in React can be optimized by using techniques such as code splitting, memoization, virtualization, avoiding unnecessary re-renders, and using the `React.PureComponent` or `React.memo`.

31. **What is the purpose of `getDerivedStateFromProps`?**
    - `getDerivedStateFromProps` is a static lifecycle method that is invoked right before rendering when new props or state are being received. It is used to update the state based on the props.

32. **What is `React.Fragment` and why is it used?**
    - `React.Fragment` allows you to group multiple elements without adding an extra node to the DOM. It is useful for returning multiple elements from a component render method.

33. **What is the `useRef` hook?**
    - The `useRef` hook returns a mutable ref object that persists across renders. It can be used to access DOM elements directly or store mutable values.

34. **What is server-side rendering (SSR) in React?**
    - Server-side rendering (SSR) is the process of rendering React components on the server and sending the HTML to the client. It improves performance and SEO.

35. **What is static site generation (SSG) in React?**
    - Static site generation (SSG) is a build-time rendering method where pages are pre-rendered as static HTML files, improving performance and scalability.

### HTML Questions

1. **What is HTML?**
   - HTML (HyperText Markup Language) is the standard markup language for creating web pages. It describes the structure of a web page using elements and tags.

2. **What are the new features of HTML5?**
   - HTML5 introduced several new features, including new semantic elements (e.g., `<article>`, `<section>`, `<header>`, `<footer>`), multimedia elements (`<audio>`, `<video>`), form controls, APIs (e.g., Canvas, Web Storage, Geolocation), and more.

3. **What is the difference between block-level and inline elements?**
   - Block-level elements take up the full width of their parent container and start on a new line (e.g., `<div>`, `<p>`, `<h1>`). Inline elements only take up as much width as necessary and do not start on a new line (e.g., `<span>`, `<a>`, `<img>`).

4. **What is the purpose of the `<!DOCTYPE html>` declaration?**
   - The `<!DOCTYPE html>` declaration defines the document type and version of HTML being used. It helps browsers to render the page correctly.

5. **What are semantic HTML elements?**
   - Semantic HTML elements clearly describe their meaning in a human- and machine-readable way. Examples include `<article>`, `<section>`, `<header>`, `<footer>`, and `<nav>`.

6. **What is the difference between `<div>` and `<span>`?**
   - `<div>` is a block-level container used to group other elements, while `<span>` is an inline container used to style a part of the text or group inline elements.

7. **What are HTML attributes?**
   - HTML attributes provide additional information about elements. They are included in the opening tag and usually come in name/value pairs (e.g., `href="https://example.com"`).

8. **What is the `alt` attribute in HTML?**
   -

 The `alt` attribute provides alternative text for an image if it cannot be displayed. It improves accessibility and SEO.

9. **What are the different types of HTML lists?**
   - The different types of HTML lists are:
     - Ordered lists (`<ol>`) for numbered items.
     - Unordered lists (`<ul>`) for bulleted items.
     - Definition lists (`<dl>`) for terms and descriptions.

10. **What is the purpose of the `<head>` element?**
    - The `<head>` element contains meta-information about the HTML document, such as the title, character set, styles, scripts, and other metadata.

11. **What is the `<meta>` tag used for?**
    - The `<meta>` tag provides metadata about the HTML document, such as character encoding, author, description, viewport settings, and more. It is placed inside the `<head>` element.

12. **What is the difference between the `<link>` and `<a>` tags?**
    - The `<link>` tag is used to link external resources, such as stylesheets, and is placed in the `<head>` section. The `<a>` tag is used to create hyperlinks to other pages or parts of the same page.

13. **What is the purpose of the `<form>` element in HTML?**
    - The `<form>` element is used to create a form for user input. It can contain various form controls, such as text fields, checkboxes, radio buttons, and submit buttons.

14. **What are the different types of input fields in HTML?**
    - The different types of input fields include `text`, `password`, `email`, `number`, `date`, `checkbox`, `radio`, `file`, `submit`, `reset`, and more.

15. **What is the purpose of the `<fieldset>` and `<legend>` tags?**
    - The `<fieldset>` tag is used to group related form elements, and the `<legend>` tag provides a caption for the `<fieldset>`, improving form accessibility and organization.

16. **What is the `<label>` tag used for?**
    - The `<label>` tag is used to define a label for an `<input>` element, improving form accessibility. It can be associated with a specific input using the `for` attribute or by nesting the input inside the label.

17. **What are HTML data attributes?**
    - HTML data attributes (`data-*`) allow you to store custom data on any HTML element. They are used to add extra information that can be accessed via JavaScript.

18. **What is the purpose of the `<table>` element in HTML?**
    - The `<table>` element is used to create a table for displaying tabular data. It consists of rows (`<tr>`) and cells (`<td>` for data cells and `<th>` for header cells).

19. **What is the difference between `<thead>`, `<tbody>`, and `<tfoot>`?**
    - `<thead>` groups the header content, `<tbody>` groups the body content, and `<tfoot>` groups the footer content in a table. They help to structure and style table data.

20. **What is the purpose of the `colspan` and `rowspan` attributes in tables?**
    - The `colspan` attribute allows a cell to span multiple columns, and the `rowspan` attribute allows a cell to span multiple rows, improving table layout and readability.

21. **What are the different types of buttons in HTML?**
    - The different types of buttons include `button`, `submit`, and `reset`. The `button` type is a general button, `submit` submits a form, and `reset` resets form fields to their default values.

22. **What is the difference between the `id` and `class` attributes in HTML?**
    - The `id` attribute provides a unique identifier for an element, while the `class` attribute assigns one or more class names to an element for styling and scripting.

23. **What is the purpose of the `viewport` meta tag?**
    - The `viewport` meta tag controls the layout of a webpage on mobile devices. It sets the width, initial scale, and other properties to ensure the page is responsive.

24. **What is the purpose of the `lang` attribute in the `<html>` tag?**
    - The `lang` attribute specifies the language of the HTML document, improving accessibility and search engine optimization.

25. **What is the purpose of the `srcset` attribute in the `<img>` tag?**
    - The `srcset` attribute provides a list of image sources with different resolutions, allowing the browser to choose the most appropriate image based on the device's screen size and resolution.

26. **What is the purpose of the `<noscript>` tag?**
    - The `<noscript>` tag defines content that is displayed if JavaScript is disabled or not supported by the browser, ensuring the page is still functional.

27. **What are the different types of media elements in HTML?**
    - The different types of media elements include `<audio>` for audio content, `<video>` for video content, and `<track>` for text tracks (e.g., subtitles).

28. **What is the purpose of the `preload` attribute in the `<audio>` and `<video>` tags?**
    - The `preload` attribute specifies how the browser should load the media content. It can be `none`, `metadata`, or `auto`, determining whether to preload nothing, only metadata, or the entire file.

29. **What is the purpose of the `autoplay` attribute in the `<audio>` and `<video>` tags?**
    - The `autoplay` attribute specifies that the media should start playing automatically as soon as it is loaded.

30. **What is the `canvas` element used for in HTML5?**
    - The `canvas` element is used to draw graphics and animations using JavaScript. It provides a drawing surface for rendering shapes, text, images, and more.

31. **What is the purpose of the `aria` attributes in HTML?**
    - The `aria` (Accessible Rich Internet Applications) attributes improve accessibility by providing additional information to assistive technologies. Examples include `aria-label`, `aria-hidden`, and `aria-expanded`.

32. **What is the difference between `src` and `href` attributes?**
    - The `src` attribute specifies the source of an embedded resource, such as an image or script, while the `href` attribute specifies the URL of a linked resource, such as a stylesheet or hyperlink.

33. **What is the purpose of the `defer` and `async` attributes in the `<script>` tag?**
    - The `defer` attribute loads the script in the background and executes it after the HTML document has been parsed. The `async` attribute loads the script asynchronously and executes it as soon as it is available.

34. **What is the purpose of the `rel` attribute in the `<link>` tag?**
    - The `rel` attribute specifies the relationship between the current document and the linked resource. Examples include `stylesheet`, `icon`, `preload`, and `alternate`.

35. **What is the `download` attribute in the `<a>` tag used for?**
    - The `download` attribute specifies that the target resource should be downloaded when the hyperlink is clicked, rather than navigating to the resource.

36. **What is the purpose of the `form` attribute in form elements?**
    - The `form` attribute specifies the form element that the input, button, or other form control is associated with, allowing form controls to be placed outside the `<form>` element.

37. **What is the `pattern` attribute in the `<input>` tag used for?**
    - The `pattern` attribute specifies a regular expression that the input value must match for the form to be submitted, providing client-side validation.

38. **What is the purpose of the `autofocus` attribute in form elements?**
    - The `autofocus` attribute automatically focuses the form control when the page loads, improving user experience by directing attention to the input field.

39. **What is the `placeholder` attribute in the `<input>` tag used for?**
    - The `placeholder` attribute provides a hint or example of the expected input value, displaying a short description inside the input field when it is empty.

40. **What is the purpose of the `multiple` attribute in the `<select>` and `<input>` tags?**
    - The `multiple` attribute allows users to select multiple options in a `<select>` element or upload multiple files in an `<input type="file">` element.

41. **What is the difference between the `name` and `id` attributes in form elements?**
    - The `name` attribute is used to reference form data after it is submitted, while the `id` attribute uniquely identifies an element within the HTML document and is used for styling and scripting.

42. **What is the `required` attribute in form elements used for?**
    - The `required` attribute specifies that an input field must be filled out before submitting the form, providing client-side validation.

43. **What is the `novalidate` attribute in the `<form>` tag used for?**
    - The `novalidate` attribute disables form validation when the form is submitted, allowing you to handle validation manually using JavaScript.

44. **What is the purpose of the `accept` attribute in the `<input type="file">` tag?**
    - The `accept` attribute specifies the types of files that the server accepts, providing a filter for the file input field.

45. **What is the purpose of the `<datalist>` element in HTML?**
    - The `<datalist>` element provides a list of predefined options for

 an `<input>` element, allowing users to choose from a set of suggestions while typing.

46. **What is the `readonly` attribute in form elements used for?**
    - The `readonly` attribute makes the input field non-editable, but the user can still select and copy the value. It is useful for displaying data that should not be modified.

47. **What is the `disabled` attribute in form elements used for?**
    - The `disabled` attribute makes the input field non-editable and non-interactive, preventing user input and form submission.

48. **What is the `step` attribute in the `<input type="number">` tag used for?**
    - The `step` attribute specifies the legal number intervals for the input value, providing control over the range of acceptable values.

49. **What is the `min` and `max` attributes in the `<input>` tag used for?**
    - The `min` and `max` attributes define the minimum and maximum values for the input field, providing constraints for numerical and date inputs.

50. **What is the purpose of the `formaction` attribute in the `<button>` and `<input type="submit">` tags?**
    - The `formaction` attribute specifies the URL that processes the form submission, allowing different form actions for individual buttons within the same form.

By studying and understanding these questions and answers, you will be well-prepared for your front-end developer interview. Additionally, practicing coding exercises and building projects will help reinforce your knowledge and skills.


