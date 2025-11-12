# HTML Tags Explanation

This document explains all the HTML tags used in the `index.html` file and their purposes.

## Document Structure Tags

### `<!DOCTYPE html>`
- **Purpose**: Document type declaration
- **Description**: Tells the browser that this is an HTML5 document. Must be the first line in an HTML document.
- **Usage**: `<!DOCTYPE html>`

### `<html>`
- **Purpose**: Root element of an HTML page
- **Description**: Contains all other HTML elements. The `lang` attribute specifies the language of the document (e.g., "en" for English).
- **Attributes**: 
  - `lang`: Specifies the language of the document
- **Usage**: `<html lang="en">...</html>`

### `<head>`
- **Purpose**: Container for metadata and document information
- **Description**: Contains elements that provide information about the document but are not displayed on the page (title, meta tags, links to stylesheets, etc.).
- **Usage**: `<head>...</head>`

### `<body>`
- **Purpose**: Contains the visible content of the web page
- **Description**: All content that users see on the webpage is placed inside the `<body>` tag.
- **Usage**: `<body>...</body>`

## Metadata Tags

### `<meta>`
- **Purpose**: Provides metadata about the HTML document
- **Description**: Used to specify character encoding, viewport settings, author information, and more. Not displayed on the page but important for browsers and search engines.
- **Attributes**:
  - `charset`: Specifies the character encoding (UTF-8 is standard)
  - `name`: Specifies the name of the metadata
  - `content`: Specifies the value of the metadata
- **Usage**: 
  - `<meta charset="UTF-8" />` - Sets character encoding
  - `<meta name="viewport" content="width=device-width, initial-scale=1.0" />` - Sets viewport for responsive design

### `<title>`
- **Purpose**: Sets the title of the document
- **Description**: The text appears in the browser tab/title bar and is used by search engines. Should be descriptive and unique for each page.
- **Usage**: `<title>Web Development I – Group Portfolio</title>`

## Semantic Structure Tags

### `<header>`
- **Purpose**: Defines a header section for a document or section
- **Description**: Typically contains introductory content, navigation, or logos. Provides semantic meaning to the header area.
- **Usage**: `<header>...</header>`

### `<main>`
- **Purpose**: Specifies the main content of the document
- **Description**: Should contain the primary content unique to the page. There should be only one `<main>` element per page.
- **Usage**: `<main>...</main>`

### `<section>`
- **Purpose**: Defines a section in a document
- **Description**: Represents a thematic grouping of content. Used to organize content into logical sections.
- **Attributes**:
  - `id`: Provides a unique identifier for the section
- **Usage**: `<section id="introduction">...</section>`

### `<footer>`
- **Purpose**: Defines a footer for a document or section
- **Description**: Typically contains copyright information, contact details, or links to related documents.
- **Usage**: `<footer>...</footer>`

### `<div>`
- **Purpose**: Generic container element
- **Description**: A block-level container used to group elements for styling or organizational purposes. Has no semantic meaning on its own.
- **Attributes**:
  - `class`: Specifies one or more class names for styling or JavaScript
- **Usage**: `<div class="leader-highlight">...</div>`

## Heading Tags

### `<h1>`
- **Purpose**: Main heading (Level 1)
- **Description**: The highest level heading, typically used once per page for the main title. Should represent the primary topic of the page.
- **Usage**: `<h1>Web Development I — Team Horizon</h1>`

### `<h2>`
- **Purpose**: Subheading (Level 2)
- **Description**: Second-level heading used for major sections. Should be used in hierarchical order (h1, then h2, then h3, etc.).
- **Usage**: `<h2>Course & Group Introduction</h2>`

## Text Content Tags

### `<p>`
- **Purpose**: Defines a paragraph
- **Description**: Used to group related text content into paragraphs. Browsers automatically add spacing before and after paragraphs.
- **Attributes**:
  - `class`: Specifies one or more class names
- **Usage**: `<p>This is a paragraph of text.</p>`

### `<strong>`
- **Purpose**: Indicates strong importance or emphasis
- **Description**: Renders text in bold and indicates that the content is of strong importance. Both visually and semantically emphasizes text.
- **Usage**: `<strong>Group Leader: Abena Mensah</strong>`

## List Tags

### `<ul>`
- **Purpose**: Defines an unordered (bulleted) list
- **Description**: Creates a list where items are marked with bullets. Used when the order of items doesn't matter.
- **Attributes**:
  - `class`: Specifies one or more class names
- **Usage**: `<ul class="members-list">...</ul>`

### `<ol>`
- **Purpose**: Defines an ordered (numbered) list
- **Description**: Creates a list where items are numbered sequentially. Used when the order of items is important.
- **Usage**: `<ol>...</ol>`

