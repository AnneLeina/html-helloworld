# HTML Hello World — Full Documentation

---

## 1. Title & Objective

**Project Title:** HTML Hello World

**Technology Chosen:** HTML5 (HyperText Markup Language)

**Objective:**
Build and understand the simplest possible webpage — one that displays "Hello, World!" in a browser — while learning the foundational structure of HTML, how a browser reads it, and how to style it with CSS.

**Why I Chose It:**
HTML is the backbone of every website on the internet. Before learning JavaScript, React, or any framework, you must understand HTML. It requires zero installation, runs instantly in any browser, and the feedback loop (edit → save → refresh) is immediate. It is the perfect starting point.

**End Goal:**
By the end of this project I can:
- Explain what HTML is and how it works
- Write a valid HTML5 document from scratch
- Open a local HTML file in a browser
- Add basic CSS styling inside the same file
- Identify and fix common beginner errors

---

## 2. Technology Overview

### What Is HTML?

HTML (HyperText Markup Language) is the standard language used to create and structure content on the web. It uses **tags** (angle-bracket elements like `<h1>`, `<p>`, `<div>`) to describe the meaning and structure of content — headings, paragraphs, images, links, forms, and more.

HTML is **not** a programming language; it has no logic or loops. It is a **markup language** — it annotates content so browsers know how to display it.

### Where Is It Used?

- Every website and web application in existence has HTML at its core
- Email templates
- Progressive Web Apps (PWAs)
- Browser-based games
- Documentation sites (like MDN, GitHub Pages)

### One Real-World Example

**Wikipedia (wikipedia.org)** — every article page is an HTML document. The heading of the article is an `<h1>` tag, sections are `<h2>` tags, body text is `<p>` tags, and images use `<img>` tags. The browser reads the HTML and renders the formatted page you see.

---

## 3. System Requirements

| Requirement | Detail |
|-------------|--------|
| **Operating System** | Windows 10 or Windows 11 |
| **Browser** | Google Chrome, Microsoft Edge, or Mozilla Firefox (any modern browser) |
| **Text Editor** | Visual Studio Code (recommended) — free download at https://code.visualstudio.com |
| **Terminal / Command Prompt** | Not required for this project |
| **Packages / Frameworks** | None — plain HTML requires no installation |
| **Internet Connection** | Not required to run the file locally |

---

## 4. Installation & Setup Instructions (Step by Step)

### Step 1 — Install Visual Studio Code

1. Go to https://code.visualstudio.com
2. Click **Download for Windows**
3. Run the installer (`.exe` file) and follow the prompts
4. Accept the default options; tick **"Add to PATH"** if prompted
5. Launch VS Code once installation is complete

### Step 2 — Install the Live Server Extension (Optional but Recommended)

Live Server auto-refreshes the browser every time you save a file.

1. Open VS Code
2. Click the **Extensions** icon in the left sidebar (or press `Ctrl + Shift + X`)
3. Search for **"Live Server"** by Ritwick Dey
4. Click **Install**

### Step 3 — Create Your Project Folder

1. Create a new folder anywhere on your computer, e.g. `C:\Projects\hello-world\`
2. Open VS Code
3. Click **File → Open Folder** and select your new folder

### Step 4 — Create the HTML File

1. In VS Code, click **New File** (the icon next to the folder name in the sidebar)
2. Name it `index.html` — the `.html` extension is required
3. Type `!` and press `Tab` — VS Code auto-generates the HTML boilerplate (Emmet shortcut)

### Step 5 — Run the File

**Option A — Open directly:**
1. Open File Explorer and navigate to your folder
2. Double-click `index.html` — it opens in your default browser

**Option B — Use Live Server:**
1. With `index.html` open in VS Code
2. Right-click anywhere in the file
3. Select **"Open with Live Server"**
4. Your browser opens at `http://127.0.0.1:5500/index.html` and auto-refreshes on save

---

## 5. Minimal Working Example

### What This Example Does

The example file (`index.html`) creates a single webpage that:
1. Shows a centred white card on a light blue-grey background
2. Displays the heading **"Hello, World! 👋"**
3. Shows a short welcome paragraph below it
4. Adds a small blue badge label at the bottom of the card

All HTML structure and CSS styling live in one single file — no external stylesheets or scripts are needed.

### Code (index.html) with Inline Comments

