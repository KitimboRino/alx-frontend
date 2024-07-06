# HTML Guidelines and Best Practices

## Introduction

Welcome to the HTML guidelines and best practices guide! This document aims to provide you with a comprehensive understanding of HTML, from the basics of creating a skeleton HTML5 page to integrating various types of media and structuring your content semantically. Whether you're a beginner or looking to improve your HTML skills, this guide will help you create well-structured and accessible web pages.

## Table of Contents

1. [Guidelines to Follow for HTML](#guidelines-to-follow-for-html)
2. [Creating the Skeleton of an HTML5 Page](#creating-the-skeleton-of-an-html5-page)
3. [Using Semantic HTML Tags to Structure a Web Page](#using-semantic-html-tags-to-structure-a-web-page)
4. [Use Cases for `div` vs `span`](#use-cases-for-div-vs-span)
5. [Semantic Values of `header`, `main`, `footer`, `article`, `nav`, `section`, `aside`](#semantic-values-of-header-main-footer-article-nav-section-aside)
6. [Using Headings and Their Hierarchical Order](#using-headings-and-their-hierarchical-order)
7. [Creating Lists in HTML](#creating-lists-in-html)
8. [Differences Between Media Types (SVG, GIF, PNG, JPG)](#differences-between-media-types-svg-gif-png-jpg)
9. [Structuring Data in a Table](#structuring-data-in-a-table)
10. [Integrating a Video in a Webpage](#integrating-a-video-in-a-webpage)
11. [Integrating an Audio File in a Webpage](#integrating-an-audio-file-in-a-webpage)
12. [Embedding External Content](#embedding-external-content)
13. [Correctly Structuring an HTML Page](#correctly-structuring-an-html-page)

## Guidelines to Follow for HTML

- **Use Semantic HTML:** Always use semantic tags to give meaning to your content.
- **Keep Code Clean and Organized:** Indent your code properly and use comments where necessary.
- **Follow Accessibility Best Practices:** Ensure your web pages are accessible to all users, including those with disabilities.
- **Use External Stylesheets and Scripts:** Keep your HTML clean by using external CSS and JavaScript files.
- **Validate Your HTML:** Use tools like the W3C Markup Validation Service to check for errors.

## Creating the Skeleton of an HTML5 Page

To create the skeleton of an HTML5 page, you need the following basic structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

## Using Semantic HTML Tags to Structure a Web Page

Semantic HTML tags provide meaning to the content they enclose. Here are some common semantic tags and their uses:

- `<header>`: Represents introductory content or a set of navigational links.
- `<main>`: Represents the dominant content of the `<body>`.
- `<footer>`: Represents the footer for its nearest sectioning content or sectioning root element.
- `<article>`: Represents a self-contained composition in a document, page, or site.
- `<nav>`: Represents a section of a page that links to other pages or to parts within the page.
- `<section>`: Represents a standalone section that can be distributed independently.
- `<aside>`: Represents a section of content that is tangentially related to the content around it.

## Use Cases for `div` vs `span`

- **`div`**: A block-level container used to group other elements. Use it for layout purposes.
  ```html
  <div>
      <p>Some text</p>
  </div>
  ```
- **`span`**: An inline container used to group text or other inline elements. Use it for styling a part of the text.
  ```html
  <p>This is a <span class="highlight">highlighted</span> text.</p>
  ```

## Semantic Values of `header`, `main`, `footer`, `article`, `nav`, `section`, `aside`

- **`header`**: Contains introductory content or navigational links.
  ```html
  <header>
      <h1>Website Title</h1>
      <nav>
          <ul>
              <li><a href="#">Home</a></li>
              <li><a href="#">About</a></li>
          </ul>
      </nav>
  </header>
  ```
- **`main`**: Contains the main content of the document.
  ```html
  <main>
      <article>
          <h2>Article Title</h2>
          <p>Article content goes here.</p>
      </article>
  </main>
  ```
- **`footer`**: Contains footer content like copyright information or links.
  ```html
  <footer>
      <p>&copy; 2024 Your Website</p>
  </footer>
  ```
- **`article`**: Represents a self-contained piece of content.
  ```html
  <article>
      <h2>Article Title</h2>
      <p>Article content goes here.</p>
  </article>
  ```
- **`nav`**: Contains navigational links.
  ```html
  <nav>
      <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
      </ul>
  </nav>
  ```
- **`section`**: Represents a standalone section.
  ```html
  <section>
      <h2>Section Title</h2>
      <p>Section content goes here.</p>
  </section>
  ```
- **`aside`**: Contains content tangentially related to the main content.
  ```html
  <aside>
      <p>Related information or advertisements go here.</p>
  </aside>
  ```

## Using Headings and Their Hierarchical Order

Headings (`<h1>` to `<h6>`) should follow a hierarchical order to maintain the document's structure and accessibility.

Example:
```html
<h1>Main Title</h1>
<h2>Subsection Title</h2>
<h3>Sub-subsection Title</h3>
```

## Creating Lists in HTML

- **Ordered List**: Uses `<ol>` for creating a numbered list.
  ```html
  <ol>
      <li>First item</li>
      <li>Second item</li>
  </ol>
  ```
- **Unordered List**: Uses `<ul>` for creating a bulleted list.
  ```html
  <ul>
      <li>First item</li>
      <li>Second item</li>
  </ul>
  ```
- **Definition List**: Uses `<dl>`, `<dt>`, and `<dd>` for creating a list of terms and definitions.
  ```html
  <dl>
      <dt>Term</dt>
      <dd>Definition of the term.</dd>
  </dl>
  ```

## Differences Between Media Types (SVG, GIF, PNG, JPG)

- **SVG**: Scalable Vector Graphics, used for vector images, resolution-independent.
- **GIF**: Graphics Interchange Format, supports animation, limited to 256 colors.
- **PNG**: Portable Network Graphics, lossless compression, supports transparency.
- **JPG**: Joint Photographic Experts Group, lossy compression, best for photographs.

## Structuring Data in a Table

Use the `<table>` element to structure tabular data.

Example:
```html
<table>
    <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
    </tbody>
</table>
```

## Integrating a Video in a Webpage

Use the `<video>` element to embed a video.

Example:
```html
<video controls>
    <source src="video.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
```

## Integrating an Audio File in a Webpage

Use the `<audio>` element to embed an audio file.

Example:
```html
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    Your browser does not support the audio tag.
</audio>
```

## Embedding External Content

Use the `<iframe>` element to embed external content like a map or a video from another site.

Example:
```html
<iframe src="https://www.example.com" width="600" height="400"></iframe>
```

## Correctly Structuring an HTML Page

A well-structured HTML page uses semantic tags and follows a logical order.

Example:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <header>
        <h1>Website Title</h1>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section>
            <h2>Section Title</h2>
                <p>Section content goes here.</p>
            <article>
                <h3>Article Title</h3>
                <p>Article content goes here.</p>
            </article>
        </section>
        <aside>
            <h2>Related Information</h2>
            <p>Related content or advertisements go here.</p>
        </aside>
    </main>
    <footer>
        <p>&copy; 2024 Your Website</p>
    </footer>
</body>
</html>

Conclusion
This guide provides a comprehensive overview of best practices and guidelines for writing clean, well-structured, and accessible HTML. By following these guidelines,  you can ensure your web pages are easy to read, maintain, and accessible to all users. Happy coding!