### `<li>`
- **Purpose**: Defines a list item
- **Description**: Represents an item in a list (either ordered `<ol>` or unordered `<ul>`). Each list item is contained within list tags.
- **Attributes**:
  - `class`: Specifies one or more class names
- **Usage**: `<li>First item</li>`

## Media Tags

### `<img>`
- **Purpose**: Embeds an image in the document
- **Description**: Displays images on the webpage. The image is referenced by its source URL or file path.
- **Attributes**:
  - `src`: Specifies the URL or path to the image file
  - `alt`: Provides alternative text if the image cannot be displayed (important for accessibility)
- **Usage**: `<img src="image.jpg" alt="Description of image" />`
- **Note**: This is a self-closing tag (void element)

### `<figure>`
- **Purpose**: Represents self-contained content with optional caption
- **Description**: Used to group media content (images, videos, diagrams) with a caption. Provides semantic meaning that the content and caption are related.
- **Usage**: `<figure>...</figure>`

### `<figcaption>`
- **Purpose**: Defines a caption for a `<figure>` element
- **Description**: Provides a caption or explanation for the content in the `<figure>` tag. Should be placed inside the `<figure>` element.
- **Usage**: `<figcaption>Caption text</figcaption>`

### `<video>`
- **Purpose**: Embeds video content in the document
- **Description**: Displays video players with controls. Supports multiple video formats through the `<source>` tag.
- **Attributes**:
  - `controls`: Adds video controls (play, pause, volume, etc.)
  - `poster`: Specifies an image to show before the video plays
- **Usage**: `<video controls poster="image.jpg">...</video>`

### `<source>`
- **Purpose**: Specifies media resources for media elements
- **Description**: Used inside `<video>` and `<audio>` elements to specify multiple media source files. The browser will use the first supported format.
- **Attributes**:
  - `src`: Specifies the URL or path to the media file
  - `type`: Specifies the MIME type of the media resource
- **Usage**: `<source src="video.mp4" type="video/mp4" />`
- **Note**: This is a self-closing tag (void element)

### `<audio>`
- **Purpose**: Embeds audio content in the document
- **Description**: Displays audio players with controls. Supports multiple audio formats through the `<source>` tag.
- **Attributes**:
  - `controls`: Adds audio controls (play, pause, volume, etc.)
- **Usage**: `<audio controls>...</audio>`

## Link Tag

### `<a>`
- **Purpose**: Defines a hyperlink
- **Description**: Creates clickable links that navigate to other pages, files, or sections. Can link to external websites or internal page sections.
- **Attributes**:
  - `href`: Specifies the URL or destination of the link
  - `target`: Specifies where to open the link (e.g., `_blank` opens in a new tab)
  - `rel`: Specifies the relationship between the current document and the linked document (e.g., `noopener` for security)
- **Usage**: `<a href="https://upsa.edu.gh" target="_blank" rel="noopener">official UPSA website</a>`

## HTML Entities

HTML entities are used to display special characters that have special meaning in HTML or are not easily typed:

### `&ndash;` or `&mdash;`
- **Purpose**: Displays an en dash (–) or em dash (—)
- **Description**: Used for punctuation in text
- **Usage**: `Web Development I &mdash; Team Horizon`

### `&amp;`
- **Purpose**: Displays an ampersand (&)
- **Description**: Used because `&` has special meaning in HTML
- **Usage**: `Course &amp; Group Introduction`

### `&copy;`
- **Purpose**: Displays a copyright symbol (©)
- **Description**: Used for copyright notices
- **Usage**: `&copy; 2025 Team Horizon`

## Tag Categories Summary

### Basic Tags (Fundamental Structure)
- `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`
- `<title>`, `<meta>`
- `<header>`, `<main>`, `<footer>`

### Text Tags (Content)
- `<h1>`, `<h2>` (headings)
- `<p>` (paragraphs)
- `<strong>` (emphasis)

### List Tags (Organization)
- `<ul>`, `<ol>`, `<li>`

### Advanced Tags (Multimedia & Semantics)
- `<section>`, `<figure>`, `<figcaption>`
- `<img>`, `<video>`, `<audio>`
- `<source>`, `<a>`
- `<div>`

## Best Practices

1. **Semantic HTML**: Use semantic tags like `<header>`, `<main>`, `<section>`, and `<footer>` to provide meaning to your content.

2. **Accessibility**: Always include `alt` attributes for images and proper heading hierarchy.

3. **Document Structure**: Maintain a clear hierarchy with proper nesting of elements.

4. **Self-Closing Tags**: Tags like `<img>`, `<source>`, and `<meta>` are self-closing and don't require a closing tag.

5. **Attributes**: Use `id` for unique identifiers and `class` for grouping elements that share characteristics.

6. **Links**: Use `target="_blank"` with `rel="noopener"` for external links to open in new tabs securely.