```html
<!DOCTYPE html>
<!-- DOCTYPE declaration: tells the browser this is an HTML5 document -->

<html lang="en">
<!-- <html> is the root element; lang="en" sets the language to English -->

<head>
  <!-- <head> holds metadata — nothing here is visible on the page -->
  <meta charset="UTF-8" />
  <!-- UTF-8 supports all characters, including emoji and accented letters -->

  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <!-- Makes the page scale correctly on phones and tablets -->

  <title>Hello World – HTML Project</title>
  <!-- Text that appears on the browser tab -->

  <style>
    /* CSS lives inside <style> tags in the <head> */

    body {
      font-family: Arial, sans-serif;
      background-color: #f0f4f8;   /* Light grey-blue page background */
      display: flex;
      justify-content: center;     /* Centre horizontally */
      align-items: center;         /* Centre vertically */
      height: 100vh;               /* 100% of the viewport height */
      margin: 0;                   /* Remove default browser margin */
    }

    .card {
      background: #ffffff;         /* White card */
      border-radius: 12px;         /* Rounded corners */
      padding: 48px 64px;
      text-align: center;
      box-shadow: 0 4px 20px rgba(0,0,0,0.1); /* Soft shadow */
    }

    h1 { color: #2c3e50; font-size: 2.5rem; margin-bottom: 8px; }
    p  { color: #555; font-size: 1rem; }

    .badge {
      display: inline-block;
      margin-top: 20px;
      background: #3498db;         /* Blue */
      color: #fff;
      padding: 6px 16px;
      border-radius: 20px;
      font-size: 0.85rem;
    }
  </style>
</head>

<body>
  <!-- Everything inside <body> is rendered in the browser window -->

  <div class="card">
    <!-- <div> is a generic block container -->

    <h1>Hello, World! 👋</h1>
    <!-- <h1> is the top-level heading — only one per page is best practice -->

    <p>Welcome to my first HTML project.</p>
    <!-- <p> is a paragraph -->

    <span class="badge">HTML5 · Beginner Project</span>
    <!-- <span> is an inline container; class="badge" applies the .badge CSS -->
  </div>

</body>
</html>
```

### Expected Output

When you open the file in a browser you will see:

```
┌─────────────────────────────────────┐
│                                     │
│         Hello, World! 👋            │
│   Welcome to my first HTML project. │
│                                     │
│     [ HTML5 · Beginner Project ]    │
│                                     │
└─────────────────────────────────────┘
```

A white rounded card, centred on a pale background, with dark heading text, grey paragraph text, and a blue badge.

---

## 6. AI Prompt Journal

The prompts below were used during this project. Each is linked to the concept it helped clarify.

---

### Prompt 1

**Prompt used:**
> "Give me a step-by-step guide to initialize Hello World in HTML."

**Curriculum link / concept:** Project initialisation — creating the first HTML file, understanding the boilerplate structure, and opening it in a browser.

**What the AI explained:**
- Create a file named `index.html`
- Add `<!DOCTYPE html>` at the very top
- Wrap all content in `<html>`, `<head>`, and `<body>` tags
- Put a heading inside `<body>` using `<h1>Hello, World!</h1>`
- Open the file in a browser by double-clicking it

**What I learned:** The order of tags matters. The browser expects `<!DOCTYPE html>` first, then `<html>`, and the content must be inside `<body>` — not `<head>`.

---

### Prompt 2

**Prompt used:**
> "What is the difference between <head> and <body> in HTML?"

**Curriculum link / concept:** HTML document structure — understanding metadata vs visible content.

**What the AI explained:**
- `<head>` holds metadata: page title, character encoding, links to CSS/JS, SEO description. Nothing in `<head>` appears on the page.
- `<body>` holds everything the user sees: headings, text, images, buttons.

**What I learned:** Putting a `<style>` tag inside `<body>` still works in most browsers, but it is invalid HTML. Always put `<style>` in `<head>`.

---

### Prompt 3

**Prompt used:**
> "How do I centre content on a webpage using CSS flexbox?"

**Curriculum link / concept:** CSS layout — using `display: flex` with `justify-content` and `align-items` to centre an element both horizontally and vertically.

**What the AI explained:**
Apply these three rules to the parent container (`body` in this case):
```css
display: flex;
justify-content: center;
align-items: center;
height: 100vh;
```

**What I learned:** Without `height: 100vh` on the body, vertical centring with flexbox does not work because the body has no height by default.

---

### Prompt 4

**Prompt used:**
> "What does <!DOCTYPE html> do and why is it needed?"

**Curriculum link / concept:** HTML5 standards mode — the DOCTYPE declaration.

**What the AI explained:**
`<!DOCTYPE html>` is not an HTML tag; it is an instruction to the browser. It tells the browser to render the page in **standards mode** (modern HTML5 rules). Without it, some browsers fall back to **quirks mode**, which emulates old browser bugs and can cause layouts to look wrong.

