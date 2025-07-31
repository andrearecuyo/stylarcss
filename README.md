# Stylar CSS Utility Library
![Stylar CSS Banner](https://raw.githubusercontent.com/andrearecuyo/stylarcss/refs/heads/main/stylarcss.png)

This is my own version of CSS Utility Library which is a collection of utility classes designed to simplify styling in web development projects. It provides a set of convenient classes for common styles and functionalities, saving you time and effort in the styling process.

## Table of Contents

1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Utilities](#utilities)
   - [Accessibility](#accessibility)
   - [Backgrounds](#backgrounds)
   - [Borders](#borders)
   - [Effects](#effects)
   - [Filters](#filters)
   - [Flex](#flex)
   - [Interactivity](#interactivity)
   - [Layout](#layout)
   - [Sizing](#sizing)
   - [Spacing](#spacing)
   - [SVG](#svg)
   - [Tables](#tables)
   - [Transition and Animation](#transition-animation)
   - [Transforms](#transforms)
   - [Typography](#typography)
5. [Contributing](#contributing)
6. [License](#license)

## Introduction 

Welcome to the CSS Utility Library, a comprehensive set of utility classes designed to streamline and enhance your web development projects. This library aims to provide a simple and flexible way to apply common styles and functionalities to your HTML elements.

### Key Features:
##### **Modular Structure**: The utility classes are organized into various categories, making it easy to find and apply the styles you need.
##### **Browser Compatibility**: The library ensures compatibility with all modern browsers, ensuring a consistent experience across different platforms.
##### **How to Use This Documentation**: Navigate through the different categories and find the utility classes that suit your requirements. Each utility class comes with a description, classes, usage guidelines, browser support information, and example usage. Simply copy and paste the provided code snippets into your project.

## Installation

Include the stylesheet in the head of your HTML file:

```html
<link rel="stylesheet" href="stylarcss/stylar-css-utility.css">
```
Import the stylesheet:
```html
import "stylarcss/stylar-css-utility.css";
```

## Usage

Using the CSS Utility Library is straightforward. Follow these steps to apply the provided utility classes to your HTML elements and achieve the desired styles.

### Applying Utility Classes

#### Class Structure

Utility classes in this library follow a structured naming convention, making it easy to understand their purpose. For example, the class for setting the aspect ratio is `aspect-ratio-{value}`.

#### Applying Classes

Add the desired utility class directly to your HTML elements using the `class` attribute.

```html
<!-- Example: Applying margin of 10px to div  -->
<div class="m-10">Sample Text</div>
```

#### Combining Classes
You can combine multiple utility classes on a single element to apply different styles.

```html
<!-- Example: Applying margin and padding -->
<div class="m-8 p-16">Combined Classes</div>
```

### Custom Styling
Feel free to customize styles further by combining utility classes with your custom CSS.
```html
<!-- Example: Custom styling with utility classes -->
<div class="m-8 p-16 custom-style">Custom Style</div>
```
### Important Notes
#### Order of Classes: The order of utility classes matters. Styles are applied in the order they appear in the class attribute.
```html
<div class="text-color-red background-color-blue">Incorrect Order</div>
```
#### Global Reset: Ensure there's no global CSS that might interfere with the utility classes. The library assumes a clean slate for styling.
```html
<!-- Example: Resetting styles -->
<link rel="stylesheet" href="reset.css">
<link rel="stylesheet" href="stylarcss/stylar-css-utility.css">
```

## Utilities 
- CSS Utility
- Description
- Classes
- Usage
- Browser Support
- Example Usage





## Layout
### Aspect Ratio

Description: Sets the aspect ratio of an element.

<details>
<summary>Classes:</summary>
<br />

.aspect-auto
.aspect-square
.aspect-video
.aspect-4x3
.aspect-3x2
.aspect-8x5
.aspect-md-auto
.aspect-lg-square
.aspect-xl-video
.aspect-padding-2x1
.aspect-padding-3x2
.aspect-padding-9x16
.aspect-img-3x4
.aspect-img-5x7
.aspect-img-1x2
</details>

<br />
Usage: Add the class aspect-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="aspect-square"></div>
```
### Container

Description: Sets a maximum-width container to center the content.

<details>
<summary>Classes:</summary>
<br />

.container
width: 100%

@media (min-width: 640px)
.sm-container
max-width: 640px

@media (min-width: 768px)
.md-container
max-width: 768px

@media (min-width: 1024px)
.lg-container
max-width: 1024px

@media (min-width: 1280px)
.xl-container
max-width: 1280px

@media (min-width: 1440px)
.xxl-container
max-width: 1440px

@media (min-width: 1600px)
.xxxl-container
max-width: 1600px

</details>

<br />
Usage: Add the class container to the container element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="container">  </div>
```
### Columns

Description: Sets the number of columns an element should span.

<details>
<summary>Classes:</summary>
<br />

.col-1 to .col-144
Set the number of columns from 1 to 144.

.col-auto-2xs
columns: auto 18rem; /* 288px */

.col-auto-xs
columns: auto 20rem; /* 320px */

.col-auto-sm
columns: auto 24rem; /* 384px */

.col-auto-md
columns: auto 28rem; /* 448px */

.col-auto-lg
columns: auto 32rem; /* 512px */

.col-auto
columns: auto

.col-3xs
columns: 16rem; /* 256px */

.col-2xs
columns: 18rem; /* 288px */

.col-xs
columns: 20rem; /* 320px */

.col-sm
columns: 24rem; /* 384px */

.col-md
columns: 28rem; /* 448px */

.col-lg
columns: 32rem; /* 512px */

.col-xl
columns: 36rem; /* 576px */

.col-2xl
columns: 42rem; /* 672px */

.col-3xl
columns: 48rem; /* 768px */

.col-4xl
columns: 56rem; /* 896px */

.col-5xl
columns: 64rem; /* 1024px */

.col-6xl
columns: 72rem; /* 1152px */

.col-7xl
columns: 80rem; /* 1280px */
</details>

<br />
Usage: Add the class col-{num} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="col-2"></div>
```
### Breaks
#### Break After

Description: Sets the type of break that should occur after an element.

<details>
<summary>Classes:</summary>
<br />

.break-after-auto: break-after: auto;
.break-after-avoid: break-after: avoid;
.break-after-all: break-after: all;
.break-after-avoid-page: break-after: avoid-page;
.break-after-page: break-after: page;
.break-after-left: break-after: left;
.break-after-right: break-after: right;
.break-after-column: break-after: column;
</details>

<br />
Usage: Add the class break-after-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<p class="break-after-avoid"></p>
```
#### Break Before

Description: Sets the type of break that should occur before an element.

<details>
<summary>Classes:</summary>
<br />

.break-before-auto: break-before: auto;
.break-before-avoid: break-before: avoid;
.break-before-all: break-before: all;
.break-before-avoid-page: break-before: avoid-page;
.break-before-page: break-before: page;
.break-before-left: break-before: left;
.break-before-right: break-before: right;
.break-before-column: break-before: column;
</details>

<br />
Usage: Add the class break-before-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<p class="break-before-always"></p>
```
#### Break Inside

Description: Sets the type of break that should occur inside an element.

<details>
<summary>Classes:</summary>
<br />

.break-inside-auto: break-inside: auto;
.break-inside-avoid: break-inside: avoid;
.break-inside-avoid-page: break-inside: avoid-page;
.break-inside-avoid-column: break-inside: avoid-column;

</details>

<br />
Usage: Add the class break-inside-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="break-inside-avoid"></div>
```
### Box Decoration Break

Description: Sets the behavior of box decoration break.

<details>
<summary>Classes:</summary>
<br />

.box-decoration-clone: box-decoration-break: clone;
.box-decoration-slice: box-decoration-break: slice;

</details>

<br />
Usage: Add the class box-decoration-break-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<p class="box-decoration-break-clone"></p>
```
### Box Sizing

Description: Sets the box sizing property.
<details>
<summary>Classes:</summary>
<br />

.box-border: box-sizing: border-box;
.box-content: box-sizing: content-box;
</details>

<br />
Usage: Add the class box-sizing-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="box-border"></div>
```
### Display

Description: Sets the display property.
<details>
<summary>Classes:</summary>
<br />

.block: display: block;
.inline-block: display: inline-block;
.inline: display: inline;
.flex: display: flex;
.inline-flex: display: inline-flex;
.table: display: table;
.inline-table: display: inline-table;
.table-caption: display: table-caption;
.table-cell: display: table-cell;
.table-column: display: table-column;
.table-column-group: display: table-column-group;
.table-footer-group: display: table-footer-group;
.table-header-group: display: table-header-group;
.table-row-group: display: table-row-group;
.table-row: display: table-row;
.flow-root: display: flow-root;
.grid: display: grid;
.inline-grid: display: inline-grid;
.contents: display: contents;
.list-item: display: list-item;
.hidden: display: none;
</details>

<br />
Usage: Add the class inline, etc. to the element.

Browser Support: All modern browsers.

Example Usage:
```jsx
<span class="inline-block"></span>
```
### Floats

Description: Sets the float property.
<details>
<summary>Classes:</summary>
<br />

.float-right: float: right;
.float-left: float: left;
.float-none: float: none;
.float-clear: clear: both;
.float-inline: float: inline;
.float-inline-start: float: inline-start;
.float-inline-end: float: inline-end;
.float-start: float: start;
.float-end: float: end;
.float-center: float: center;
</details>

<br />
Usage: Add the class float-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<img class="float-left" src="image.jpg" alt="An image">
```
### Clear

Description: Sets the clear property.
<details>
<summary>Classes:</summary>
<br />

.clear-left: clear: left;
.clear-right: clear: right;
.clear-both: clear: both;
.clear-none: clear: none;
</details>

<br />
Usage: Add the class clear-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="clear-both"></div>
```
### Isolation

Description: Sets the isolation property.
<details>
<summary>Classes:</summary>
<br />

.isolate: isolation: isolate;
.isolation-auto: isolation: auto;
</details>

<br />
Usage: Add the class isolation-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<iframe class="isolate" src="yourpage.html"></iframe>
```
### Object Fit

Description: Sets the object-fit property.
<details>
<summary>Classes:</summary>
<br />

.object-contain: object-fit: contain;
.object-cover: object-fit: cover;
.object-fill: object-fit: fill;
.object-none: object-fit: none;
.object-scale-down: object-fit: scale-down;

</details>

<br />
Usage: Add the class object-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<img class="object-cover" src="yourimage.jpg" alt="An image">
```
### Object Position

Description: Sets the object-position property.
<details>
<summary>Classes:</summary>
<br />

.object-bottom: object-position: bottom;
.object-center: object-position: center;
.object-left: object-position: left;
.object-left-bottom: object-position: left bottom;
.object-left-top: object-position: left top;
.object-right: object-position: right;
.object-right-bottom: object-position: right bottom;
.object-right-top: object-position: right top;
.object-top: object-position: top;

</details>

<br />
Usage: Add the class object-{value} to the element.

Browser Support: All modern browsers.

Example Usage:
`
```jsx
<img class="object-center" src="yourimage.jpg" alt="An image">
```
### Overflow

Description: Sets the overflow property.
<details>
<summary>Classes:</summary>
<br />

Overflow
.overflow-auto: overflow: auto;
.overflow-hidden: overflow: hidden;
.overflow-clip: overflow: clip;
.overflow-visible: overflow: visible;
.overflow-scroll: overflow: scroll;

Overflow X and Y

.overflow-x-auto: overflow-x: auto;
.overflow-y-auto: overflow-y: auto;
.overflow-x-hidden: overflow-x: hidden;
.overflow-y-hidden: overflow-y: hidden;
.overflow-x-clip: overflow-x: clip;
.overflow-y-clip: overflow-y: clip;
.overflow-x-visible: overflow-x: visible;
.overflow-y-visible: overflow-y: visible;
.overflow-x-scroll: overflow-x: scroll;
.overflow-y-scroll: overflow-y: scroll;
</details>

<br />
Usage: Add the class overflow-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="overflow-hidden"></div>
```
### Overscroll Behavior

Description: Sets the overscroll behavior property.
<details>
<summary>Classes:</summary>
<br />

Overscroll Behavior
.overscroll-auto: overscroll-behavior: auto;
.overscroll-contain: overscroll-behavior: contain;
.overscroll-none: overscroll-behavior: none;

Overscroll Behavior Y
.overscroll-y-auto: overscroll-behavior-y: auto;
.overscroll-y-contain: overscroll-behavior-y: contain;
.overscroll-y-none: overscroll-behavior-y: none;

Overscroll Behavior X
.overscroll-x-auto: overscroll-behavior-x: auto;
.overscroll-x-contain: overscroll-behavior-x: contain;
.overscroll-x-none: overscroll-behavior-x: none;
</details>

<br />
Usage: Add the class overscroll-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="overscroll-contain"></div>
```
### Position

Description: Sets the position property.
<details>
<summary>Classes:</summary>
<br />

.position-static: position: static;
.position-fixed: position: fixed;
.position-absolute: position: absolute;
.position-relative: position: relative;
.position-sticky: position: sticky;
</details>

<br />
Usage: Add the class position-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="position-relative"></div>
```
### Top / Right / Bottom / Left / Position Inset

Description: Sets the top, right, bottom, or left property.
<details>
<summary>Classes:</summary>
<br />

Inset Utilities:
.inset-0 to .inset-10: Sets inset values in different increments, from 0 to 2.5rem.
.inset-x-0 to .inset-x-10: Sets left and right values in different increments.
.inset-y-0 to .inset-y-10: Sets top and bottom values in different increments.
.start-0 to .start-10: Sets inset-inline-start values in different increments.
.end-0 to .end-10: Sets inset-inline-end values in different increments.
.top-0 to .top-10: Sets top values in different increments.
.right-0 to .right-10: Sets right values in different increments.
.bottom-0 to .bottom-10: Sets bottom values in different increments.
.left-0 to .left-10: Sets left values in different increments.
</details>

<br />
Usage: Add the class top-{value}, right-{value}, bottom-{value}, or left-{value} to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="top-0 right-0"></div>
```
### Visibility

Description: Sets visibility to visible, hidden, or collapse.
<details>
<summary>Classes:</summary>
<br />

.visible: visibility: visible;
Sets the element to be visible.

.invisible: visibility: hidden;
Hides the element, but the space it occupies is still reserved in the layout.

.collapse: visibility: collapse;
Typically used with table rows (tr), it hides the row and the space it occupies, similar to display: none for non-table elements.

</details>

<br />
Usage: Add the class visible, invisible, or collapse to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="invisible"></div>
```
### Z-Index

Description: Sets the z-index property.
<details>
<summary>Classes:</summary>
<br />

.z-0: z-index: 0;
.z-10: z-index: 10;
.z-20: z-index: 20;
.z-30: z-index: 30;
.z-40: z-index: 40;
.z-50: z-index: 50;
.z-auto: z-index: auto;
</details>

<br />
Usage: Add the class z-{value} or z-auto to the element.

Browser Support: All modern browsers.

Example Usage:

```jsx
<div class="z-10"></div>
```
## Accessibility
### Screen Readers

Description: Screen readers are assistive technologies for users with visual impairments.

<details>
<summary>Classes:</summary>
<br />

Screen Reader Text Utilities:
.sr-only-text
Visually hide text but make it accessible to screen readers.

.not-sr-only-text
Display text both visually and to screen readers.

Screen Reader Focus Utilities:
.focus-sr-only
Hide visually but make focusable and readable by screen readers.

.not-sr-only-focus
Keep default focus styling for keyboard navigation without visual display.

.not-sr-only-focus-colored
Same as .not-sr-only-focus with a custom colored focus outline.

.not-sr-only-focus-large
Same as .not-sr-only-focus with a larger focus outline.

Screen Reader Only Visually on Focus:
.focus-sr-only-visible
Make visible when focused but hidden otherwise for screen readers.

.focus-sr-only-hidden
Hide visually but make focusable and readable by screen readers.

.hidden-but-readable
Hide visually but make readable by screen readers.

.hidden-and-not-readable
Hide visually and make not readable by screen readers.

Indicating Focus for Keyboard Users:
.focus-indicator
Add a focus outline for keyboard users.

Visually Hidden, but Show on Hover or Focus:
.visible-on-hover-focus:hover, .visible-on-hover-focus:focus
Make visible on hover or focus but hidden otherwise.

Link Indicator for Screen Reader Users:
.link-sr-indicator
Indicate that an element is a link for screen reader users.

.link-sr-indicator::before
Add a visually hidden text ("Link: ") to indicate a link for screen readers.

Screen Reader Only - Announce to Screen Readers:
.sr-only-announce
Announce content to screen readers without displaying it visually.

Screen Reader Visible - Hide Visually but Announce to Screen Readers:
.sr-visible
Make visible to screen readers but hide visually.

Indicate Required Fields for Screen Readers:
.required-field::before
Add a visually hidden "(Required) " text before indicating a required field.

Indicate Error Messages for Screen Readers:
.error-message::before
Add a visually hidden "(Error) " text before indicating an error message.

Accessible Visually Hidden Heading:
.visually-hidden-heading
Visually hide a heading but make it accessible to screen readers.

Visually hide content and announce to screen readers:
.visually-hidden-announce
Visually hide content but announce to screen readers.

Screen Reader Read More Link:
.read-more-link
Add a "(Read more)" text after a link for screen reader users.

Screen Reader Skip to Content Link:
.skip-to-content
Provide a link to skip to the main content for screen readers.
</details>

<br />
Usage: Apply the class sr-only-text to the element containing text that you want to visually hide while remaining accessible to screen readers.

Browser Support: All modern browsers.
Example Usage:
```jsx
<button class="sr-only-text">Click me</button>
```
## Backgrounds
### Background Attachment
Description: Sets whether the background image is fixed or scrolls with the rest of the page.
<details>
<summary>Classes:</summary>
<br />

.bg-fixed: background-attachment: fixed;
.bg-local: background-attachment: local;
.bg-scroll: background-attachment: scroll;
</details>

<br />
Usage: Apply bg-{value} to control the background attachment property.

Browser Support: All modern browsers.

Example Usage:
```jsx
<div class="bg-fixed"></div>
```
### Background Clip
Description: Specifies how far the background color or image should extend within an element.
<details>
<summary>Classes:</summary>
<br />

.bg-clip-border: background-clip: border-box;
.bg-clip-padding: background-clip: padding-box;
.bg-clip-content: background-clip: content-box;
.bg-clip-text: background-clip: text;
</details>

<br />
Usage: Apply bg-{value} to control the background clip property.

Browser Support: All modern browsers.

Example Usage:
```jsx
<div class="bg-clip-border"></div>
```
### Background Color
Description: Sets the background color of an element.

Usage: Apply bg-{value} to control the background color property.
<details>
<summary>Classes:</summary>
<br />

.bg-inherit: background-color: inherit;
.bg-current: background-color: currentColor;
.bg-transparent: background-color: transparent;
.bg-black: background-color: rgb(0 0 0);
.bg-gray: background-color: gray;
.bg-white: background-color: rgb(255 255 255);

</details>

<br />
Browser Support: All modern browsers.

Example Usage:
```jsx
<div class="bg-inherit"></div>
```
### Background Image
Description: Sets one or more background images for an element.
<details>
<summary>Classes:</summary>
<br />


.bg-none: background-image: none;
.bg-gradient-to-t: background-image: linear-gradient(to top, var(--gradient-stops));
.bg-gradient-to-tr: background-image: linear-gradient(to top right, var(--gradient-stops));
.bg-gradient-to-r: background-image: linear-gradient(to right, var(--gradient-stops));
.bg-gradient-to-br: background-image: linear-gradient(to bottom right, var(--gradient-stops));
.bg-gradient-to-b: background-image: linear-gradient(to bottom, var(--gradient-stops));
.bg-gradient-to-bl: background-image: linear-gradient(to bottom left, var(--gradient-stops));
.bg-gradient-to-l: background-image: linear-gradient(to left, var(--gradient-stops));
.bg-gradient-to-tl: background-image: linear-gradient(to top left, var(--gradient-stops));
</details>

<br />
Usage: Apply bg-{value} to control the background image property.

Browser Support: All modern browsers.

Example Usage:
```jsx
<div class="bg-none"></div>
```
### Background Origin
Description: Specifies where the background image or color is positioned.
<details>
<summary>Classes:</summary>
<br />

.bg-origin-border: background-origin: border-box;
.bg-origin-padding: background-origin: padding-box;
.bg-origin-content: background-origin: content-box;
</details>

<br />
Usage: Apply bg-{value} to control the background origin property.

Browser Support: All modern browsers.

Example Usage:
```jsx
<div class="bg-origin-border"></div>
```
### Background Position
Description: Sets the initial position of the background image.
<details>
<summary>Classes:</summary>
<br />

.bg-bottom: background-position: bottom;
.bg-center: background-position: center;
.bg-left: background-position: left;
.bg-left-bottom: background-position: left bottom;
.bg-left-top: background-position: left top;
.bg-right: background-position: right;
.bg-right-bottom: background-position: right bottom;
.bg-right-top: background-position: right top;
.bg-top: background-position: top;
</details>

<br />
Usage: Apply bg-{value} to control the background position property.

Browser Support: All modern browsers.

Example Usage:
```jsx
<div class="bg-bottom"></div>
```
### Background Repeat
Description: Sets how a background image is repeated.
<details>
<summary>Classes:</summary>
<br />

.bg-repeat: background-repeat: repeat;
.bg-no-repeat: background-repeat: no-repeat;
.bg-repeat-x: background-repeat: repeat-x;
.bg-repeat-y: background-repeat: repeat-y;
.bg-repeat-round: background-repeat: round;
.bg-repeat-space: background-repeat: space;
</details>

<br />
Usage: Apply bg-{value} to control the background repeat property.

Browser Support: All modern browsers.

Example Usage:
```jsx
<div class="bg-repeat"></div>
```
### Background Size
Description: Specifies the size of the background image.
<details>
<summary>Classes:</summary>
<br />

.bg-auto: background-size: auto;
.bg-cover: background-size: cover;
.bg-contain: background-size: contain;
</details>

<br />
Usage: Apply bg-{value} to control the background size property.

Browser Support: All modern browsers.

Example Usage:
```jsx
<div class="bg-auto"></div>
```
## Borders
### Border
Description: Sets the border properties of an element.
<details>
<summary>Classes:</summary>
<br />

Border Radius
.rounded-none: border-radius: 0px;
.rounded-sm: border-radius: 0.125rem; /* 2px */
.rounded: border-radius: 0.25rem; /* 4px */
.rounded-md: border-radius: 0.375rem; /* 6px */
.rounded-lg: border-radius: 0.5rem; /* 8px */
.rounded-xl: border-radius: 0.75rem; /* 12px */
.rounded-2xl: border-radius: 1rem; /* 16px */
.rounded-3xl: border-radius: 1.5rem; /* 24px */
.rounded-full: border-radius: 9999px;

Border Radius - Specific Corners
Top-Left
.rounded-tl-none: border-top-left-radius: 0px;
.rounded-tl-sm: border-top-left-radius: 0.125rem; /* 2px */
.rounded-tl: border-top-left-radius: 0.25rem; /* 4px */
.rounded-tl-md: border-top-left-radius: 0.375rem; /* 6px */
.rounded-tl-lg: border-top-left-radius: 0.5rem; /* 8px */
.rounded-tl-xl: border-top-left-radius: 0.75rem; /* 12px */
.rounded-tl-2xl: border-top-left-radius: 1rem; /* 16px */
.rounded-tl-3xl: border-top-left-radius: 1.5rem; /* 24px */
.rounded-tl-full: border-top-left-radius: 9999px;

Top-Right
.rounded-tr-none: border-top-right-radius: 0px;
.rounded-tr-sm: border-top-right-radius: 0.125rem; /* 2px */
.rounded-tr: border-top-right-radius: 0.25rem; /* 4px */
.rounded-tr-md: border-top-right-radius: 0.375rem; /* 6px */
.rounded-tr-lg: border-top-right-radius: 0.5rem; /* 8px */
.rounded-tr-xl: border-top-right-radius: 0.75rem; /* 12px */
.rounded-tr-2xl: border-top-right-radius: 1rem; /* 16px */
.rounded-tr-3xl: border-top-right-radius: 1.5rem; /* 24px */
.rounded-tr-full: border-top-right-radius: 9999px;

Bottom-Right
.rounded-br-none: border-bottom-right-radius: 0px;
.rounded-br-sm: border-bottom-right-radius: 0.125rem; /* 2px */
.rounded-br: border-bottom-right-radius: 0.25rem; /* 4px */
.rounded-br-md: border-bottom-right-radius: 0.375rem; /* 6px */
.rounded-br-lg: border-bottom-right-radius: 0.5rem; /* 8px */
.rounded-br-xl: border-bottom-right-radius: 0.75rem; /* 12px */
.rounded-br-2xl: border-bottom-right-radius: 1rem; /* 16px */
.rounded-br-3xl: border-bottom-right-radius: 1.5rem; /* 24px */
.rounded-br-full: border-bottom-right-radius: 9999px;

Bottom-Left
.rounded-bl-none: border-bottom-left-radius: 0px;
.rounded-bl-sm: border-bottom-left-radius: 0.125rem; /* 2px */
.rounded-bl: border-bottom-left-radius: 0.25rem; /* 4px */
.rounded-bl-md: border-bottom-left-radius: 0.375rem; /* 6px */
.rounded-bl-lg: border-bottom-left-radius: 0.5rem; /* 8px */
.rounded-bl-xl: border-bottom-left-radius: 0.75rem; /* 12px */
.rounded-bl-2xl: border-bottom-left-radius: 1rem; /* 16px */
.rounded-bl-3xl: border-bottom-left-radius: 1.5rem; /* 24px */
.rounded-bl-full: border-bottom-left-radius: 9999px;

Specific Sides 
Start-Start
.rounded-ss-none: border-start-start-radius: 0px;
.rounded-ss-sm: border-start-start-radius: 0.125rem; /* 2px */
.rounded-ss: border-start-start-radius: 0.25rem; /* 4px */
.rounded-ss-md: border-start-start-radius: 0.375rem; /* 6px */
.rounded-ss-lg: border-start-start-radius: 0.5rem; /* 8px */
.rounded-ss-xl: border-start-start-radius: 0.75rem; /* 12px */
.rounded-ss-2xl: border-start-start-radius: 1rem; /* 16px */
.rounded-ss-3xl: border-start-start-radius: 1.5rem; /* 24px */
.rounded-ss-full: border-start-start-radius: 9999px;

Start-End
.rounded-se-none: border-start-end-radius: 0px;
.rounded-se-sm: border-start-end-radius: 0.125rem; /* 2px */
.rounded-se: border-start-end-radius: 0.25rem; /* 4px */
.rounded-se-md: border-start-end-radius: 0.375rem; /* 6px */
.rounded-se-lg: border-start-end-radius: 0.5rem; /* 8px */
.rounded-se-xl: border-start-end-radius: 0.75rem; /* 12px */
.rounded-se-2xl: border-start-end-radius: 1rem; /* 16px */
.rounded-se-3xl: border-start-end-radius: 1.5rem; /* 24px */
.rounded-se-full: border-start-end-radius: 9999px;

End-End
.rounded-ee-none: border-end-end-radius: 0px;
.rounded-ee-sm: border-end-end-radius: 0.125rem; /* 2px */
.rounded-ee: border-end-end-radius: 0.25rem; /* 4px */
.rounded-ee-md: border-end-end-radius: 0.375rem; /* 6px */
.rounded-ee-lg: border-end-end-radius: 0.5rem; /* 8px */
.rounded-ee-xl: border-end-end-radius: 0.75rem; /* 12px */
.rounded-ee-2xl: border-end-end-radius: 1rem; /* 16px */
.rounded-ee-3xl: border-end-end-radius: 1.5rem; /* 24px */
.rounded-ee-full: border-end-end-radius: 9999px;

End-Start
.rounded-es-none: border-end-start-radius: 0px;
.rounded-es-sm: border-end-start-radius: 0.125rem; /* 2px */
.rounded-es: border-end-start-radius: 0.25rem; /* 4px */
.rounded-es-md: border-end-start-radius: 0.375rem; /* 6px */
.rounded-es-lg: border-end-start-radius: 0.5rem; /* 8px */
.rounded-es-xl: border-end-start-radius: 0.75rem; /* 12px */
.rounded-es-2xl: border-end-start-radius: 1rem; /* 16px */
.rounded-es-3xl: border-end-start-radius: 1.5rem; /* 24px */
.rounded-es-full: border-end-start-radius: 9999px;

Border Width

.border-0: border-width: 0px;
.border-2: border-width: 2px;
.border-4: border-width: 4px;
.border-8: border-width: 8px;
.border: border-width: 1px;
.border-x-0: border-left-width: 0px; border-right-width: 0px;
.border-x-2: border-left-width: 2px; border-right-width: 2px;
.border-x-4: border-left-width: 4px; border-right-width: 4px;
.border-x-8: border-left-width: 8px; border-right-width: 8px;
.border-x: border-left-width: 1px; border-right-width: 1px;
.border-y-0: border-top-width: 0px; border-bottom-width: 0px;
.border-y-2: border-top-width: 2px; border-bottom-width: 2px;
.border-y-4: border-top-width: 4px; border-bottom-width: 4px;
.border-y-8: border-top-width: 8px; border-bottom-width: 8px;
.border-y: border-top-width: 1px; border-bottom-width: 1px;
.border-s-0: border-inline-start-width: 0px;
.border-s-2: border-inline-start-width: 2px;
.border-s-4: border-inline-start-width: 4px;
.border-s-8: border-inline-start-width: 8px;
.border-s: border-inline-start-width: 1px;
.border-e-0: border-inline-end-width: 0px;
.border-e-2: border-inline-end-width: 2px;
.border-e-4: border-inline-end-width: 4px;
.border-e-8: border-inline-end-width: 8px;
.border-e: border-inline-end-width: 1px;
.border-t-0: border-top-width: 0px;
.border-t-2: border-top-width: 2px;
.border-t-4: border-top-width: 4px;
.border-t-8: border-top-width: 8px;
.border-t: border-top-width: 1px;
.border-r-0: border-right-width: 0px;
.border-r-2: border-right-width: 2px;
.border-r-4: border-right-width: 4px;
.border-r-8: border-right-width: 8px;
.border-r: border-right-width: 1px;
.border-b-0: border-bottom-width: 0px;
.border-b-2: border-bottom-width: 2px;
.border-b-4: border-bottom-width: 4px;
.border-b-8: border-bottom-width: 8px;
.border-b: border-bottom-width: 1px;
.border-l-0: border-left-width: 0px;
.border-l-2: border-left-width: 2px;
.border-l-4: border-left-width: 4px;
.border-l-8: border-left-width: 8px;
.border-l: border-left-width: 1px;

Border Color
.border-inherit: border-color: inherit;
.border-current: border-color: currentColor;
.border-transparent: border-color: transparent;
.border-black: border-color: rgb(0 0 0);
.border-white: border-color: rgb(255 255 255);

Border Style

.border-solid: border-style: solid;
.border-dashed: border-style: dashed;
.border-dotted: border-style: dotted;
.border-double: border-style: double;
.border-hidden: border-style: hidden;
.border-none: border-style: none;

</details>

<br />
Usage: Apply border-{value} to control the border properties.

Example Usage:

```jsx
<div class="border-none"></div>
```
### Divide
Description: Adds dividers between child elements.
<details>
<summary>Classes:</summary>
<br />

Divide Width
Horizontal Dividers
.divide-x-0 > * + *: border-right-width: 0px; border-left-width: 0px;
.divide-x-2 > * + *: border-right-width: 0px; border-left-width: 2px;
.divide-x-4 > * + *: border-right-width: 0px; border-left-width: 4px;
.divide-x-8 > * + *: border-right-width: 0px; border-left-width: 8px;
.divide-x > * + *: border-right-width: 0px; border-left-width: 1px;

Vertical Dividers
.divide-y-0 > * + *: border-top-width: 0px; border-bottom-width: 0px;
.divide-y-2 > * + *: border-top-width: 2px; border-bottom-width: 0px;
.divide-y-4 > * + *: border-top-width: 4px; border-bottom-width: 0px;
.divide-y-8 > * + *: border-top-width: 8px; border-bottom-width: 0px;
.divide-y > * + *: border-top-width: 1px; border-bottom-width: 0px;

Reverse Dividers

Divide Color
Inherit
.divide-inherit > * + *: border-color: inherit;
Current Color
.divide-current > * + *: border-color: currentColor;
Transparent
.divide-transparent > * + *: border-color: transparent;
Black
.divide-black > * + *: border-color: rgb(0 0 0);
White
.divide-white > * + *: border-color: rgb(255 255 255);

Divide Style
Solid
.divide-solid > * + *: border-style: solid;
Dashed
.divide-dashed > * + *: border-style: dashed;
Dotted
.divide-dotted > * + *: border-style: dotted;
Double
.divide-double > * + *: border-style: double;
None
.divide-none > * + *: border-style: none;

</details>

<br />
Usage: Apply divide-{value} to a container to create dividers between its child elements.

Example Usage:

```jsx
<ul class="divide-solid">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```
### Outline
Description: Sets the outline properties of an element.
<details>
<summary>Classes:</summary>
<br />

Outline Width
.outline-0: outline-width: 0px;
.outline-1: outline-width: 1px;
.outline-2: outline-width: 2px;
.outline-4: outline-width: 4px;
.outline-8: outline-width: 8px;

Outline Color
.outline-inherit: outline-color: inherit;
.outline-current: outline-color: currentColor;
.outline-transparent: outline-color: transparent;
.outline-black: outline-color: #000;
.outline-white: outline-color: #fff;

Outline Style
.outline-none: outline: 2px solid transparent; outline-offset: 2px;
.outline-solid: outline-style: solid;
.outline-dashed: outline-style: dashed;
.outline-dotted: outline-style: dotted;
.outline-double: outline-style: double;

Outline Offset
.outline-offset-0: outline-offset: 0px;
.outline-offset-1: outline-offset: 1px;
.outline-offset-2: outline-offset: 2px;
.outline-offset-4: outline-offset: 4px;
.outline-offset-8: outline-offset: 8px;

</details>

<br />
Usage: Apply outline-{value} to control the outline properties.

Example Usage:

```jsx
<button class="outline-0">
  Click me
</button>
```
### Ring
Description: Adds a focus ring around an element.
<details>
<summary>Classes:</summary>
<br />

Ring Width
.ring-0: box-shadow: var(--ring-inset) 0 0 0 calc(0px + var(--ring-offset-width)) var(--ring-color);
.ring-1: box-shadow: var(--ring-inset) 0 0 0 calc(1px + var(--ring-offset-width)) var(--ring-color);
.ring-2: box-shadow: var(--ring-inset) 0 0 0 calc(2px + var(--ring-offset-width)) var(--ring-color);
.ring: box-shadow: var(--ring-inset) 0 0 0 calc(3px + var(--ring-offset-width)) var(--ring-color);
.ring-4: box-shadow: var(--ring-inset) 0 0 0 calc(4px + var(--ring-offset-width)) var(--ring-color);
.ring-8: box-shadow: var(--ring-inset) 0 0 0 calc(8px + var(--ring-offset-width)) var(--ring-color);
.ring-inset: --ring-inset: inset;

Ring Color
.ring-inherit: --ring-color: inherit;
.ring-current: --ring-color: currentColor;
.ring-transparent: --ring-color: transparent;
.ring-black: --ring-color: rgb(0 0 0);
.ring-white: --ring-color: rgb(255 255 255);

Ring Offset Width
.ring-offset-0: --ring-offset-width: 0px; box-shadow: 0 0 0 var(--ring-offset-width) var(--ring-offset-color), var(--ring-shadow);
.ring-offset-1: --ring-offset-width: 1px; box-shadow: 0 0 0 var(--ring-offset-width) var(--ring-offset-color), var(--ring-shadow);
.ring-offset-2: --ring-offset-width: 2px; box-shadow: 0 0 0 var(--ring-offset-width) var(--ring-offset-color), var(--ring-shadow);
.ring-offset-4: --ring-offset-width: 4px; box-shadow: 0 0 0 var(--ring-offset-width) var(--ring-offset-color), var(--ring-shadow);
.ring-offset-8: --ring-offset-width: 8px; box-shadow: 0 0 0 var(--ring-offset-width) var(--ring-offset-color), var(--ring-shadow);

Ring Offset Color
.ring-offset-inherit: --ring-offset-color: inherit; box-shadow: 0 0 0 var(--ring-offset-width) var(--ring-offset-color), var(--ring-shadow);
.ring-offset-current: --ring-offset-color: currentColor; box-shadow: 0 0 0 var(--ring-offset-width) var(--ring-offset-color), var(--ring-shadow);
.ring-offset-transparent: --ring-offset-color: transparent; box-shadow: 0 0 0 var(--ring-offset-width) var(--ring-offset-color), var(--ring-shadow);
.ring-offset-black: --ring-offset-color: #000;

</details>

<br />
Usage: Apply ring-{value} to make a focus ring visible on the element when it receives focus.

Example Usage:

```jsx
<input type="text" class="ring-0" placeholder="Type here">
```
## Effects
### Background Blend Mode
Description: Specifies how the background image of an element should blend with its background color.
<details>
<summary>Classes:</summary>
<br />

.bg-blend-normal: background-blend-mode: normal;
.bg-blend-multiply: background-blend-mode: multiply;
.bg-blend-screen: background-blend-mode: screen;
.bg-blend-overlay: background-blend-mode: overlay;
.bg-blend-darken: background-blend-mode: darken;
.bg-blend-lighten: background-blend-mode: lighten;
.bg-blend-color-dodge: background-blend-mode: color-dodge;
.bg-blend-color-burn: background-blend-mode: color-burn;
.bg-blend-hard-light: background-blend-mode: hard-light;
.bg-blend-soft-light: background-blend-mode: soft-light;
.bg-blend-difference: background-blend-mode: difference;
.bg-blend-exclusion: background-blend-mode: exclusion;
.bg-blend-hue: background-blend-mode: hue;
.bg-blend-saturation: background-blend-mode: saturation;
.bg-blend-color: background-blend-mode: color;
.bg-blend-luminosity: background-blend-mode: luminosity;
</details>

<br />
Usage: Apply bg-blend-{value} to control the background blend mode property.

Example Usage:
```jsx
<div class="bg-blend-normal"></div>
```
### Box Shadow
Description: Adds a shadow effect to an element.
<details>
<summary>Classes:</summary>
<br />


Box Shadow
.shadow-sm: box-shadow: 0 1px 2px 0 rgb(0 0 0 / 0.05);
.shadow: box-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);
.shadow-md: box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
.shadow-lg: box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);
.shadow-xl: box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
.shadow-2xl: box-shadow: 0 25px 50px -12px rgb(0 0 0 / 0.25);
.shadow-inner: box-shadow: inset 0 2px 4px 0 rgb(0 0 0 / 0.05);
.shadow-none: box-shadow: 0 0 #0000;

Box Shadow Color
.shadow-inherit: --shadow-color: inherit;
.shadow-current: --shadow-color: currentColor;
.shadow-transparent: --shadow-color: transparent;
.shadow-black: --shadow-color: #000;
.shadow-white: --shadow-color: #fff;
</details>

<br />
Usage: Apply shadow-{value} to control the box shadow property.

Example Usage:
```jsx
<div class="shadow-sm"></div>
```
### Mixblend Mode
Description: Specifies how an element's content should blend with its background.
<details>
<summary>Classes:</summary>
<br />

Mix Blend Mode
.mix-blend-normal: mix-blend-mode: normal;
.mix-blend-multiply: mix-blend-mode: multiply;
.mix-blend-screen: mix-blend-mode: screen;
.mix-blend-overlay: mix-blend-mode: overlay;
.mix-blend-darken: mix-blend-mode: darken;
.mix-blend-lighten: mix-blend-mode: lighten;
.mix-blend-color-dodge: mix-blend-mode: color-dodge;
.mix-blend-color-burn: mix-blend-mode: color-burn;
.mix-blend-hard-light: mix-blend-mode: hard-light;
.mix-blend-soft-light: mix-blend-mode: soft-light;
.mix-blend-difference: mix-blend-mode: difference;
.mix-blend-exclusion: mix-blend-mode: exclusion;
.mix-blend-hue: mix-blend-mode: hue;
.mix-blend-saturation: mix-blend-mode: saturation;
.mix-blend-color: mix-blend-mode: color;
.mix-blend-luminosity: mix-blend-mode: luminosity;

</details>

<br />
Usage: Apply mix-blend-{value} to control the mix blend mode property.

Example Usage:
```jsx
<div class="mix-blend-normal"></div>
```
### Opacity
Description: Sets the transparency level of an element.
<details>
<summary>Classes:</summary>
<br />

.opacity-0: opacity: 0;
.opacity-5: opacity: 0.05;
.opacity-10: opacity: 0.1;
.opacity-20: opacity: 0.2;
.opacity-25: opacity: 0.25;
.opacity-30: opacity: 0.3;
.opacity-40: opacity: 0.4;
.opacity-50: opacity: 0.5;
.opacity-60: opacity: 0.6;
.opacity-70: opacity: 0.7;
.opacity-75: opacity: 0.75;
.opacity-80: opacity: 0.8;
.opacity-90: opacity: 0.9;
.opacity-95: opacity: 0.95;
.opacity-100: opacity: 1;
</details>

<br />
Usage: Apply opacity-{value} to control the opacity property.

Example Usage:
```jsx
<div class="opacity-5"></div>
```
## Filters
### Backdrop
Description: Applies a backdrop filter effect to an element's background.
<details>
<summary>Classes:</summary>
<br />

Backdrop Blur
.backdrop-blur-none: backdrop-filter: blur(0);

.backdrop-blur-sm: backdrop-filter: blur(4px);

.backdrop-blur: backdrop-filter: blur(8px);

.backdrop-blur-md: backdrop-filter: blur(12px);

.backdrop-blur-lg: backdrop-filter: blur(16px);

.backdrop-blur-xl: backdrop-filter: blur(24px);

.backdrop-blur-2xl: backdrop-filter: blur(40px);

.backdrop-blur-3xl: backdrop-filter: blur(64px);

Backdrop Brightness
.backdrop-brightness-0: backdrop-filter: brightness(0);

.backdrop-brightness-50: backdrop-filter: brightness(0.5);

.backdrop-brightness-75: backdrop-filter: brightness(0.75);

.backdrop-brightness-90: backdrop-filter: brightness(0.9);

.backdrop-brightness-95: backdrop-filter: brightness(0.95);

.backdrop-brightness-100: backdrop-filter: brightness(1);

.backdrop-brightness-105: backdrop-filter: brightness(1.05);

.backdrop-brightness-110: backdrop-filter: brightness(1.1);

.backdrop-brightness-125: backdrop-filter: brightness(1.25);

.backdrop-brightness-150: backdrop-filter: brightness(1.5);

.backdrop-brightness-200: backdrop-filter: brightness(2);

Backdrop Contrast
.backdrop-contrast-0: backdrop-filter: contrast(0);

.backdrop-contrast-50: backdrop-filter: contrast(0.5);

.backdrop-contrast-75: backdrop-filter: contrast(0.75);

.backdrop-contrast-100: backdrop-filter: contrast(1);

.backdrop-contrast-125: backdrop-filter: contrast(1.25);

.backdrop-contrast-150: backdrop-filter: contrast(1.5);

.backdrop-contrast-200: backdrop-filter: contrast(2);

Backdrop Grayscale
.backdrop-grayscale-0: backdrop-filter: grayscale(0);

.backdrop-grayscale: backdrop-filter: grayscale(100%);

Backdrop Hue Rotate
.backdrop-hue-rotate-0: backdrop-filter: hue-rotate(0deg);

.backdrop-hue-rotate-15: backdrop-filter: hue-rotate(15deg);

.backdrop-hue-rotate-30: backdrop-filter: hue-rotate(30deg);

.backdrop-hue-rotate-60: backdrop-filter: hue-rotate(60deg);

.backdrop-hue-rotate-90: backdrop-filter: hue-rotate(90deg);

.backdrop-hue-rotate-180: backdrop-filter: hue-rotate(180deg);

Backdrop Invert
.backdrop-invert-0: backdrop-filter: invert(0);

.backdrop-invert: backdrop-filter: invert(100%);

Backdrop Opacity
.backdrop-opacity-0: backdrop-filter: opacity(0);

.backdrop-opacity-5: backdrop-filter: opacity(0.05);

.backdrop-opacity-10: backdrop-filter: opacity(0.1);

.backdrop-opacity-20: backdrop-filter: opacity(0.2);

.backdrop-opacity-25: backdrop-filter: opacity(0.25);

.backdrop-opacity-30: backdrop-filter: opacity(0.3);

.backdrop-opacity-40: backdrop-filter: opacity(0.4);

.backdrop-opacity-50: backdrop-filter: opacity(0.5);

.backdrop-opacity-60: backdrop-filter: opacity(0.6);

.backdrop-opacity-70: backdrop-filter: opacity(0.7);

.backdrop-opacity-75: backdrop-filter: opacity(0.75);

.backdrop-opacity-80: backdrop-filter: opacity(0.8);

.backdrop-opacity-90: backdrop-filter: opacity(0.9);

.backdrop-opacity-95: backdrop-filter: opacity(0.95);

.backdrop-opacity-100: backdrop-filter: opacity(1);

Backdrop Saturate
.backdrop-saturate-0: backdrop-filter: saturate(0);

.backdrop-saturate-50: backdrop-filter: saturate(0.5);

.backdrop-saturate-100: backdrop-filter: saturate(1);

.backdrop-saturate-150: backdrop-filter: saturate(1.5);

.backdrop-saturate-200: backdrop-filter: saturate(2);

Backdrop Sepia
.backdrop-sepia-0: backdrop-filter: sepia(0);

.backdrop-sepia: backdrop-filter: sepia(100%);

</details>

<br />
Usage: Apply backdrop-blur-{value} to control the backdrop-filter property.

Example Usage:

```jsx
<div class="backdrop-blur-none"></div>
```
### Blur
Description: Applies a blur effect to an element.
<details>
<summary>Classes:</summary>
<br />

.blur-none: filter: blur(0);
.blur-sm: filter: blur(4px);
.blur: filter: blur(8px);
.blur-md: filter: blur(12px);
.blur-lg: filter: blur(16px);
.blur-xl: filter: blur(24px);
.blur-2xl: filter: blur(40px);
.blur-3xl: filter: blur(64px);

</details>

<br />
Usage: Apply blur-{value} to control the blur filter property.

Example Usage:

```jsx
<div class="blur-none"></div>
```
### Brightness
Description: Adjusts the brightness of an element.
<details>
<summary>Classes:</summary>
<br />

.brightness-0: filter: brightness(0);
.brightness-50: filter: brightness(0.5);
.brightness-75: filter: brightness(0.75);
.brightness-90: filter: brightness(0.9);
.brightness-95: filter: brightness(0.95);
.brightness-100: filter: brightness(1);
.brightness-105: filter: brightness(1.05);
.brightness-110: filter: brightness(1.1);
.brightness-125: filter: brightness(1.25);
.brightness-150: filter: brightness(1.5);
.brightness-200: filter: brightness(2);

</details>

<br />
Usage: Apply brightness-{value} to control the brightness filter property.

Example Usage:

```jsx
<div class="brightness-50"></div>
```
### Contrast
Description: Adjusts the contrast of an element.
<details>
<summary>Classes:</summary>
<br />

.contrast-0: filter: contrast(0);
.contrast-50: filter: contrast(0.5);
.contrast-75: filter: contrast(0.75);
.contrast-100: filter: contrast(1);
.contrast-125: filter: contrast(1.25);
.contrast-150: filter: contrast(1.5);
.contrast-200: filter: contrast(2);

</details>

<br />
Usage: Apply contrast-{value} to control the contrast filter property.

Example Usage:

```jsx
<div class="contrast-50"></div>
```
### Dropshadow
Description: Adds a drop shadow effect to an element.
<details>
<summary>Classes:</summary>
<br />

.drop-shadow-sm: filter: drop-shadow(0 1px 1px rgba(0, 0, 0, 0.05));
.drop-shadow: filter: drop-shadow(0 1px 2px rgba(0, 0, 0, 0.1)) drop-shadow(0 1px 1px rgba(0, 0, 0, 0.06));
.drop-shadow-md: filter: drop-shadow(0 4px 3px rgba(0, 0, 0, 0.07)) drop-shadow(0 2px 2px rgba(0, 0, 0, 0.06));
.drop-shadow-lg: filter: drop-shadow(0 10px 8px rgba(0, 0, 0, 0.04)) drop-shadow(0 4px 3px rgba(0, 0, 0, 0.1));
.drop-shadow-xl: filter: drop-shadow(0 20px 13px rgba(0, 0, 0, 0.03)) drop-shadow(0 8px 5px rgba(0, 0, 0, 0.08));
.drop-shadow-2xl: filter: drop-shadow(0 25px 25px rgba(0, 0, 0, 0.15));
.drop-shadow-none: filter: drop-shadow(0 0 rgba(0, 0, 0, 0));

</details>

<br />
Usage: Apply drop-shadow-{value} to control the drop-shadow filter property.

Example Usage:

```jsx
<div class="drop-shadow"></div>
```
### Grayscale
Description: Converts an element to grayscale.
<details>
<summary>Classes:</summary>
<br />

.grayscale-0: filter: grayscale(0);
.grayscale: filter: grayscale(100%);

</details>

<br />
Usage: Apply grayscale-{value} to control the grayscale filter property.

Example Usage:

```jsx
<div class="grayscale"></div>
```
### Huerotate
Description: Applies a hue rotation to an element.
<details>
<summary>Classes:</summary>
<br />

.hue-rotate-0: filter: hue-rotate(0deg);
.hue-rotate-15: filter: hue-rotate(15deg);
.hue-rotate-30: filter: hue-rotate(30deg);
.hue-rotate-60: filter: hue-rotate(60deg);
.hue-rotate-90: filter: hue-rotate(90deg);
.hue-rotate-180: filter: hue-rotate(180deg);
</details>

<br />
Usage: Apply hue-rotate-{value} to control the hue-rotate filter property.

Example Usage:

```jsx
<div class="hue-rotate-15"></div>
```
### Invert
Description: Inverts the colors of an element.
<details>
<summary>Classes:</summary>
<br />

.invert-0: filter: invert(0);
.invert: filter: invert(100%);

</details>

<br />
Usage: Apply invert-{value} to control the invert filter property.

Example Usage:

```jsx
<div class="invert"></div>
```
### Saturate
Description: Adjusts the saturation of an element.
<details>
<summary>Classes:</summary>
<br />

.saturate-0: filter: saturate(0);
.saturate-50: filter: saturate(0.5);
.saturate-100: filter: saturate(1);
.saturate-150: filter: saturate(1.5);
.saturate-200: filter: saturate(2);

</details>

<br />
Usage: Apply saturate-{value} to control the saturate filter property.

Example Usage:

```jsx
<div class="saturate-50"></div>
```
### Sepia
Description: Applies a sepia tone to an element.
<details>
<summary>Classes:</summary>
<br />

.sepia-0: filter: sepia(0);
.sepia: filter: sepia(100%);
</details>

<br />
Usage: Apply sepia-{value} to control the sepia filter property.

Example Usage:

```jsx
<div class="sepia"></div>
```
## Flex
### Align
Description: Sets the alignment of an element along the cross-axis in a flex container.
<details>
<summary>Classes:</summary>
<br />

.content-normal: align-content: normal;
.content-center: align-content: center;
.content-start: align-content: flex-start;
.content-end: align-content: flex-end;
.content-between: align-content: space-between;
.content-around: align-content: space-around;
.content-evenly: align-content: space-evenly;
.content-baseline: align-content: baseline;
.content-stretch: align-content: stretch;

.items-start: align-items: flex-start;
.items-end: align-items: flex-end;
.items-center: align-items: center;
.items-baseline: align-items: baseline;
.items-stretch: align-items: stretch;

.self-auto: align-self: auto;
.self-start: align-self: flex-start;
.self-end: align-self: flex-end;
.self-center: align-self: center;
.self-stretch: align-self: stretch;
.self-baseline: align-self: baseline;

</details>

<br />
Usage: Apply the class content-{value}, items-{value} and self-{value} to control the alignment.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="content-center"></div>
```
### Flex
Description: Sets the flexible properties of a flex container.
<details>
<summary>Classes:</summary>
<br />

.flex-1: flex: 1 1 0%;
.flex-auto: flex: 1 1 auto;
.flex-initial: flex: 0 1 auto;
.flex-none: flex: none;
.flex-between: display: flex; align-items: center; justify-content: space-between;
.flex-center: display: flex; align-items: center; justify-content: center;
.flex-around: display: flex; align-items: center; justify-content: space-around;
.flex-evenly: display: flex; align-items: center; justify-content: space-evenly;
.flex-start-between: display: flex; align-items: flex-start; justify-content: space-between;
.flex-end-between: display: flex; align-items: flex-end; justify-content: space-between;

</details>

<br />
Usage: Apply the class flex-{value} to create a flex container.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="flex"></div>
```
### Flex Basis
Description: Sets the initial size of a flex item.
<details>
<summary>Classes:</summary>
<br />

.basis-0: flex-basis: 0px;
.basis-1: flex-basis: 0.25rem; /* 4px */
.basis-2: flex-basis: 0.5rem; /* 8px */
.basis-3: flex-basis: 0.75rem; /* 12px */
.basis-4: flex-basis: 1rem; /* 16px */
.basis-5: flex-basis: 1.25rem; /* 20px */
.basis-6: flex-basis: 1.5rem; /* 24px */
.basis-7: flex-basis: 1.75rem; /* 28px */
.basis-8: flex-basis: 2rem; /* 32px */
.basis-9: flex-basis: 2.25rem; /* 36px */
.basis-10: flex-basis: 2.5rem; /* 40px */
.basis-11: flex-basis: 2.75rem; /* 44px */
.basis-12: flex-basis: 3rem; /* 48px */
.basis-14: flex-basis: 3.5rem; /* 56px */
.basis-16: flex-basis: 4rem; /* 64px */
.basis-20: flex-basis: 5rem; /* 80px */
.basis-24: flex-basis: 6rem; /* 96px */
.basis-28: flex-basis: 7rem; /* 112px */
.basis-32: flex-basis: 8rem; /* 128px */
.basis-36: flex-basis: 9rem; /* 144px */
.basis-40: flex-basis: 10rem; /* 160px */
.basis-44: flex-basis: 11rem; /* 176px */
.basis-48: flex-basis: 12rem; /* 192px */
.basis-52: flex-basis: 13rem; /* 208px */
.basis-56: flex-basis: 14rem; /* 224px */
.basis-60: flex-basis: 15rem; /* 240px */
.basis-64: flex-basis: 16rem; /* 256px */
.basis-72: flex-basis: 18rem; /* 288px */
.basis-80: flex-basis: 20rem; /* 320px */
.basis-96: flex-basis: 24rem; /* 384px */
.basis-auto: flex-basis: auto;
.basis-px: flex-basis: 1px;
.basis-0\.5: flex-basis: 0.125rem; /* 2px */
.basis-1\.5: flex-basis: 0.375rem; /* 6px */
.basis-2\.5: flex-basis: 0.625rem; /* 10px */
.basis-3\.5: flex-basis: 0.875rem; /* 14px */
.basis-1\/2: flex-basis: 50%;
.basis-1\/3: flex-basis: 33.333333%;
.basis-2\/3: flex-basis: 66.666667%;
.basis-1\/4: flex-basis: 25%;
.basis-2\/4: flex-basis: 50%;
.basis-3\/4: flex-basis: 75%;
.basis-1\/5: flex-basis: 20%;
.basis-2\/5: flex-basis: 40%;
.basis-3\/5: flex-basis: 60%;
.basis-4\/5: flex-basis: 80%;
.basis-1\/6: flex-basis: 16.666667%;
.basis-2\/6: flex-basis: 33.333333%;
.basis-3\/6: flex-basis: 50%;
.basis-4\/6: flex-basis: 66.666667%;
.basis-5\/6: flex-basis: 83.333333%;
.basis-1\/12: flex-basis: 8.333333%;
.basis-2\/12: flex-basis: 16.666667%;
.basis-3\/12: flex-basis: 25%;
.basis-4\/12: flex-basis: 33.333333%;
.basis-5\/12: flex-basis: 41.666667%;
.basis-6\/12: flex-basis: 50%;
.basis-7\/12: flex-basis: 58.333333%;
.basis-8\/12: flex-basis: 66.666667%;
.basis-9\/12: flex-basis: 75%;
.basis-10\/12: flex-basis: 83.333333%;
.basis-11\/12: flex-basis: 91.666667%;
.basis-full: flex-basis: 100%;

</details>

<br />
Usage: Apply the class basis-{value} to control the flex basis.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="basis-1"></div>
```
### Flex Direction
Description: Specifies the direction of the main axis in a flex container.
<details>
<summary>Classes:</summary>
<br />

.flex-row: flex-direction: row;
.flex-row-reverse: flex-direction: row-reverse;
.flex-col: flex-direction: column;
.flex-col-reverse: flex-direction: column-reverse;

</details>

<br />
Usage: Apply the class flex-{value} to control the flex direction.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="flex-row"></div>
```
### Flex Grow
Description: Sets the flexibility of a flex item to grow.
<details>
<summary>Classes:</summary>
<br />

.grow: flex-grow: 1;
.grow-0: flex-grow: 0;

</details>

<br />
Usage: Apply the class grow-{value} to control the flex grow property.

Example Usage:

```jsx
<div class="grow"></div>
```
### Flex Shrink
Description: Sets the flexibility of a flex item to shrink.
<details>
<summary>Classes:</summary>
<br />

.shrink: flex-shrink: 1;
.shrink-0: flex-shrink: 0;
</details>

<br />
Usage: Apply the class shrink-{value} to control the flex shrink property.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="shrink"></div>
```
### Flex Wrap
Description: Specifies whether flex items should wrap onto multiple lines.
<details>
<summary>Classes:</summary>
<br />

.flex-wrap: flex-wrap: wrap;
.flex-wrap-reverse: flex-wrap: wrap-reverse;
.flex-nowrap: flex-wrap: nowrap;

</details>

<br />
Usage: Apply the class flex-{value} to control the flex wrap property.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="flex-wrap"></div>
```
### Gap
Description: Sets the gap between grid and flex items.
<details>
<summary>Classes:</summary>
<br />

.g-0: gap: 0;
.g-2: gap: 2px;
.g-4: gap: 4px;
.g-6: gap: 6px;
.g-8: gap: 8px;
.g-10: gap: 10px;
.g-12: gap: 12px;
.g-14: gap: 14px;
.g-16: gap: 16px;
.g-18: gap: 18px;
.g-20: gap: 20px;
.g-24: gap: 24px;
.g-28: gap: 28px;
.g-32: gap: 32px;
.g-36: gap: 36px;
.g-40: gap: 40px;

.g-x-0: column-gap: 0;
.g-x-2: column-gap: 2px;
.g-x-4: column-gap: 4px;
.g-x-6: column-gap: 6px;
.g-x-8: column-gap: 8px;
.g-x-10: column-gap: 10px;
.g-x-12: column-gap: 12px;
.g-x-14: column-gap: 14px;
.g-x-16: column-gap: 16px;
.g-x-18: column-gap: 18px;
.g-x-20: column-gap: 20px;
.g-x-24: column-gap: 24px;
.g-x-28: column-gap: 28px;
.g-x-32: column-gap: 32px;
.g-x-36: column-gap: 36px;
.g-x-40: column-gap: 40px;

.g-y-0: row-gap: 0;
.g-y-2: row-gap: 2px;
.g-y-4: row-gap: 4px;
.g-y-6: row-gap: 6px;
.g-y-8: row-gap: 8px;
.g-y-10: row-gap: 10px;
.g-y-12: row-gap: 12px;
.g-y-14: row-gap: 14px;
.g-y-16: row-gap: 16px;
.g-y-18: row-gap: 18px;
.g-y-20: row-gap: 20px;
.g-y-24: row-gap: 24px;
.g-y-28: row-gap: 28px;
.g-y-32: row-gap: 32px;
.g-y-36: row-gap: 36px;
.g-y-40: row-gap: 40px;

</details>

<br />
Usage: Apply the class g-{value} to control the gap property.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="g-10"></div>
```
### Grid Auto
Description: Sets the size of additional grid tracks in a grid container.
<details>
<summary>Classes:</summary>
<br />

.grid-flow-row: grid-auto-flow: row;
.grid-flow-col: grid-auto-flow: column;
.grid-flow-dense: grid-auto-flow: dense;
.grid-flow-row-dense: grid-auto-flow: row dense;
.grid-flow-col-dense: grid-auto-flow: column dense;

.auto-cols-auto: grid-auto-columns: auto;
.auto-cols-min: grid-auto-columns: min-content;
.auto-cols-max: grid-auto-columns: max-content;
.auto-cols-fr: grid-auto-columns: minmax(0, 1fr);

.auto-rows-auto: grid-auto-rows: auto;
.auto-rows-min: grid-auto-rows: min-content;
.auto-rows-max: grid-auto-rows: max-content;
.auto-rows-fr: grid-auto-rows: minmax(0, 1fr);
</details>

<br />
Usage: Apply the class grid-{value} to control the grid auto property.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="grid-flow-row"></div>
```
### Grid Columns
Description: Specifies the size of the columns in a grid container.
<details>
<summary>Classes:</summary>
<br />

.grid-cols-1: grid-template-columns: repeat(1, minmax(0, 1fr));
.grid-cols-2: grid-template-columns: repeat(2, minmax(0, 1fr));
.grid-cols-3: grid-template-columns: repeat(3, minmax(0, 1fr));
.grid-cols-4: grid-template-columns: repeat(4, minmax(0, 1fr));
.grid-cols-5: grid-template-columns: repeat(5, minmax(0, 1fr));
.grid-cols-6: grid-template-columns: repeat(6, minmax(0, 1fr));
.grid-cols-7: grid-template-columns: repeat(7, minmax(0, 1fr));
.grid-cols-8: grid-template-columns: repeat(8, minmax(0, 1fr));
.grid-cols-9: grid-template-columns: repeat(9, minmax(0, 1fr));
.grid-cols-10: grid-template-columns: repeat(10, minmax(0, 1fr));
.grid-cols-11: grid-template-columns: repeat(11, minmax(0, 1fr));
.grid-cols-12: grid-template-columns: repeat(12, minmax(0, 1fr));
.grid-cols-none: grid-template-columns: none;

.col-auto: grid-column: auto;
.col-span-1: grid-column: span 1 / span 1;
.col-span-2: grid-column: span 2 / span 2;
.col-span-3: grid-column: span 3 / span 3;
.col-span-4: grid-column: span 4 / span 4;
.col-span-5: grid-column: span 5 / span 5;
.col-span-6: grid-column: span 6 / span 6;
.col-span-7: grid-column: span 7 / span 7;
.col-span-8: grid-column: span 8 / span 8;
.col-span-9: grid-column: span 9 / span 9;
.col-span-10: grid-column: span 10 / span 10;
.col-span-11: grid-column: span 11 / span 11;
.col-span-12: grid-column: span 12 / span 12;
.col-span-full: grid-column: 1 / -1;

.col-start-1: grid-column-start: 1;
.col-start-2: grid-column-start: 2;
.col-start-3: grid-column-start: 3;
.col-start-4: grid-column-start: 4;
.col-start-5: grid-column-start: 5;
.col-start-6: grid-column-start: 6;
.col-start-7: grid-column-start: 7;
.col-start-8: grid-column-start: 8;
.col-start-9: grid-column-start: 9;
.col-start-10: grid-column-start: 10;
.col-start-11: grid-column-start: 11;
.col-start-12: grid-column-start: 12;
.col-start-13: grid-column-start: 13;
.col-start-auto: grid-column-start: auto;

.col-end-1: grid-column-end: 1;
.col-end-2: grid-column-end: 2;
.col-end-3: grid-column-end: 3;
.col-end-4: grid-column-end: 4;
.col-end-5: grid-column-end: 5;
.col-end-6: grid-column-end: 6;
.col-end-7: grid-column-end: 7;
.col-end-8: grid-column-end: 8;
.col-end-9: grid-column-end: 9;
.col-end-10: grid-column-end: 10;
.col-end-11: grid-column-end: 11;
.col-end-12: grid-column-end: 12;
.col-end-13: grid-column-end: 13;
.col-end-auto: grid-column-end: auto;

</details>

<br />
Usage: Apply the class grid-cols-{value} and col-{value} to control the grid columns.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="grid-cols-1"></div>
```
### Grid Rows
Description: Specifies the size of the rows in a grid container.
<details>
<summary>Classes:</summary>
<br />

.grid-rows-1: grid-template-rows: repeat(1, minmax(0, 1fr));
.grid-rows-2: grid-template-rows: repeat(2, minmax(0, 1fr));
.grid-rows-3: grid-template-rows: repeat(3, minmax(0, 1fr));
.grid-rows-4: grid-template-rows: repeat(4, minmax(0, 1fr));
.grid-rows-5: grid-template-rows: repeat(5, minmax(0, 1fr));
.grid-rows-6: grid-template-rows: repeat(6, minmax(0, 1fr));
.grid-rows-none: grid-template-rows: none;

.row-auto: grid-row: auto;

.row-span-1: grid-row: span 1 / span 1;
.row-span-2: grid-row: span 2 / span 2;
.row-span-3: grid-row: span 3 / span 3;
.row-span-4: grid-row: span 4 / span 4;
.row-span-5: grid-row: span 5 / span 5;
.row-span-6: grid-row: span 6 / span 6;
.row-span-full: grid-row: 1 / -1;

.row-start-1: grid-row-start: 1;
.row-start-2: grid-row-start: 2;
.row-start-3: grid-row-start: 3;
.row-start-4: grid-row-start: 4;
.row-start-5: grid-row-start: 5;
.row-start-6: grid-row-start: 6;
.row-start-7: grid-row-start: 7;
.row-start-auto: grid-row-start: auto;

.row-end-1: grid-row-end: 1;
.row-end-2: grid-row-end: 2;
.row-end-3: grid-row-end: 3;
.row-end-4: grid-row-end: 4;
.row-end-5: grid-row-end: 5;
.row-end-6: grid-row-end: 6;
.row-end-7: grid-row-end: 7;
.row-end-auto: grid-row-end: auto;

</details>

<br />
Usage: Apply the class grid-rows-{value} and row-{value} to control the grid rows.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="grid-rows-2"></div>
```
### Justify
Description: Sets the alignment of an element along the main axis in a flex container.
<details>
<summary>Classes:</summary>
<br />

.justify-normal: justify-content: normal;
.justify-start: justify-content: flex-start;
.justify-end: justify-content: flex-end;
.justify-center: justify-content: center;
.justify-between: justify-content: space-between;
.justify-around: justify-content: space-around;
.justify-evenly: justify-content: space-evenly;
.justify-stretch: justify-content: stretch;

.justify-items-start: justify-items: start;
.justify-items-end: justify-items: end;
.justify-items-center: justify-items: center;
.justify-items-stretch: justify-items: stretch;

.justify-self-auto: justify-self: auto;
.justify-self-start: justify-self: start;
.justify-self-end: justify-self: end;
.justify-self-center: justify-self: center;
.justify-self-stretch: justify-self: stretch;

</details>

<br />
Usage: Apply the class justify-{value} to control the justification.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="justify-end"></div>
```
### Order
Description: Sets the order of a flex item.
<details>
<summary>Classes:</summary>
<br />

.order-1: order: 1;
.order-2: order: 2;
.order-3: order: 3;
.order-4: order: 4;
.order-5: order: 5;
.order-6: order: 6;
.order-7: order: 7;
.order-8: order: 8;
.order-9: order: 9;
.order-10: order: 10;
.order-11: order: 11;
.order-12: order: 12;
.order-first: order: -9999;
.order-last: order: 9999;
.order-none: order: 0;

</details>

<br />
Usage: Apply the class order-{value} to control the order.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="order-2"></div>
```
### Place
Description: Sets both the align and justify properties in a single shorthand property.
<details>
<summary>Classes:</summary>
<br />

Place Content
.place-content-center: place-content: center;
.place-content-start: place-content: start;
.place-content-end: place-content: end;
.place-content-between: place-content: space-between;
.place-content-around: place-content: space-around;
.place-content-evenly: place-content: space-evenly;
.place-content-baseline: place-content: baseline;
.place-content-stretch: place-content: stretch;

Place Items
.place-items-start: place-items: start;
.place-items-end: place-items: end;
.place-items-center: place-items: center;
.place-items-baseline: place-items: baseline;
.place-items-stretch: place-items: stretch;

Place Self
.place-self-auto: place-self: auto;
.place-self-start: place-self: start;
.place-self-end: place-self: end;
.place-self-center: place-self: center;
.place-self-stretch: place-self: stretch;

</details>

<br />
Usage: Apply the class place-content-{value}, place-items-{value} and place-self-{value} to control both alignment and justification.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="place-center-end"></div>
```
## Interactivity
### Appearance
Description: Controls the appearance of an element.
<details>
<summary>Classes:</summary>
<br />

.appearance-none: appearance-none: appearance: none;
</details>

<br />
Usage: Apply the class appearance-none to control the appearance property.
Browser Support: All modern browsers.
Example Usage:

```jsx
<button class="appearance-none"></button>
```
### Caret Color
Description: Sets the color of the caret in an editable text area.
<details>
<summary>Classes:</summary>
<br />

.caret-inherit: caret-color: inherit;
.caret-current: caret-color: currentColor;
.caret-transparent: caret-color: transparent;
.caret-black: caret-color: #000;
.caret-white: caret-color: #fff;

</details>

<br />
Usage: Apply the class caret-{value} to control the caret color.
Browser Support: All modern browsers.
Example Usage:

```jsx
<input type="text" class="caret-black">
```
### Cursor
Description: Specifies the type of cursor to be displayed.
<details>
<summary>Classes:</summary>
<br />
.cursor-auto: cursor: auto;
.cursor-default: cursor: default;
.cursor-pointer: cursor: pointer;
.cursor-wait: cursor: wait;
.cursor-text: cursor: text;
.cursor-move: cursor: move;
.cursor-help: cursor: help;
.cursor-not-allowed: cursor: not-allowed;
.cursor-none: cursor: none;
.cursor-context-menu: cursor: context-menu;
.cursor-progress: cursor: progress;
.cursor-cell: cursor: cell;
.cursor-crosshair: cursor: crosshair;
.cursor-vertical-text: cursor: vertical-text;
.cursor-alias: cursor: alias;
.cursor-copy: cursor: copy;
.cursor-no-drop: cursor: no-drop;
.cursor-grab: cursor: grab;
.cursor-grabbing: cursor: grabbing;
.cursor-all-scroll: cursor: all-scroll;
.cursor-col-resize: cursor: col-resize;
.cursor-row-resize: cursor: row-resize;
.cursor-n-resize: cursor: n-resize;
.cursor-e-resize: cursor: e-resize;
.cursor-s-resize: cursor: s-resize;
.cursor-w-resize: cursor: w-resize;
.cursor-ne-resize: cursor: ne-resize;
.cursor-nw-resize: cursor: nw-resize;
.cursor-se-resize: cursor: se-resize;
.cursor-sw-resize: cursor: sw-resize;
.cursor-ew-resize: cursor: ew-resize;
.cursor-ns-resize: cursor: ns-resize;
.cursor-nesw-resize: cursor: nesw-resize;
.cursor-nwse-resize: cursor: nwse-resize;
.cursor-zoom-in: cursor: zoom-in;
.cursor-zoom-out: cursor: zoom-out;

</details>

<br />
Usage: Apply the class cursor-{value} to control the cursor type.

Example Usage:

```jsx
<div class="cursor-pointer"></div>
```
### Pointer Events
Description: Specifies whether an element can be the target for pointer events.
<details>
<summary>Classes:</summary>
<br />

.pointer-events-none: pointer-events: none;

.pointer-events-auto: pointer-events: auto;
</details>

<br />
Usage: Apply the class pointer-events-{value} to control the pointer events.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="pointer-events-none"></div>
```
### Resize
Description: Specifies whether an element is resizable.
<details>
<summary>Classes:</summary>
<br />

.resize-none: resize: none;
.resize-y: resize: vertical;
.resize-x: resize: horizontal;
.resize: resize: both;

</details>

<br />
Usage: Apply the class resize-{value} to control the resize property.
Browser Support: All modern browsers.
Example Usage:

```jsx
<textarea class="resize-none"></textarea>
```
### Scroll
Description: Specifies the behavior of scrolling for an element.
<details>
<summary>Classes:</summary>
<br />

.scroll-auto: scroll-behavior: auto;
.scroll-smooth: scroll-behavior: smooth;

.scroll-m-0: scroll-margin: 0px;
.scroll-mx-0: scroll-margin-left: 0px; scroll-margin-right: 0px;
.scroll-my-0: scroll-margin-top: 0px; scroll-margin-bottom: 0px;
.scroll-ms-0: scroll-margin-inline-start: 0px;
.scroll-me-0: scroll-margin-inline-end: 0px;
.scroll-mt-0: scroll-margin-top: 0px;
.scroll-mr-0: scroll-margin-right: 0px;
.scroll-mb-0: scroll-margin-bottom: 0px;
.scroll-ml-0: scroll-margin-left: 0px;
.scroll-m-px: scroll-margin: 1px;
.scroll-mx-px: scroll-margin-left: 1px; scroll-margin-right: 1px;
.scroll-my-px: scroll-margin-top: 1px; scroll-margin-bottom: 1px;
.scroll-ms-px: scroll-margin-inline-start: 1px;
.scroll-me-px: scroll-margin-inline-end: 1px;
.scroll-m-0-5: scroll-margin: 0.125rem; /* 2px */
.scroll-mx-0-5: scroll-margin-left: 0.125rem; /* 2px */ scroll-margin-right: 0.125rem; /* 2px */
.scroll-my-0-5: scroll-margin-top: 0.125rem; /* 2px */ scroll-margin-bottom: 0.125rem; /* 2px */
.scroll-ms-0-5: scroll-margin-inline-start: 0.125rem; /* 2px */
.scroll-me-0-5: scroll-margin-inline-end: 0.125rem; /* 2px */
.scroll-m-1: scroll-margin: 0.25rem; /* 4px */
.scroll-mx-1: scroll-margin-left: 0.25rem; /* 4px */ scroll-margin-right: 0.25rem; /* 4px */
.scroll-my-1: scroll-margin-top: 0.25rem; /* 4px */ scroll-margin-bottom: 0.25rem; /* 4px */
.scroll-ms-1: scroll-margin-inline-start: 0.25rem; /* 4px */
.scroll-me-1: scroll-margin-inline-end: 0.25rem; /* 4px */
.scroll-m-1-5: scroll-margin: 0.375rem; /* 6px */
.scroll-mx-1-5: scroll-margin-left: 0.375rem; /* 6px */ scroll-margin-right: 0.375rem; /* 6px */
.scroll-my-1-5: scroll-margin-top: 0.375rem; /* 6px */ scroll-margin-bottom: 0.375rem; /* 6px */
.scroll-ms-1-5: scroll-margin-inline-start: 0.375rem; /* 6px */
.scroll-me-1-5: scroll-margin-inline-end: 0.375rem; /* 6px */
.scroll-m-2: scroll-margin: 0.5rem; /* 8px */
.scroll-mx-2: scroll-margin-left: 0.5rem; /* 8px */ scroll-margin-right: 0.5rem; /* 8px */
.scroll-my-2: scroll-margin-top: 0.5rem; /* 8px */ scroll-margin-bottom: 0.5rem; /* 8px */
.scroll-ms-2: scroll-margin-inline-start: 0.5rem; /* 8px */
.scroll-me-2: scroll-margin-inline-end: 0.5rem; /* 8px */

.scroll-p-0: scroll-padding: 0px;
.scroll-px-0: scroll-padding-left: 0px; scroll-padding-right: 0px;
.scroll-py-0: scroll-padding-top: 0px; scroll-padding-bottom: 0px;
.scroll-ps-0: scroll-padding-inline-start: 0px;
.scroll-pe-0: scroll-padding-inline-end: 0px;
.scroll-pt-0: scroll-padding-top: 0px;
.scroll-pr-0: scroll-padding-right: 0px;
.scroll-pb-0: scroll-padding-bottom: 0px;
.scroll-pl-0: scroll-padding-left: 0px;

.scroll-p-px: scroll-padding: 1px;
.scroll-px-px: scroll-padding-left: 1px; scroll-padding-right: 1px;
.scroll-py-px: scroll-padding-top: 1px; scroll-padding-bottom: 1px;

.snap-start: scroll-snap-align: start;
.snap-end: scroll-snap-align: end;
.snap-center: scroll-snap-align: center;
.snap-align-none: scroll-snap-align: none;
.snap-normal: scroll-snap-stop: normal;
.snap-always: scroll-snap-stop: always;
.snap-none: scroll-snap-type: none;
.snap-x: scroll-snap-type: x var(--scroll-snap-strictness);
.snap-y: scroll-snap-type: y var(--scroll-snap-strictness);
.snap-both: scroll-snap-type: both var(--scroll-snap-strictness);
.snap-mandatory: --scroll-snap-strictness: mandatory;
.snap-proximity: --scroll-snap-strictness: proximity;

</details>

<br />
Usage: Apply the class scroll-{value} to control the scroll behavior.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="scroll-auto"></div>
```
### Touch Action
Description: Specifies the touch behavior of an element.
<details>
<summary>Classes:</summary>
<br />

.touch-auto: touch-action: auto;
.touch-none: touch-action: none;
.touch-pan-x: touch-action: pan-x;
.touch-pan-left: touch-action: pan-left;
.touch-pan-right: touch-action: pan-right;
.touch-pan-y: touch-action: pan-y;
.touch-pan-up: touch-action: pan-up;
.touch-pan-down: touch-action: pan-down;
.touch-pinch-zoom: touch-action: pinch-zoom;
.touch-manipulation: touch-action: manipulation;

</details>

<br />
Usage: Apply the class touch-{value} to control the touch action.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="touch-auto"></div>
```
### User Select
Description: Controls the user's ability to select text.
<details>
<summary>Classes:</summary>
<br />

.select-none: user-select: none;
.select-text: user-select: text;
.select-all: user-select: all;
.select-auto: user-select: auto;

</details>

<br />
Usage: Apply the class select-{value} to control the user select.
Browser Support: All modern browsers.
Example Usage:

```jsx
<p class="select-none"></p>
```
### Will Change
Description: Informs the browser of the properties that may change, allowing it to optimize rendering.
<details>
<summary>Classes:</summary>
<br />

.will-change-auto: will-change: auto;
.will-change-scroll: will-change: scroll-position;
.will-change-contents: will-change: contents;
.will-change-transform: will-change: transform;

</details>

<br />
Usage: Apply the class will-change-{value} to control the will change property.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="will-change-auto"></div>
```
## Sizing
### Height
Description: Sets the height of an element.
<details>
<summary>Classes:</summary>
<br />

.h-0: height: 0px;
.h-px: height: 1px;
.h-0-5: height: 0.125rem; /* 2px */
.h-1: height: 0.25rem; /* 4px */
.h-1-5: height: 0.375rem; /* 6px */
.h-2: height: 0.5rem; /* 8px */
.h-2-5: height: 0.625rem; /* 10px */
.h-3: height: 0.75rem; /* 12px */
.h-3-5: height: 0.875rem; /* 14px */
.h-4: height: 1rem; /* 16px */
.h-5: height: 1.25rem; /* 20px */
.h-6: height: 1.5rem; /* 24px */
.h-7: height: 1.75rem; /* 28px */
.h-8: height: 2rem; /* 32px */
.h-9: height: 2.25rem; /* 36px */
.h-10: height: 2.5rem; /* 40px */
.h-11: height: 2.75rem; /* 44px */
.h-12: height: 3rem; /* 48px */
.h-14: height: 3.5rem; /* 56px */
.h-16: height: 4rem; /* 64px */
.h-20: height: 5rem; /* 80px */
.h-24: height: 6rem; /* 96px */
.h-28: height: 7rem; /* 112px */
.h-32: height: 8rem; /* 128px */
.h-36: height: 9rem; /* 144px */
.h-40: height: 10rem; /* 160px */
.h-44: height: 11rem; /* 176px */
.h-48: height: 12rem; /* 192px */
.h-52: height: 13rem; /* 208px */
.h-56: height: 14rem; /* 224px */
.h-60: height: 15rem; /* 240px */
.h-64: height: 16rem; /* 256px */
.h-72: height: 18rem; /* 288px */
.h-80: height: 20rem; /* 320px */
.h-96: height: 24rem; /* 384px */
.h-auto: height: auto;
.h-1-2: height: 50%;
.h-1-3: height: 33.333333%;
.h-2-3: height: 66.666667%;
.h-1-4: height: 25%;
.h-2-4: height: 50%;
.h-3-4: height: 75%;
.h-1-5: height: 20%;
.h-2-5: height: 40%;
.h-3-5: height: 60%;
.h-4-5: height: 80%;
.h-1-6: height: 16.666667%;
.h-2-6: height: 33.333333%;
.h-3-6: height: 50%;
.h-4-6: height: 66.666667%;
.h-5-6: height: 83.333333%;
.h-full: height: 100%;
.h-screen: height: 100vh;
.h-min: height: min-content;
.h-max: height: max-content;
.h-fit: height: fit-content;
.min-h-0: min-height: 0px;
.min-h-full: min-height: 100%;
.min-h-screen: min-height: 100vh;
.min-h-min: min-height: min-content;
.min-h-max: min-height: max-content;
.min-h-fit: min-height: fit-content;
.max-h-0: max-height: 0px;
.max-h-px: max-height: 1px;
.max-h-0-5: max-height: 0.125rem; /* 2px */
.max-h-1: max-height: 0.25rem; /* 4px */
.max-h-1-5: max-height: 0.375rem; /* 6px */
.max-h-2: max-height: 0.5rem; /* 8px */
.max-h-2-5: max-height: 0.625rem; /* 10px */
.max-h-3: max-height: 0.75rem; /* 12px */
.max-h-3-5: max-height: 0.875rem; /* 14px */
.max-h-4: max-height: 1rem; /* 16px */
.max-h-5: max-height: 1.25rem; /* 20px */
.max-h-6: max-height: 1.5rem; /* 24px */
.max-h-7: max-height: 1.75rem; /* 28px */
.max-h-8: max-height: 2rem; /* 32px */
.max-h-9: max-height: 2.25rem; /* 36px */
.max-h-10: max-height: 2.5rem; /* 40px */
.max-h-11: max-height: 2.75rem; /* 44px */
.max-h-12: max-height: 3rem; /* 48px */
.max-h-14: max-height: 3.5rem; /* 56px */
.max-h-16: max-height: 4rem; /* 64px */
.max-h-20: max-height: 5rem; /* 80px */
.max-h-24: max-height: 6rem; /* 96px */
.max-h-28: max-height: 7rem; /* 112px */
.max-h-32: max-height: 8rem; /* 128px */
.max-h-36: max-height: 9rem; /* 144px */
.max-h-40: max-height: 10rem; /* 160px */
.max-h-44: max-height: 11rem; /* 176px */
.max-h-48: max-height: 12rem; /* 192px */
.max-h-52: max-height: 13rem; /* 208px */
.max-h-56: max-height: 14rem; /* 224px */
.max-h-60: max-height: 15rem; /* 240px */
.max-h-64: max-height: 16rem; /* 256px */
.max-h-72: max-height: 18rem; /* 288px */
.max-h-80: max-height: 20rem; /* 320px */
.max-h-96: max-height: 24rem; /* 384px */
.max-h-none: max-height: none;
.max-h-full: max-height: 100%;
.max-h-screen: max-height: 100vh;
.max-h-min: max-height: min-content;
.max-h-max: max-height: max-content;
.max-h-fit: max-height: fit-content;

</details>

<br />
Usage: Apply the class h-{value} to control the height.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="h-full"></div>
```
### Width
Description: Sets the width of an element.
<details>
<summary>Classes:</summary>
<br />

.w-0: width: 0px;
.w-px: width: 1px;
.w-0-5: width: 0.125rem; /* 2px */
.w-1: width: 0.25rem; /* 4px */
.w-1-5: width: 0.375rem; /* 6px */
.w-2: width: 0.5rem; /* 8px */
.w-2-5: width: 0.625rem; /* 10px */
.w-3: width: 0.75rem; /* 12px */
.w-3-5: width: 0.875rem; /* 14px */
.w-4: width: 1rem; /* 16px */
.w-5: width: 1.25rem; /* 20px */
.w-6: width: 1.5rem; /* 24px */
.w-7: width: 1.75rem; /* 28px */
.w-8: width: 2rem; /* 32px */
.w-9: width: 2.25rem; /* 36px */
.w-10: width: 2.5rem; /* 40px */
.w-11: width: 2.75rem; /* 44px */
.w-12: width: 3rem; /* 48px */
.w-14: width: 3.5rem; /* 56px */
.w-16: width: 4rem; /* 64px */
.w-20: width: 5rem; /* 80px */
.w-24: width: 6rem; /* 96px */
.w-28: width: 7rem; /* 112px */
.w-32: width: 8rem; /* 128px */
.w-36: width: 9rem; /* 144px */
.w-40: width: 10rem; /* 160px */
.w-44: width: 11rem; /* 176px */
.w-48: width: 12rem; /* 192px */
.w-52: width: 13rem; /* 208px */
.w-56: width: 14rem; /* 224px */
.w-60: width: 15rem; /* 240px */
.w-64: width: 16rem; /* 256px */
.w-72: width: 18rem; /* 288px */
.w-80: width: 20rem; /* 320px */
.w-96: width: 24rem; /* 384px */
.w-auto: width: auto;
.w-1-2: width: 50%;
.w-1-3: width: 33.333333%;
.w-2-3: width: 66.666667%;
.w-1-4: width: 25%;
.w-2-4: width: 50%;
.w-3-4: width: 75%;
.w-1-5: width: 20%;
.w-2-5: width: 40%;
.w-3-5: width: 60%;
.w-4-5: width: 80%;
.w-1-6: width: 16.666667%;
.w-2-6: width: 33.333333%;
.w-3-6: width: 50%;
.w-4-6: width: 66.666667%;
.w-5-6: width: 83.333333%;
.w-1-12: width: 8.333333%;
.w-2-12: width: 16.666667%;
.w-3-12: width: 25%;
.w-4-12: width: 33.333333%;
.w-5-12: width: 41.666667%;
.w-6-12: width: 50%;
.w-7-12: width: 58.333333%;
.w-8-12: width: 66.666667%;
.w-9-12: width: 75%;
.w-10-12: width: 83.333333%;
.w-11-12: width: 91.666667%;
.w-full: width: 100%;
.w-screen: width: 100vw;
.w-min: width: min-content;
.w-max: width: max-content;
.w-fit: width: fit-content;
.min-w-0: min-width: 0px;
.min-w-full: min-width: 100%;
.min-w-min: min-width: min-content;
.min-w-max: min-width: max-content;
.min-w-fit: min-width: fit-content;
.max-w-0: max-width: 0rem; /* 0px */
.max-w-none: max-width: none;
.max-w-xs: max-width: 20rem; /* 320px */
.max-w-sm: max-width: 24rem; /* 384px */
.max-w-md: max-width: 28rem; /* 448px */
.max-w-lg: max-width: 32rem; /* 512px */
.max-w-xl: max-width: 36rem; /* 576px */
.max-w-2xl: max-width: 42rem; /* 672px */
.max-w-3xl: max-width: 48rem; /* 768px */
.max-w-4xl: max-width: 56rem; /* 896px */
.max-w-5xl: max-width: 64rem; /* 1024px */
.max-w-6xl: max-width: 72rem; /* 1152px */
.max-w-7xl: max-width: 80rem; /* 1280px */
.max-w-full: max-width: 100%;
.max-w-min: max-width: min-content;
.max-w-max: max-width: max-content;
.max-w-fit: max-width: fit-content;
.max-w-prose: max-width: 65ch;
.max-w-screen-sm: max-width: 640px;
.max-w-screen-md: max-width: 768px;
.max-w-screen-lg: max-width: 1024px;
.max-w-screen-xl: max-width: 1280px;
.max-w-screen-2xl: max-width: 1536px;

</details>

<br />
Usage: Apply the class w-{value} to control the width.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="w-full"></div>
```
## Spacing
### Margin
Description: Sets the margin space around an element.
<details>
<summary>Classes:</summary>
<br />

Margin
.m-0: margin: 0px;
.m-2: margin: 2px;
.m-4: margin: 4px;
.m-6: margin: 6px;
.m-8: margin: 8px;
.m-10: margin: 10px;
.m-12: margin: 12px;
.m-14: margin: 14px;
.m-16: margin: 16px;
.m-20: margin: 20px;
.m-24: margin: 24px;
.m-28: margin: 28px;
.m-32: margin: 32px;
.m-36: margin: 36px;
.m-40: margin: 40px;
Margin Left
.ml-0: margin-left: 0px;
.ml-2: margin-left: 2px;
.ml-4: margin-left: 4px;
.ml-6: margin-left: 6px;
.ml-8: margin-left: 8px;
.ml-10: margin-left: 10px;
.ml-12: margin-left: 12px;
.ml-14: margin-left: 14px;
.ml-16: margin-left: 16px;
.ml-20: margin-left: 20px;
.ml-24: margin-left: 24px;
.ml-28: margin-left: 28px;
.ml-32: margin-left: 32px;
.ml-36: margin-left: 36px;
.ml-40: margin-left: 40px;
Margin Right
.mr-0: margin-right: 0px;
.mr-2: margin-right: 2px;
.mr-4: margin-right: 4px;
.mr-6: margin-right: 6px;
.mr-8: margin-right: 8px;
.mr-10: margin-right: 10px;
.mr-12: margin-right: 12px;
.mr-14: margin-right: 14px;
.mr-16: margin-right: 16px;
.mr-20: margin-right: 20px;
.mr-24: margin-right: 24px;
.mr-28: margin-right: 28px;
.mr-32: margin-right: 32px;
.mr-36: margin-right: 36px;
.mr-40: margin-right: 40px;
Margin Bottom
.mb-0: margin-bottom: 0px;
.mb-2: margin-bottom: 2px;
.mb-4: margin-bottom: 4px;
.mb-6: margin-bottom: 6px;
.mb-8: margin-bottom: 8px;
.mb-10: margin-bottom: 10px;
.mb-12: margin-bottom: 12px;
.mb-14: margin-bottom: 14px;
.mb-16: margin-bottom: 16px;
.mb-20: margin-bottom: 20px;
.mb-24: margin-bottom: 24px;
.mb-28: margin-bottom: 28px;
.mb-32: margin-bottom: 32px;
.mb-36: margin-bottom: 36px;
.mb-40: margin-bottom: 40px;
Margin top
.mt-0: margin-top: 0px;
.mt-2: margin-top: 2px;
.mt-4: margin-top: 4px;
.mt-6: margin-top: 6px;
.mt-8: margin-top: 8px;
.mt-10: margin-top: 10px;
.mt-12: margin-top: 12px;
.mt-14: margin-top: 14px;
.mt-16: margin-top: 16px;
.mt-20: margin-top: 20px;
.mt-24: margin-top: 24px;
.mt-28: margin-top: 28px;
.mt-32: margin-top: 32px;
.mt-36: margin-top: 36px;
.mt-40: margin-top: 40px;
Margin X (Horizontal)
.mx-0: margin-left: 0px; margin-right: 0px;
.mx-2: margin-left: 2px; margin-right: 2px;
.mx-4: margin-left: 4px; margin-right: 4px;
.mx-6: margin-left: 6px; margin-right: 6px;
.mx-8: margin-left: 8px; margin-right: 8px;
.mx-10: margin-left: 10px; margin-right: 10px;
.mx-12: margin-left: 12px; margin-right: 12px;
.mx-14: margin-left: 14px; margin-right: 14px;
.mx-16: margin-left: 16px; margin-right: 16px;
.mx-20: margin-left: 20px; margin-right: 20px;
.mx-24: margin-left: 24px; margin-right: 24px;
.mx-28: margin-left: 28px; margin-right: 28px;
.mx-32: margin-left: 32px; margin-right: 32px;
.mx-36: margin-left: 36px; margin-right: 36px;
.mx-40: margin-left: 40px; margin-right: 40px;
Margin Y (Vertical)
.my-0: margin-top: 0px; margin-bottom: 0px;
.my-2: margin-top: 2px; margin-bottom: 2px;
.my-4: margin-top: 4px; margin-bottom: 4px;
.my-6: margin-top: 6px; margin-bottom: 6px;
.my-8: margin-top: 8px; margin-bottom: 8px;
.my-10: margin-top: 10px; margin-bottom: 10px;
.my-12: margin-top: 12px; margin-bottom: 12px;
.my-14: margin-top: 14px; margin-bottom: 14px;
.my-16: margin-top: 16px; margin-bottom: 16px;
.my-20: margin-top: 20px; margin-bottom: 20px;
.my-24: margin-top: 24px; margin-bottom: 24px;
.my-28: margin-top: 28px; margin-bottom: 28px;
.my-32: margin-top: 32px; margin-bottom: 32px;
.my-36: margin-top: 36px; margin-bottom: 36px;
.my-40: margin-top: 40px; margin-bottom: 40px;
Margin Inline-Start (ps)
.ms-0: margin-inline-start: 0px;
.ms-2: margin-inline-start: 2px;
.ms-4: margin-inline-start: 4px;
.ms-6: margin-inline-start: 6px;
.ms-8: margin-inline-start: 8px;
.ms-10: margin-inline-start: 10px;
.ms-12: margin-inline-start: 12px;
.ms-14: margin-inline-start: 14px;
.ms-16: margin-inline-start: 16px;
.ms-20: margin-inline-start: 20px;
.ms-24: margin-inline-start: 24px;
.ms-28: margin-inline-start: 28px;
.ms-32: margin-inline-start: 32px;
.ms-36: margin-inline-start: 36px;
.ms-40: margin-inline-start: 40px;
Margin Inline-End (pe)
.me-0: margin-inline-end: 0px;
.me-2: margin-inline-end: 2px;
.me-4: margin-inline-end: 4px;
.me-6: margin-inline-end: 6px;
.me-8: margin-inline-end: 8px;
.me-10: margin-inline-end: 10px;
.me-12: margin-inline-end: 12px;
.me-14: margin-inline-end: 14px;
.me-16: margin-inline-end: 16px;
.me-20: margin-inline-end: 20px;
.me-24: margin-inline-end: 24px;
.me-28: margin-inline-end: 28px;
.me-32: margin-inline-end: 32px;
.me-36: margin-inline-end: 36px;
.me-40: margin-inline-end: 40px;
Margin Auto
.m-auto: margin: auto;
Margin X Auto
.mx-auto: margin-left: auto; margin-right: auto;
Margin Y Auto
.my-auto: margin-top: auto; margin-bottom: auto;
Margin Start Auto
.ms-auto: margin-inline-start: auto;
Margin End Auto
.me-auto: margin-inline-end: auto;
Margin Top Auto
.mt-auto: margin-top: auto;
Margin Right Auto
.mr-auto: margin-right: auto;
Margin Bottom Auto
.mb-auto: margin-bottom: auto;
Margin Left Auto
.ml-auto: margin-left: auto;
</details>

<br />
Usage: Apply the class m-{value} to control the margin.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="m-20"></div>
```
### Padding
Description: Sets the padding space inside an element.
<details>
<summary>Classes:</summary>
<br />

Padding
.p-0 :padding: 0px;
.p-2 :padding: 2px;
.p-4 :padding: 4px;
.p-6 :padding: 6px;
.p-8 :padding: 8px;
.p-10 :padding: 10px;
.p-12 :padding: 12px;
.p-14 :padding: 14px;
.p-16 :padding: 16px;
.p-20 :padding: 20px;
.p-24 :padding: 24px;
.p-28 :padding: 28px;
.p-32 :padding: 32px;
.p-36 :padding: 36px;
.p-40 :padding: 40px;
Padding Left
.pl-0 :padding-left: 0px;
.pl-2 :padding-left: 2px;
.pl-4 :padding-left: 4px;
.pl-6 :padding-left: 6px;
.pl-8 :padding-left: 8px;
.pl-10 :padding-left: 10px;
.pl-12 :padding-left: 12px;
.pl-14 :padding-left: 14px;
.pl-16 :padding-left: 16px;
.pl-20 :padding-left: 20px;
.pl-24 :padding-left: 24px;
.pl-28 :padding-left: 28px;
.pl-32 :padding-left: 32px;
.pl-36 :padding-left: 36px;
.pl-40 :padding-left: 40px;
Padding Right
.pr-0 :padding-right: 0px;
.pr-2 :padding-right: 2px;
.pr-4 :padding-right: 4px;
.pr-6 :padding-right: 6px;
.pr-8 :padding-right: 8px;
.pr-10 :padding-right: 10px;
.pr-12 :padding-right: 12px;
.pr-14 :padding-right: 14px;
.pr-16 :padding-right: 16px;
.pr-20 :padding-right: 20px;
.pr-24 :padding-right: 24px;
.pr-28 :padding-right: 28px;
.pr-32 :padding-right: 32px;
.pr-36 :padding-right: 36px;
.pr-40 :padding-right: 40px;
Padding Bottom
.pb-0 :padding-bottom: 0px;
.pb-2 :padding-bottom: 2px;
.pb-4 :padding-bottom: 4px;
.pb-6 :padding-bottom: 6px;
.pb-8 :padding-bottom: 8px;
.pb-10 :padding-bottom: 10px;
.pb-12 :padding-bottom: 12px;
.pb-14 :padding-bottom: 14px;
.pb-16 :padding-bottom: 16px;
.pb-20 :padding-bottom: 20px;
.pb-24 :padding-bottom: 24px;
.pb-28 :padding-bottom: 28px;
.pb-32 :padding-bottom: 32px;
.pb-36 :padding-bottom: 36px;
.pb-40 :padding-bottom: 40px;
Padding top
.pt-0 :padding-top: 0px;
.pt-2 :padding-top: 2px;
.pt-4 :padding-top: 4px;
.pt-6 :padding-top: 6px;
.pt-8 :padding-top: 8px;
.pt-10 :padding-top: 10px;
.pt-12 :padding-top: 12px;
.pt-14 :padding-top: 14px;
.pt-16 :padding-top: 16px;
.pt-20 :padding-top: 20px;
.pt-24 :padding-top: 24px;
.pt-28 :padding-top: 28px;
.pt-32 :padding-top: 32px;
.pt-36 :padding-top: 36px;
.pt-40 :padding-top: 40px;
Padding X (Horizontal)
.px-0 :padding-left: 0px:padding-right: 0px;
.px-2 :padding-left: 2px:padding-right: 2px;
.px-4 :padding-left: 4px:padding-right: 4px;
.px-6 :padding-left: 6px:padding-right: 6px;
.px-8 :padding-left: 8px:padding-right: 8px;
.px-10 :padding-left: 10px:padding-right: 10px;
.px-12 :padding-left: 12px:padding-right: 12px;
.px-14 :padding-left: 14px:padding-right: 14px;
.px-16 :padding-left: 16px:padding-right: 16px;
.px-20 :padding-left: 20px:padding-right: 20px;
.px-24 :padding-left: 24px:padding-right: 24px;
.px-28 :padding-left: 28px:padding-right: 28px;
.px-32 :padding-left: 32px:padding-right: 32px;
.px-36 :padding-left: 36px:padding-right: 36px;
.px-40 :padding-left: 40px:padding-right: 40px;
Padding Y (Vertical)
.py-0 :padding-top: 0px:padding-bottom: 0px;
.py-2 :padding-top: 2px:padding-bottom: 2px;
.py-4 :padding-top: 4px:padding-bottom: 4px;
.py-6 :padding-top: 6px:padding-bottom: 6px;
.py-8 :padding-top: 8px:padding-bottom: 8px;
.py-10 :padding-top: 10px:padding-bottom: 10px;
.py-12 :padding-top: 12px:padding-bottom: 12px;
.py-14 :padding-top: 14px:padding-bottom: 14px;
.py-16 :padding-top: 16px:padding-bottom: 16px;
.py-20 :padding-top: 20px:padding-bottom: 20px;
.py-24 :padding-top: 24px:padding-bottom: 24px;
.py-28 :padding-top: 28px:padding-bottom: 28px;
.py-32 :padding-top: 32px:padding-bottom: 32px;
.py-36 :padding-top: 36px:padding-bottom: 36px;
.py-40 :padding-top: 40px:padding-bottom: 40px;
Padding Inline-Start (ps)
.ps-0 :padding-inline-start: 0px;
.ps-2 :padding-inline-start: 2px;
.ps-4 :padding-inline-start: 4px;
.ps-6 :padding-inline-start: 6px;
.ps-8 :padding-inline-start: 8px;
.ps-10 :padding-inline-start: 10px;
.ps-12 :padding-inline-start: 12px;
.ps-14 :padding-inline-start: 14px;
.ps-16 :padding-inline-start: 16px;
.ps-20 :padding-inline-start: 20px;
.ps-24 :padding-inline-start: 24px;
.ps-28 :padding-inline-start: 28px;
.ps-32 :padding-inline-start: 32px;
.ps-36 :padding-inline-start: 36px;
.ps-40 :padding-inline-start: 40px;
Padding Inline-End (pe)
.pe-0 :padding-inline-end: 0px;
.pe-2 :padding-inline-end: 2px;
.pe-4 :padding-inline-end: 4px;
.pe-6 :padding-inline-end: 6px;
.pe-8 :padding-inline-end: 8px;
.pe-10 :padding-inline-end: 10px;
.pe-12 :padding-inline-end: 12px;
.pe-14 :padding-inline-end: 14px;
.pe-16 :padding-inline-end: 16px;
.pe-20 :padding-inline-end: 20px;
.pe-24 :padding-inline-end: 24px;
.pe-28 :padding-inline-end: 28px;
.pe-32 :padding-inline-end: 32px;
.pe-36 :padding-inline-end: 36px;
.pe-40 :padding-inline-end: 40px;

</details>

<br />
Usage: Apply the class p-{value} to control the padding.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="p-10"></div>
```
### Space
Description: Sets both margin and padding spaces around an element.
<details>
<summary>Classes:</summary>
<br />

Space Between Utilities

Horizontal Space Between
.space-x-0 > * + *:margin-left: 0px;
.space-x-0-5 > * + *:margin-left: 0.125rem; /* 2px */
.space-x-1 > * + *:margin-left: 0.25rem; /* 4px */
.space-x-1-5 > * + *:margin-left: 0.375rem; /* 6px */
.space-x-2 > * + *:margin-left: 0.5rem; /* 8px */
.space-x-2-5 > * + *:margin-left: 0.625rem; /* 10px */
.space-x-3 > * + *:margin-left: 0.75rem; /* 12px */
.space-x-3-5 > * + *:margin-left: 0.875rem; /* 14px */
.space-x-4 > * + *:margin-left: 1rem; /* 16px */
Vertical Space Between
.space-y-0 > * + *:margin-top: 0px;
.space-y-0-5 > * + *:margin-top: 0.125rem; /* 2px */
.space-y-1 > * + *:margin-top: 0.25rem; /* 4px */
.space-y-1-5 > * + *:margin-top: 0.375rem; /* 6px */
.space-y-2 > * + *:margin-top: 0.5rem; /* 8px */
.space-y-2-5 > * + *:margin-top: 0.625rem; /* 10px */
.space-y-3 > * + *:margin-top: 0.75rem; /* 12px */
.space-y-3-5 > * + *:margin-top: 0.875rem; /* 14px */
.space-y-4 > * + *:margin-top: 1rem; /* 16px */
</details>

<br />
Usage: Apply the class space-{value} to control both margin and padding.
Browser Support: All modern browsers.
Example Usage:

```jsx
<div class="space-x-0"></div>
```
## SVG
### Fill
Description: Sets the fill color of an SVG element.
<details>
<summary>Classes:</summary>
<br />

.fill-none: fill: none;
.fill-inherit: fill: inherit;
.fill-current: fill: currentColor;
.fill-transparent: fill: transparent;
.fill-black: fill: #000;
.fill-white: fill: #fff;

</details>

<br />
Usage: Apply the class fill-{value} to control the fill color.
Browser Support: All modern browsers.
Example Usage:

```jsx
<svg class="fill-none" width="100" height="100">
  <circle cx="50" cy="50" r="40" />
</svg>
```
### Stroke
Description: Sets the stroke color of an SVG element.
<details>
<summary>Classes:</summary>
<br />

.stroke-none: stroke: none;
.stroke-inherit: stroke: inherit;
.stroke-current: stroke: currentColor;
.stroke-transparent: stroke: transparent;
.stroke-black: stroke: #000;
.stroke-white: stroke: #fff;

Stroke Width Utilities
.stroke-0: stroke-width: 0;
.stroke-1: stroke-width: 1;
.stroke-2: stroke-width: 2;

</details>

<br />
Usage: Apply the class stroke-{value} to control the stroke color.
Browser Support: All modern browsers.
Example Usage:

```jsx
<svg class="troke-inherit" width="100" height="100">
  <circle cx="50" cy="50" r="40" />
</svg>
```


## Tables
### Border Collapse
Description: Specifies whether table borders should be collapsed into a single border or separated.
<details>
<summary>Classes:</summary>
<br />

.border-collapse: border-collapse: collapse;
.border-separate: border-collapse: separate;
</details>

<br />
Usage: Apply the class border-{value} to control the border-collapse property.
Browser Support: All modern browsers.
Example Usage:

```jsx
<table class="border-collapse"></table>
```
### Border Spacing
Description: Sets the distance between the borders of adjacent table cells.
<details>
<summary>Classes:</summary>
<br />

.border-spacing-0: border-spacing: 0px 0px;
.border-spacing-x-0: border-spacing: 0px var(--border-spacing-y);
.border-spacing-y-0: border-spacing: var(--border-spacing-x) 0px;
.border-spacing-px: border-spacing: 1px 1px;
.border-spacing-x-px: border-spacing: 1px var(--border-spacing-y);
.border-spacing-y-px: border-spacing: var(--border-spacing-x) 1px;
.border-spacing-0-5: border-spacing: 0.125rem 0.125rem;
.border-spacing-x-0-5: border-spacing: 0.125rem var(--border-spacing-y);
.border-spacing-y-0-5: border-spacing: var(--border-spacing-x) 0.125rem;
.border-spacing-1: border-spacing: 0.25rem 0.25rem;
.border-spacing-x-1: border-spacing: 0.25rem var(--border-spacing-y);
.border-spacing-y-1: border-spacing: var(--border-spacing-x) 0.25rem;
.border-spacing-1-5: border-spacing: 0.375rem 0.375rem;
.border-spacing-x-1-5: border-spacing: 0.375rem var(--border-spacing-y);
.border-spacing-y-1-5: border-spacing: var(--border-spacing-x) 0.375rem;
.border-spacing-2: border-spacing: 0.5rem 0.5rem;
.border-spacing-x-2: border-spacing: 0.5rem var(--border-spacing-y);
.border-spacing-y-2: border-spacing: var(--border-spacing-x) 0.5rem;
.border-spacing-2-5: border-spacing: 0.625rem 0.625rem;
.border-spacing-x-2-5: border-spacing: 0.625rem var(--border-spacing-y);
.border-spacing-y-2-5: border-spacing: var(--border-spacing-x) 0.625rem;
.border-spacing-3: border-spacing: 0.75rem 0.75rem;
.border-spacing-x-3: border-spacing: 0.75rem var(--border-spacing-y);
.border-spacing-y-3: border-spacing: var(--border-spacing-x) 0.75rem;
.border-spacing-3-5: border-spacing: 0.875rem 0.875rem;
.border-spacing-x-3-5: border-spacing: 0.875rem var(--border-spacing-y);
.border-spacing-y-3-5: border-spacing: var(--border-spacing-x) 0.875rem;
.border-spacing-4: border-spacing: 1rem 1rem;
.border-spacing-x-4: border-spacing: 1rem var(--border-spacing-y);
.border-spacing-y-4: border-spacing: var(--border-spacing-x) 1rem;
.border-spacing-5: border-spacing: 1.25rem 1.25rem;
.border-spacing-x-5: border-spacing: 1.25rem var(--border-spacing-y);
.border-spacing-y-5: border-spacing: var(--border-spacing-x) 1.25rem;
.border-spacing-6: border-spacing: 1.5rem 1.5rem;
.border-spacing-x-6: border-spacing: 1.5rem var(--border-spacing-y);
.border-spacing-y-6: border-spacing: var(--border-spacing-x) 1.5rem;
.border-spacing-7: border-spacing: 1.75rem 1.75rem;
.border-spacing-x-7: border-spacing: 1.75rem var(--border-spacing-y);
.border-spacing-y-7: border-spacing: var(--border-spacing-x) 1.75rem;
.border-spacing-8: border-spacing: 2rem 2rem;
.border-spacing-x-8: border-spacing: 2rem var(--border-spacing-y);
.border-spacing-y-8: border-spacing: var(--border-spacing-x) 2rem;
.border-spacing-9: border-spacing: 2.25rem 2.25rem;
.border-spacing-x-9: border-spacing: 2.25rem var(--border-spacing-y);
.border-spacing-y-9: border-spacing: var(--border-spacing-x) 2.25rem;
.border-spacing-10: border-spacing: 2.5rem 2.5rem;
.border-spacing-x-10: border-spacing: 2.5rem var(--border-spacing-y);
.border-spacing-y-10: border-spacing: var(--border-spacing-x) 2.5rem;
.border-spacing-11: border-spacing: 2.75rem 2.75rem;
.border-spacing-x-11: border-spacing: 2.75rem var(--border-spacing-y);
.border-spacing-y-11: border-spacing: var(--border-spacing-x) 2.75rem;
.border-spacing-12: border-spacing: 3rem 3rem;
.border-spacing-x-12: border-spacing: 3rem var(--border-spacing-y);
.border-spacing-y-12: border-spacing: var(--border-spacing-x) 3rem;
.border-spacing-14: border-spacing: 3.5rem 3.5rem;
.border-spacing-x-14: border-spacing: 3.5rem var(--border-spacing-y);
.border-spacing-y-14: border-spacing: var(--border-spacing-x) 3.5rem;
.border-spacing-16: border-spacing: 4rem 4rem;
.border-spacing-x-16: border-spacing: 4rem var(--border-spacing-y);
.border-spacing-y-16: border-spacing: var(--border-spacing-x) 4rem;
.border-spacing-20: border-spacing: 5rem 5rem;
.border-spacing-x-20: border-spacing: 5rem var(--border-spacing-y);
.border-spacing-y-20: border-spacing: var(--border-spacing-x) 5rem;
.border-spacing-24: border-spacing: 6rem 6rem;
.border-spacing-x-24: border-spacing: 6rem var(--border-spacing-y);
.border-spacing-y-24: border-spacing: var(--border-spacing-x) 6rem;
.border-spacing-28: border-spacing: 7rem 7rem;
.border-spacing-x-28: border-spacing: 7rem var(--border-spacing-y);
.border-spacing-y-28: border-spacing: var(--border-spacing-x) 7rem;
.border-spacing-32: border-spacing: 8rem 8rem;
.border-spacing-x-32: border-spacing: 8rem var(--border-spacing-y);
.border-spacing-y-32: border-spacing: var(--border-spacing-x) 8rem;
.border-spacing-36: border-spacing: 9rem 9rem;
.border-spacing-x-36: border-spacing: 9rem var(--border-spacing-y);
.border-spacing-y-36: border-spacing: var(--border-spacing-x) 9rem;
.border-spacing-40: border-spacing: 10rem 10rem;
.border-spacing-x-40: border-spacing: 10rem var(--border-spacing-y);
.border-spacing-y-40: border-spacing: var(--border-spacing-x) 10rem;
</details>

<br />
Usage: Apply the class border-spacing-{value} to control the border-spacing property.
Browser Support: All modern browsers.
Example Usage:

```jsx
<table class="border-spacing-5"></table>
```
### Caption Side
Description: Specifies the placement of the table caption.
<details>
<summary>Classes:</summary>
<br />

.caption-top: caption-side: top;
.caption-bottom: caption-side: bottom;
</details>

<br />
Usage: Apply the class caption-{value} to control the caption-side property.
Browser Support: All modern browsers.
Example Usage:

```jsx
<table class="caption-top">
  <caption>Table Caption</caption>
</table>
```
### Table Layout
Description: Specifies the algorithm used to lay out the table cells, rows, and columns.
<details>
<summary>Classes:</summary>
<br />

.table-auto: table-layout: auto;
.table-fixed: table-layout: fixed;
</details>

<br />
Usage: Apply the class table-{value} to control the table-layout property.
Browser Support: All modern browsers.
Example Usage:

```jsx
<table class="table-auto"></table>
```
## Transforms
### Rotate
Description: Rotates an element around a fixed point.
<details>
<summary>Classes:</summary>
<br />

.rotate-0: transform: rotate(0deg);
.rotate-1: transform: rotate(1deg);
.rotate-2: transform: rotate(2deg);
.rotate-3: transform: rotate(3deg);
.rotate-6: transform: rotate(6deg);
.rotate-12: transform: rotate(12deg);
.rotate-45: transform: rotate(45deg);
.rotate-90: transform: rotate(90deg);
.rotate-180: transform: rotate(180deg);

</details>

<br />
Usage: Apply the class rotate-{value} to control the rotation.

Example Usage:

```jsx
<div class="rotate-45"></div>
```
### Scale
Description: Scales an element by modifying its dimensions.
<details>
<summary>Classes:</summary>
<br />

.scale-0: transform: scale(0);
.scale-x-0: transform: scaleX(0);
.scale-y-0: transform: scaleY(0);
.scale-50: transform: scale(0.5);
.scale-x-50: transform: scaleX(0.5);
.scale-y-50: transform: scaleY(0.5);
.scale-75: transform: scale(0.75);
.scale-x-75: transform: scaleX(0.75);
.scale-y-75: transform: scaleY(0.75);
.scale-90: transform: scale(0.9);
.scale-x-90: transform: scaleX(0.9);
.scale-y-90: transform: scaleY(0.9);
.scale-95: transform: scale(0.95);
.scale-x-95: transform: scaleX(0.95);
.scale-y-95: transform: scaleY(0.95);
.scale-100: transform: scale(1);
.scale-x-100: transform: scaleX(1);
.scale-y-100: transform: scaleY(1);
.scale-105: transform: scale(1.05);
.scale-x-105: transform: scaleX(1.05);
.scale-y-105: transform: scaleY(1.05);
.scale-110: transform: scale(1.1);
.scale-x-110: transform: scaleX(1.1);
.scale-y-110: transform: scaleY(1.1);
.scale-125: transform: scale(1.25);
.scale-x-125: transform: scaleX(1.25);
.scale-y-125: transform: scaleY(1.25);
.scale-150: transform: scale(1.5);
.scale-x-150: transform: scaleX(1.5);
.scale-y-150: transform: scaleY(1.5);

</details>

<br />
Usage: Apply the class scale-{value} to control the scaling.

Example Usage:

```jsx
<div class="scale-2"></div>
```
### Skew
Description: Skews an element along the X and/or Y-axis.
<details>
<summary>Classes:</summary>
<br />

.skew-x-0: transform: skewX(0deg);
.skew-y-0: transform: skewY(0deg);
.skew-x-1: transform: skewX(1deg);
.skew-y-1: transform: skewY(1deg);
.skew-x-2: transform: skewX(2deg);
.skew-y-2: transform: skewY(2deg);
.skew-x-3: transform: skewX(3deg);
.skew-y-3: transform: skewY(3deg);
.skew-x-6: transform: skewX(6deg);
.skew-y-6: transform: skewY(6deg);
.skew-x-12: transform: skewX(12deg);
.skew-y-12: transform: skewY(12deg);

</details>

<br />
Usage: Apply the class skew-{value} to control the skewing along the X and Y axes.

Example Usage:

```jsx
<div class="skew-x-1"></div>
```
### Transform Origin
Description: Sets the origin point for transformations.
<details>
<summary>Classes:</summary>
<br />

.origin-center: transform-origin: center;
.origin-top: transform-origin: top;
.origin-top-right: transform-origin: top right;
.origin-right: transform-origin: right;
.origin-bottom-right: transform-origin: bottom right;
.origin-bottom: transform-origin: bottom;
.origin-bottom-left: transform-origin: bottom left;
.origin-left: transform-origin: left;
.origin-top-left: transform-origin: top left;

</details>

<br />
Usage: Apply the class origin-{value} to control the transform origin.

Example Usage:

```jsx
<div class="origin-center"></div>
```
### Translate
Description: Moves an element along the X and/or Y-axis.
<details>
<summary>Classes:</summary>
<br />

.translate-x-0: transform: translateX(0px);
.translate-y-0: transform: translateY(0px);
.translate-x-px: transform: translateX(1px);
.translate-y-px: transform: translateY(1px);
.translate-x-0-5: transform: translateX(0.125rem);
.translate-y-0-5: transform: translateY(0.125rem);
.translate-x-1: transform: translateX(0.25rem);
.translate-y-1: transform: translateY(0.25rem);
.translate-x-1-5: transform: translateX(0.375rem);
.translate-y-1-5: transform: translateY(0.375rem);
.translate-x-2: transform: translateX(0.5rem);
.translate-y-2: transform: translateY(0.5rem);

Percentage-based translations
.translate-x-1-2: transform: translateX(50%);
.translate-x-1-3: transform: translateX(33.333333%);
.translate-x-2-3: transform: translateX(66.666667%);
.translate-x-1-4: transform: translateX(25%);
.translate-x-2-4: transform: translateX(50%);
.translate-x-3-4: transform: translateX(75%);
.translate-x-full: transform: translateX(100%);
.translate-y-1-2: transform: translateY(50%);
.translate-y-1-3: transform: translateY(33.333333%);
.translate-y-2-3: transform: translateY(66.666667%);
.translate-y-1-4: transform: translateY(25%);
.translate-y-2-4: transform: translateY(50%);
.translate-y-3-4: transform: translateY(75%);
.translate-y-full: transform: translateY(100%);
}
</details>

<br />
Usage: Apply the class translate-{value} to control the translation along the X and Y axes.

Example Usage:

```jsx
<div class="translate-y-0"></div>
```
## Transition Animation
### Animation
Description: Applies keyframe animations to an element.
<details>
<summary>Classes:</summary>
<br />

Transition
.transition-none: transition: none;
.transition-all: transition: all 0.3s ease-in-out;
.transition-opacity: transition: opacity 0.3s ease-in-out;
.transition-transform: transition: transform 0.3s ease-in-out;
.transition-color: transition: color 0.3s ease-in-out;
.transition-bg-color: transition: background-color 0.3s ease-in-out;

Transition Delay
.transition-delay-0: transition-delay: 0s;
.transition-delay-100: transition-delay: 0.1s;
.transition-delay-200: transition-delay: 0.2s;
.transition-delay-300: transition-delay: 0.3s;
.transition-delay-400: transition-delay: 0.4s;
.transition-delay-500: transition-delay: 0.5s;

Transition Duration
.transition-duration-100: transition-duration: 0.1s;
.transition-duration-200: transition-duration: 0.2s;
.transition-duration-300: transition-duration: 0.3s;
.transition-duration-400: transition-duration: 0.4s;
.transition-duration-500: transition-duration: 0.5s;

Transition Property
.transition-property-none: transition-property: none;
.transition-property-all: transition-property: all;
.transition-property-opacity: transition-property: opacity;
.transition-property-transform: transition-property: transform;
.transition-property-color: transition-property: color;
.transition-property-bg-color: transition-property: background-color;

Transition Timing
.transition-timing-linear: transition-timing-function: linear;
.transition-timing-ease: transition-timing-function: ease;
.transition-timing-ease-in: transition-timing-function: ease-in;
.transition-timing-ease-out: transition-timing-function: ease-out;
.transition-timing-ease-in-out: transition-timing-function: ease-in-out;

</details>

<br />
Usage: Apply the class animate-{value} to control the animation.

Example Usage:

```jsx
<div class="animate-fade-out"></div>
```
### Transition Delay
Description: Sets the delay before a CSS transition effect starts.
<details>
<summary>Classes:</summary>
<br />

.delay-0: transition-delay: 0s;
.delay-75: transition-delay: 75ms;
.delay-100: transition-delay: 100ms;
.delay-150: transition-delay: 150ms;
.delay-200: transition-delay: 200ms;
.delay-300: transition-delay: 300ms;
.delay-500: transition-delay: 500ms;
.delay-700: transition-delay: 700ms;
.delay-1000: transition-delay: 1000ms;
</details>

<br />
Usage: Apply the class delay-{value} to control the transition delay.

Example Usage:

```jsx
<div class="delay-0"></div>
```
### Transition Duration
Description: Sets the duration of a CSS transition effect.
<details>
<summary>Classes:</summary>
<br />

duration-0: transition-duration: 0s;
duration-75: transition-duration: 75ms;
duration-100: transition-duration: 100ms;
duration-150: transition-duration: 150ms;
duration-200: transition-duration: 200ms;
duration-300: transition-duration: 300ms;
duration-500: transition-duration: 500ms;
duration-700: transition-duration: 700ms;
duration-1000: transition-duration: 1000ms;
</details>

<br />
Usage: Apply the class duration-{value} to control the transition duration.

Example Usage:

```jsx
<div class="duration-0"></div>
```
### Transition Property
Description: Specifies the CSS property to which a transition effect should be applied.
<details>
<summary>Classes:</summary>
<br />

.transition-none: transition-property: none;
.transition-all: transition-property: all;transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);transition-duration: 150ms;
.transition: transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, backdrop-filter;transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);transition-duration: 150ms;
.transition-colors: transition-property: color, background-color, border-color, text-decoration-color, fill, stroke;transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);transition-duration: 150ms;
.transition-opacity: transition-property: opacity;transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);transition-duration: 150ms;
.transition-shadow: transition-property: box-shadow;transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);transition-duration: 150ms;
.transition-transform: transition-property: transform;transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);transition-duration: 150ms;
</details>

<br />
Usage: Apply the class transition-{value} to control the transition property.

Example Usage:

```jsx
<div class="transition-all"></div>
```
### Transition Timing
Description: Specifies the timing function for a CSS transition effect.
<details>
<summary>Classes:</summary>
<br />

.ease-linear: transition-timing-function: linear;
.ease-in: transition-timing-function: cubic-bezier(0.4, 0, 1, 1);
.ease-out: transition-timing-function: cubic-bezier(0, 0, 0.2, 1);
.ease-in-out: transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
</details>

<br />
Usage: Apply the class ease-{value} to control the transition timing function.

Example Usage:

```jsx
<div class="ease-linear"></div>
```
## Typography
### Content
Description: Sets the content of an element generated using the ::before or ::after pseudo-elements.
<details>
<summary>Classes:</summary>
<br />

.content-none: content: none;
</details>

<br />
Usage: Apply the class content-{value} to control the content.

Example Usage:

```jsx
<p class="content-none"></p>
```
### Font
Description: Sets the font properties for an element.
<details>
<summary>Classes:</summary>
<br />

Font Family Utilities
.font-sans: font-family: ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
.font-serif: font-family: ui-serif, Georgia, Cambria, "Times New Roman", Times, serif;
.font-mono: font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;

Font Size Utilities
.text-xs: font-size: 0.75rem; /* 12px */ line-height: 1rem; /* 16px */
.text-sm: font-size: 0.875rem; /* 14px */ line-height: 1.25rem; /* 20px */
.text-base: font-size: 1rem; /* 16px */ line-height: 1.5rem; /* 24px */
.text-lg: font-size: 1.125rem; /* 18px */ line-height: 1.75rem; /* 28px */
.text-xl: font-size: 1.25rem; /* 20px */ line-height: 1.75rem; /* 28px */
.text-2xl: font-size: 1.5rem; /* 24px */ line-height: 2rem; /* 32px */
.text-3xl: font-size: 1.875rem; /* 30px */ line-height: 2.25rem; /* 36px */
.text-4xl: font-size: 2.25rem; /* 36px */ line-height: 2.5rem; /* 40px */
.text-5xl: font-size: 3rem; /* 48px */ line-height: 1;
.text-6xl: font-size: 3.75rem; /* 60px */ line-height: 1;
.text-7xl: font-size: 4.5rem; /* 72px */ line-height: 1;
.text-8xl: font-size: 6rem; /* 96px */ line-height: 1;
.text-9xl: font-size: 8rem; /* 128px */ line-height: 1;

Font Smoothing Utilities
.antialiased: -webkit-font-smoothing: antialiased; -moz-osx-font-smoothing: grayscale;
.subpixel-antialiased: -webkit-font-smoothing: auto; -moz-osx-font-smoothing: auto;

Font Style Utilities
.italic: font-style: italic;
.not-italic: font-style: normal;

Font Weight Utilities
.font-thin: font-weight: 100;
.font-extralight: font-weight: 200;
.font-light: font-weight: 300;
.font-normal: font-weight: 400;
.font-medium: font-weight: 500;
.font-semibold: font-weight: 600;
.font-bold: font-weight: 700;
.font-extrabold: font-weight: 800;
.font-black: font-weight: 900;

Font Variant Numeric Utilities
.normal-nums: font-variant-numeric: normal;
.ordinal: font-variant-numeric: ordinal;
.slashed-zero: font-variant-numeric: slashed-zero;
.lining-nums: font-variant-numeric: lining-nums;
.oldstyle-nums: font-variant-numeric: oldstyle-nums;
.proportional-nums: font-variant-numeric: proportional-nums;
.tabular-nums: font-variant-numeric: tabular-nums;
.diagonal-fractions: font-variant-numeric: diagonal-fractions;
.stacked-fractions: font-variant-numeric: stacked-fractions;
</details>

<br />
Usage: Apply the class font-{value} to control the font.

Example Usage:

```jsx
<div class="font-bold"></div>
```
### Hyphens
Description: Sets whether to allow hyphenation within words.
<details>
<summary>Classes:</summary>
<br />

.hyphens-none: hyphens: none;
.hyphens-manual: hyphens: manual;
.hyphens-auto: hyphens: auto;
</details>

<br />
Usage: Apply the class hyphens-{value} to control hyphenation.

Example Usage:

```jsx
<p class="hyphens-auto"></p>
```
### Letter Spacing
Description: Sets the spacing between characters.
<details>
<summary>Classes:</summary>
<br />

.letter-tighter: letter-spacing: -0.05em;
.letter-tight: letter-spacing: -0.025em;
.letter-normal: letter-spacing: 0em;
.letter-wide: letter-spacing: 0.025em;
.letter-wider: letter-spacing: 0.05em;
.letter-widest: letter-spacing: 0.1em;
</details>

<br />
Usage: Apply the class letter-{value} to control letter spacing.

Example Usage:

```jsx
<span class="letter-normal"></span>
```
### Line
Description: Sets the height of a line of text.
<details>
<summary>Classes:</summary>
<br />

.leading-3: line-height: 0.75rem; /* 12px */
.leading-4: line-height: 1rem; /* 16px */
.leading-5: line-height: 1.25rem; /* 20px */
.leading-6: line-height: 1.5rem; /* 24px */
.leading-7: line-height: 1.75rem; /* 28px */
.leading-8: line-height: 2rem; /* 32px */
.leading-9: line-height: 2.25rem; /* 36px */
.leading-10: line-height: 2.5rem; /* 40px */
.leading-none: line-height: 1;
.leading-tight: line-height: 1.25;
.leading-snug: line-height: 1.375;
.leading-normal: line-height: 1.5;
.leading-relaxed: line-height: 1.625;
.leading-loose: line-height: 2;/* Line Clamp */
.line-clamp-1: overflow: hidden;display: -webkit-box;-webkit-box-orient: vertical;-webkit-line-clamp: 1;
.line-clamp-2: overflow: hidden;display: -webkit-box;-webkit-box-orient: vertical;-webkit-line-clamp: 2;
.line-clamp-3: overflow: hidden;display: -webkit-box;-webkit-box-orient: vertical;-webkit-line-clamp: 3;
.line-clamp-4: overflow: hidden;display: -webkit-box;-webkit-box-orient: vertical;-webkit-line-clamp: 4;
.line-clamp-5: overflow: hidden;display: -webkit-box;-webkit-box-orient: vertical;-webkit-line-clamp: 5;
.line-clamp-6: overflow: hidden;display: -webkit-box;-webkit-box-orient: vertical;-webkit-line-clamp: 6;
.line-clamp-none: overflow: visible;display: block;-webkit-box-orient: horizontal;-webkit-line-clamp: none;
</details>

<br />
Usage: Apply the class leading-{value} to control line height.

Example Usage:

```jsx
<p class="leading-3"></p>
```
### List Style
Description: Sets the style of the list marker for list items.
<details>
<summary>Classes:</summary>
<br />

List Style Image
.list-image-none: list-style-image: none;

List Style Position
.list-inside: list-style-position: inside;
.list-outside: list-style-position: outside;

List Style Type
.list-none: list-style-type: none;
.list-disc: list-style-type: disc;
.list-decimal: list-style-type: decimal;
</details>

<br />
Usage: Apply the class list-{value} to control list style.

Example Usage:

```jsx
<ul class="list-none">
  <!-- Unordered list with no list marker -->
  <li>Item 1</li>
  <li>Item 2</li>
</ul>
```
### Text Align
Description: Sets the horizontal alignment of text.
<details>
<summary>Classes:</summary>
<br />

.text-left: text-align: left;
.text-center: text-align: center;
.text-right: text-align: right;
.text-justify: text-align: justify;
.text-start: text-align: start;
.text-end: text-align: end;
</details>

<br />
Usage: Apply the class text-{value} to control text alignment.

Example Usage:

```jsx
<div class="text-center"></div>
```
### Text Color
Description: Sets the color of text.
<details>
<summary>Classes:</summary>
<br />

.text-inherit: color: inherit;
.text-current: color: currentColor;
.text-transparent: color: transparent;
.text-black: color: rgb(0 0 0);
.text-white: color: rgb(255 255 255);
</details>

<br />
Usage: Apply the class text-{value} to control text color.

Example Usage:

```jsx
<p class="text-white"></p>
```
### Text Decoration
Description: Sets the decoration of text (underline, overline, or line-through).
<details>
<summary>Classes:</summary>
<br />

Text Decoration
.text-underline: text-decoration-line: underline;
.text-overline: text-decoration-line: overline;
.text-line-through: text-decoration-line: line-through;
.no-underline: text-decoration-line: none;

Text Decoration Color
.decoration-inherit: text-decoration-color: inherit;
.decoration-current: text-decoration-color: currentColor;
.decoration-transparent: text-decoration-color: transparent;
.decoration-black: text-decoration-color: #000;
.decoration-white: text-decoration-color: #fff;

Text Decoration Style
.decoration-solid: text-decoration-style: solid;
.decoration-double: text-decoration-style: double;
.decoration-dotted: text-decoration-style: dotted;
.decoration-dashed: text-decoration-style: dashed;
.decoration-wavy: text-decoration-style: wavy;

Text Decoration Thickness
.decoration-auto: text-decoration-thickness: auto;
.decoration-from-font: text-decoration-thickness: from-font;
.decoration-0: text-decoration-thickness: 0px;
.decoration-1: text-decoration-thickness: 1px;
.decoration-2: text-decoration-thickness: 2px;
.decoration-4: text-decoration-thickness: 4px;
.decoration-8: text-decoration-thickness: 8px;
</details>

<br />
Usage: Apply the class text-{value} and decoration-{value} to control text decoration.

Example Usage:

```jsx
<span class="text-underline"></span>
```
### Text Indent
Description: Sets the indentation of the first line in a text block.
<details>
<summary>Classes:</summary>
<br />

.indent-0: text-indent: 0px;
.indent-px: text-indent: 1px;
.indent-0-5: text-indent: 0.125rem; /* 2px */
.indent-1: text-indent: 0.25rem; /* 4px */
.indent-1-5: text-indent: 0.375rem; /* 6px */
.indent-2: text-indent: 0.5rem; /* 8px */
.indent-2-5: text-indent: 0.625rem; /* 10px */
.indent-3: text-indent: 0.75rem; /* 12px */
.indent-3-5: text-indent: 0.875rem; /* 14px */
.indent-4: text-indent: 1rem; /* 16px */
.indent-5: text-indent: 1.25rem; /* 20px */
.indent-6: text-indent: 1.5rem; /* 24px */
.indent-7: text-indent: 1.75rem; /* 28px */
.indent-8: text-indent: 2rem; /* 32px */
.indent-9: text-indent: 2.25rem; /* 36px */
.indent-10: text-indent: 2.5rem; /* 40px */
.indent-11: text-indent: 2.75rem; /* 44px */
.indent-12: text-indent: 3rem; /* 48px */
.indent-14: text-indent: 3.5rem; /* 56px */
.indent-16: text-indent: 4rem; /* 64px */
.indent-20: text-indent: 5rem; /* 80px */
.indent-24: text-indent: 6rem; /* 96px */
.indent-28: text-indent: 7rem; /* 112px */
.indent-32: text-indent: 8rem; /* 128px */
.indent-36: text-indent: 9rem; /* 144px */
.indent-40: text-indent: 10rem; /* 160px */
.indent-44: text-indent: 11rem; /* 176px */
.indent-48: text-indent: 12rem; /* 192px */
.indent-52: text-indent: 13rem; /* 208px */
.indent-56: text-indent: 14rem; /* 224px */
.indent-60: text-indent: 15rem; /* 240px */
.indent-64: text-indent: 16rem; /* 256px */
.indent-72: text-indent: 18rem; /* 288px */
.indent-80: text-indent: 20rem; /* 320px */
.indent-96: text-indent: 24rem; /* 384px */
</details>

<br />
Usage: Apply the class indent-{value} to control text indentation.

Example Usage:

```jsx
<p class="indent-10"></p>
```
### Text Overflow
Description: Sets what should happen when text overflows the containing element.
<details>
<summary>Classes:</summary>
<br />

.truncate: overflow: hidden; text-overflow: ellipsis; white-space: nowrap;
.text-ellipsis: text-overflow: ellipsis;
.text-clip: text-overflow: clip;
</details>

<br />
Usage: Apply the class text-{value} and truncate to control text overflow.

Example Usage:

```jsx
<div class="text-ellipsis"></div>
```
### Text Transform
Description: Sets the capitalization of text.
<details>
<summary>Classes:</summary>
<br />

.uppercase: text-transform: uppercase;
.lowercase: text-transform: lowercase;
.capitalize: text-transform: capitalize;
.normal-case: text-transform: none;
</details>

<br />
Usage: Apply the class above to control text capitalization.

Example Usage:

```jsx
<span class="uppercase"></span>
```
### Vertical Align
Description: Sets the vertical alignment of an inline or table-cell element.
<details>
<summary>Classes:</summary>
<br />

.align-baseline: vertical-align: baseline;
.align-top: vertical-align: top;
.align-middle: vertical-align: middle;
.align-bottom: vertical-align: bottom;
.align-text-top: vertical-align: text-top;
.align-text-bottom: vertical-align: text-bottom;
.align-sub: vertical-align: sub;
.align-super: vertical-align: super;
</details>

<br />
Usage: Apply the class align-{value} to control vertical alignment.

Example Usage:

```jsx
<img class="align-baseline" src="image.jpg" alt="Center-aligned image">
```
### Whitespace
Description: Sets how white space inside an element is handled.
<details>
<summary>Classes:</summary>
<br />

.whitespace-normal: white-space: normal;
.whitespace-nowrap: white-space: nowrap;
.whitespace-pre: white-space: pre;
.whitespace-pre-line: white-space: pre-line;
.whitespace-pre-wrap: white-space: pre-wrap;
.whitespace-break-spaces: white-space: break-spaces;
</details>

<br />
Usage: Apply the class whitespace-{value} to control whitespace handling.

Example Usage:

```jsx
<div class="whitespace-nowrap"></div>
```
### Wordbreak
Description: Specifies how words should break when reaching the end of a line.
<details>
<summary>Classes:</summary>
<br />

.break-normal: overflow-wrap: normal;word-break: normal;
.break-words: overflow-wrap: break-word;
.break-all: word-break: break-all;
.break-keep: word-break: keep-all;
</details>

<br />
Usage: Apply the class break-{value} to control word breaking.

Example Usage:

```jsx
<p class="break-all"></p>
```
## Contributing

Contributions are always welcome!

See `contributing.md` for ways to get started.


## License
This project is licensed under the [MIT License](LICENSE).

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
Copyright (c) 2023 stylarcss


