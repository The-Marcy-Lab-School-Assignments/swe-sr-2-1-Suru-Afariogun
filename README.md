# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Do some research on semantic and non-semantic elements and share your findings. Your response should include:

- Examples of semantic and non-semantic tags
- The differences between semantic and non-semantic tags
- The benefits of using semantic tags (when possible)

### Response 1

Semantic elements in HTML clearly describe their meaning both to the browser and developers, improving readability and accessibility. Non-semantic elements, on the other hand, do not convey any meaning about their content.
some examples include:
-Semantic Tags: `<header>`, `<article>`, `<section>`, `<nav>`, `<footer>`, `<aside>`, `<figure>`
-Non-Semantic Tags: `<div>`, `<span>`
The differences is that semantic elements improve readability and accessibility, making it easier to understand the document structure. On the other hand non-semantic elements provide no meaning and are usually used for styling or JavaScript interactions. some benefits of Semantic Tags include, better Accessibility, with things like Assistive technologies (such as screen readers) using semantic elements to interpret page structures. Search engines are able to better understand the content, improving rankings. And finally, enhanced maintainability in which developers can quickly comprehend the document's structure, making code easier to update.

## Prompt 2

Do some research on accessibility. What are some ways to make your website more accessible? Explain why it is important for developers to create websites that meet accessibility standards.

### Response 2

Accessibility ensures that websites are usable by all individuals, including those with disabilities. A well-designed website accommodates users with visual, auditory, motor, and cognitive impairments by incorporating best practices that enhance usability. Proper HTML semantics, such as using `<header>`, `<nav>`, and `<main>`, improve navigation for screen readers. Adding alternative text (`alt`) to images helps visually impaired users understand visual content, while ensuring keyboard navigation allows users to interact with all elements using keys like `tab`. Implementing ARIA (Accessible Rich Internet Applications) attributes enhances the interpretation of dynamic content for assistive technologies, and maintaining sufficient contrast between text and background improves readability for users with vision impairments. Prioritizing accessibility ensures equal access to web content for all users, helps businesses comply with legal standards such as ADA and WCAG, and enhances search engine optimization (SEO) and overall user experience.

## Prompt 3

It is possible to add "inline" CSS styles to our html elements using the `style` attribute like so:

```html
<p style="color: red;">hello world</p>
```

While this is possible, it is a best practice to instead write styles in a separate CSS file. Provide at least one argument for why it _might_ be considered useful to write inline styles, and then provide a more compelling argument for writing styles in a separate CSS file.

### Response 3

Inline styles can be useful for quick fixes or testing styles on a single element. They are also helpful when applying unique styles that do not need to be reused elsewhere. However, using external CSS is generally a better practice because it keeps HTML clean and organized by separating content from design. It also makes maintenance easier, as changes made in a single CSS file apply to multiple pages. Additionally, external stylesheets improve website performance since browsers can cache them, reducing page load times. While inline styles have their place in specific situations, external stylesheets are the preferred approach for creating scalable and maintainable websites.

## Prompt 4

Imagine you are teaching a brand new programmer a brief lesson about the `class` and `id` attributes in HTML as well as how to use them to style elements using CSS. Your lesson should have the following components:

- An explanation of the concept of "classes" and "ids" with an analogy.
- An example of the usage using an HTML code block and a CSS code block.
- An explanation of the syntax using the terms: **attribute**, **selector**

### Response 4

An id in HTML is like a unique ID card assigned to one person, meaning it is used for a single element. On the other hand, a class is like a school uniform worn by many students, allowing multiple elements to share the same style.

```html
<div id="main-header" class="header">Welcome to My Website</div>
<p class="content">
  This is a paragraph with the same class as other paragraphs.
</p>
<p class="content">Another paragraph with the same class.</p>
```

```css
#main-header {
  background-color: blue;
  color: white;
}

.content {
  font-size: 16px;
  color: black;
}
```

In the example code, the <div> element has an id="main-header" and a class="header", while multiple <p> elements share the class="content". In CSS, #main-header targets the unique id, applying a blue background and white text, while .content styles all paragraphs with a font size of 16px and black text. The id attribute uniquely identifies an element and is selected using #id-name in CSS. The class attribute allows multiple elements to share a style and is selected using .class-name. The selector in CSS (like #main-header and .content`) determines which elements the styles apply to.

## Prompt 5

The Document Object Model (DOM) API provides functions for manipulating HTML documents. It is possible to build an entire website using only JavaScript and the DOM API, however is that the best practice?

When building a website, how can I decide which content I should write using HTML/CSS and which content I should create using the JavaScript and the DOM API?

### Response 5

While JavaScript and the DOM API enable dynamic modifications, it is best to use HTML and CSS for static content and rely on JavaScript for interactive elements. HTML and CSS should handle static content like text, headings, images, and overall page structure, as well as styling and layout, including colors, fonts, and positioning. JavaScript and the DOM API are best used for dynamic content, such as fetching new data or processing user inputs, and for interactive elements, like form validation, animations, and event handling. The best practice is to use HTML and CSS for structure and design while reserving JavaScript for interactivity and real-time updates, ensuring better performance and easier maintenance.