**What I learned:** Always include `<!DOCTYPE html>` as the very first line — even before `<html>`.

---

## 7. Common Issues & Fixes

### Issue 1 — The page is blank / nothing shows

**What went wrong:** The content was accidentally placed inside `<head>` instead of `<body>`.

**Error symptom:** Browser tab shows the title correctly but the page is completely blank.

**Fix:**
Move your visible content tags (`<h1>`, `<p>`, `<div>`) into the `<body>` section.

```html
<!-- ❌ Wrong -->
<head>
  <h1>Hello, World!</h1>
</head>

<!-- ✅ Correct -->
<body>
  <h1>Hello, World!</h1>
</body>
```

**Reference:** https://stackoverflow.com/questions/3940840/html-content-in-head-vs-body

---

### Issue 2 — Styles are not applying / page looks unstyled

**What went wrong:** The `<style>` tag was placed inside `<body>`, or CSS property names were misspelled.

**Error symptom:** The text appears with no formatting — default browser font, no colours, no layout.

**Fix:**
Move `<style>` into `<head>`. Also check for typos like `colour` instead of `color` (CSS uses American English).

```html
<!-- ❌ Wrong -->
<body>
  <style> h1 { colour: red; } </style>

<!-- ✅ Correct -->
<head>
  <style> h1 { color: red; } </style>
```

**Reference:** https://stackoverflow.com/questions/2830296/using-style-tags-in-the-body-with-other-elements

---

### Issue 3 — File opens as text, not a webpage

**What went wrong:** The file was saved with the wrong extension (e.g. `index.html.txt`).

**Error symptom:** Double-clicking the file opens Notepad showing raw HTML code instead of the rendered page.

**Fix:**
1. In File Explorer, enable **"File name extensions"** under the View menu
2. Rename the file and ensure it ends in `.html` only (not `.html.txt`)
3. In VS Code, check the bottom-right corner shows "HTML" as the language mode

**Reference:** https://stackoverflow.com/questions/18840760/html-file-opens-in-notepad-instead-of-browser

---

### Issue 4 — Emoji or special characters show as boxes / question marks

**What went wrong:** The `<meta charset="UTF-8">` line was missing from `<head>`.

**Error symptom:** Emoji (👋) or accented characters (é, ñ) appear as `?` or `□`.

**Fix:**
Add the charset meta tag as the **first** element inside `<head>`:

```html
<head>
  <meta charset="UTF-8" />
  ...
</head>
```

**Reference:** https://stackoverflow.com/questions/18447970/utf-8-in-html-and-css

---

### Issue 5 — Vertical centring with flexbox is not working

**What went wrong:** `height: 100vh` was missing from the `body` CSS rule.

**Error symptom:** Content is centred horizontally but sits at the top of the page.

**Fix:**
Add `height: 100vh` (and optionally `margin: 0` to remove the default body margin) to the `body` selector:

```css
body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;  /* ← this line is required */
  margin: 0;
}
```

**Reference:** https://stackoverflow.com/questions/8865458/how-to-vertically-center-a-div-for-all-browsers

---

## 8. Reference Resources

### Official Documentation

| Resource | URL |
|----------|-----|
| MDN Web Docs — HTML basics | https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics |
| MDN — HTML elements reference | https://developer.mozilla.org/en-US/docs/Web/HTML/Element |
| MDN — CSS basics | https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics |
| MDN — Flexbox guide | https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox |
| W3C HTML5 Specification | https://html.spec.whatwg.org/multipage/ |
| W3Schools HTML Tutorial | https://www.w3schools.com/html/ |
| VS Code Download | https://code.visualstudio.com |

---

## 9. My Learning Reflections

**What surprised me:**
I expected HTML to be complicated. What surprised me was how immediately visual the feedback is — I saved the file, refreshed the browser, and could see the change instantly. That fast loop made learning very satisfying.

**What was hard:**
Understanding the difference between `<head>` and `<body>` took a moment. I kept putting my `<style>` tags in the wrong place at first. Reading about standards mode vs quirks mode also took a second read before it clicked.

**What I would do differently:**
I would set up Live Server (the VS Code extension) from the very beginning. Opening and re-opening the file manually was slower and I occasionally forgot to save before checking the browser.

**What I want to learn next:**
- Linking an external CSS file instead of using `<style>` in `<head>`
- Adding an image with `<img>`
- Creating a navigation bar with `<nav>` and `<a>` (anchor/link) tags
- Basic JavaScript to make the heading change colour when clicked

---

*Documentation written as part of a self-directed HTML learning project.*
