# HTML Self-Study Lab: Build Your First Web Pages

**Duration:** 2 hours · **Level:** Complete beginner · **Tools:** A text editor and a web browser

Welcome! In this lab, you will learn HTML by making small changes and seeing what happens in your browser.

- **First 90 minutes:** Follow the guided tasks to build **My Learning Hub**.
- **Last 30 minutes:** Work independently to build a **Student Club Open Day** page.
- **After the lab:** Use the extra reference and practice ideas to continue learning.

> **What does “learn HTML” mean here?** HTML is a large topic. Two hours is enough to practise its main building blocks and make a complete basic page. It is not enough to master every element, attribute, accessibility rule, or browser feature. This lab covers the essential skills, then gives you a clear route to the remaining topics.

## Contents

- [Before you begin](#before-you-begin)
- [Your two-hour plan](#your-two-hour-plan)
- [Task 1 — Create your first page](#task-1--create-your-first-page)
- [Task 2 — Add readable text](#task-2--add-readable-text)
- [Task 3 — Make lists](#task-3--make-lists)
- [Task 4 — Add links and an image](#task-4--add-links-and-an-image)
- [Task 5 — Give your page a clear structure](#task-5--give-your-page-a-clear-structure)
- [Task 6 — Build a timetable](#task-6--build-a-timetable)
- [Task 7 — Create a form](#task-7--create-a-form)
- [Task 8 — Add media and a question box](#task-8--add-media-and-a-question-box)
- [Task 9 — Check and repair](#task-9--check-and-repair)
- [Final task — Student Club Open Day](#final-task--student-club-open-day)
- [HTML quick reference](#html-quick-reference)
- [Common problems and easy fixes](#common-problems-and-easy-fixes)
- [Continue learning after the lab](#continue-learning-after-the-lab)

## Before you begin

### What you need

- A computer with a browser, such as Chrome, Firefox, or Edge.
- A plain-text editor, such as VS Code or Notepad. Do not use Word.
- One small JPG or PNG image. Use your own photo or drawing; any suitable image is fine.
- Internet access for the external links, optional media playback, and online HTML checker.

**Before the session:** Have the editor ready and the image available. If you have no image, make a simple drawing in Paint or another drawing app and save it as a PNG. You do not need to install any extensions.

**No internet?** You can still do the main tasks using local files. Skip external-link and media-playback checks, and use the manual checklist instead of the online checker.

### What you will learn

By the end, you should be able to:

- Create and open an HTML document.
- Explain tags, elements, attributes, and nesting.
- Add headings, paragraphs, text emphasis, lists, links, and images.
- Organise a page with meaningful HTML elements.
- Create a table and a labelled form.
- Use browser form validation and a disclosure box.
- Recognise how audio and video are added.
- Check basic accessibility and fix common HTML mistakes.

### How to use this lab

For each task: **read → type → save → refresh → change → check**.

1. Read the short explanation.
2. Type the example into your HTML file. Copying is fine if typing slows you down, but read each line.
3. Save the file using **Ctrl+S** or **Cmd+S**.
4. Refresh the browser to see your changes.
5. Complete the **Your turn** activity yourself.
6. Complete the checkpoint before moving on.

> The code blocks in this README are examples. Put the HTML code in your `.html` file. Do not copy the triple backticks. This README is the instruction sheet, not the website.

## Task 1 — Create your first page

**Time: 8 minutes · File: `index.html`**

### Learn

**HTML** means **HyperText Markup Language**. It describes the content and structure of a web page.

| Technology | Its job | Simple example |
| --- | --- | --- |
| HTML | Content and structure | A heading and a form |
| CSS | Presentation and layout | Colours and spacing |
| JavaScript | Programmed behaviour | Calculate a total when a button is clicked |

Today, use HTML only. A plain-looking page is expected.

### Follow these steps

1. Create a folder called `html-lab`.
2. Inside it, create a folder called `images`.
3. Copy your image into `images`. Give it a simple name, such as `club.jpg` or `club.png`. Keep its real file extension.
4. Create a file called `index.html` directly inside `html-lab`.
5. Type this complete document into `index.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Learning Hub</title>
</head>
<body>
  <h1>Welcome to My Learning Hub</h1>
  <p>I am learning how to create a web page.</p>
</body>
</html>
```

6. Save the file. In Notepad, choose **All files** when saving so that it is not saved as `index.html.txt`.
7. Open the saved file with your browser. Double-click it, or use **Open with** and choose your browser.

### Understand the code

| Code | Simple meaning |
| --- | --- |
| `<!DOCTYPE html>` | Tells the browser to use standards mode for modern HTML. |
| `<html lang="en">` | The root element; the page language is English. |
| `<head>` | Information about the document. |
| `<meta charset="UTF-8">` | Sets the text encoding so characters can be interpreted correctly. |
| The viewport `<meta>` line | Helps mobile browsers use the device width; responsive layout still needs suitable content and usually CSS. |
| `<title>` | The name shown in the browser tab. |
| `<body>` | The page content. |
| `<h1>` | The main heading. |
| `<p>` | A paragraph. |

In `<p>Hello!</p>`, `<p>` is the opening tag, `Hello!` is the content, and `</p>` is the closing tag. Together, they form an **element**.

In `<html lang="en">`, `lang` is an **attribute** and `en` is its value. Attributes add information to an element. Put them in the opening tag.

### Your turn

Change the paragraph to include your first name. Change the tab title to `Learning HTML with YOUR NAME`.

### Checkpoint

- [ ] I can see my heading and paragraph in the browser.
- [ ] The browser tab has my new title.
- [ ] I know that changing the file requires saving and refreshing.

## Task 2 — Add readable text

**Time: 10 minutes · Keep working in `index.html`.**

### Learn

Headings organise content. Use `<h1>` for this page's main heading, `<h2>` for its main sections, and `<h3>` for subsections. Heading levels continue to `<h6>`. Choose a level for its meaning, not its text size.

### Try it

Add this code **after your existing paragraph, inside `<body>`**:

```html
<h2 id="about">About my learning</h2>
<p>I want to build <strong>useful websites</strong>.</p>
<p>I will practise <em>a little every day</em>.</p>
<p>Today's topic is <mark>HTML</mark>.</p>

<h3>A small science note</h3>
<p>Water is H<sub>2</sub>O. The square of x is x<sup>2</sup>.</p>

<h3>My study place</h3>
<p>Computer Lab<br>First Floor</p>

<hr>
<p>I can display a tag as text: &lt;p&gt;.</p>
<p>Learning &amp; practice work well together.</p>

<!-- This note is for someone reading the source code. -->
```

| Element or code | Purpose |
| --- | --- |
| `<strong>` | Strong importance; usually shown in bold. |
| `<em>` | Emphasis; usually shown in italics. |
| `<mark>` | Highlights relevant text. |
| `<sub>`, `<sup>` | Subscript and superscript. |
| `<br>` | A meaningful line break, such as in an address. |
| `<hr>` | A change of topic or thematic break. |
| `&lt;`, `&gt;`, `&amp;` | Display `<`, `>`, and `&`. These are character references. |
| `<!-- ... -->` | A comment: not displayed as page content, but visible in source code. |

`<br>`, `<hr>`, `<meta>`, `<img>`, and `<input>` are **void elements**. They do not have closing tags. Do not write `</img>` or `</input>`.

**Nesting** means placing an element inside another element. Close the inner element first:

```html
<p>I <strong>enjoy learning</strong> HTML.</p>
```

Do not put a heading or a whole section inside a paragraph. Use separate elements.

### Your turn

1. Add a new paragraph about your favourite subject.
2. Emphasise one important phrase using `<strong>` or `<em>`.
3. Add a comment containing `Task 2 completed`.
4. Put several spaces between two words in your source, then refresh. Notice that ordinary HTML text normally collapses repeated spaces.

> Use paragraphs for separate ideas. Do not use repeated `<br>` tags or spaces to design a layout; that is a CSS job.

### Checkpoint

- [ ] My headings have a sensible order.
- [ ] The science note shows a lowered 2 and a raised 2.
- [ ] My comment is not shown on the page.

## Task 3 — Make lists

**Time: 8 minutes**

### Learn

- `<ul>` makes an unordered list, usually shown with bullets.
- `<ol>` makes an ordered list, usually shown with numbers.
- `<li>` is one item in either kind of list.
- `<dl>`, `<dt>`, and `<dd>` make a description list: terms and their descriptions.

### Try it

Add this **before `</body>`**:

```html
<h2>My learning plan</h2>

<h3>Things I need</h3>
<ul>
  <li>A computer</li>
  <li>A text editor</li>
  <li>A web browser</li>
</ul>

<h3>My practice routine</h3>
<ol>
  <li>Read the task.</li>
  <li>Write the code.</li>
  <li>Save and check the page.</li>
</ol>

<h3>A new word</h3>
<dl>
  <dt>Browser</dt>
  <dd>An application used to open and display web pages.</dd>
</dl>
```

### Your turn

1. Add a fourth item to your equipment list.
2. Add `Fix any mistakes.` as the final step in your routine.
3. Add `HTML` and its meaning to the description list, using another `<dt>` and `<dd>` pair.

### Checkpoint

- [ ] The equipment list has bullets.
- [ ] The routine has numbers.
- [ ] My description list contains two terms and two explanations.

## Task 4 — Add links and an image

**Time: 10 minutes**

### Learn

A link uses `<a>` and an `href` destination. An image uses `<img>`, a `src` file location, and an `alt` text alternative.

### Try it

Add this **before `</body>`**. If your image is a PNG, change the filename to match.

```html
<h2>Useful places</h2>
<p><a href="https://developer.mozilla.org/en-US/docs/Web/HTML">Read the MDN HTML guide</a></p>
<p><a href="#about">Back to About my learning</a></p>
<p><a href="mailto:learning@example.com">Email the learning club</a></p>

<figure>
  <img src="images/club.jpg" alt="A drawing of a computer used for learning" width="300">
  <figcaption>A picture for my learning page.</figcaption>
</figure>
```

**Change the `alt` text to describe your actual image.** A useful alternative explains what the image contributes. A purely decorative image can use `alt=""`.

`<figure>` groups self-contained content, such as a picture, with its optional `<figcaption>` caption.

| Example | Meaning |
| --- | --- |
| `https://developer.mozilla.org/...` | An absolute URL to an external website. |
| `images/club.jpg` | A relative path: open `images`, then find `club.jpg`. |
| `#about` | Go to the element whose `id` is `about` on this page. |
| `mailto:learning@example.com` | Ask the device to open an email application; it does not send an email automatically. |

### Your turn

1. Change the caption to suit your image.
2. Click the internal link. It should jump to the About heading; on a short page, the movement may be small.
3. Create a second file called `hello.html` beside `index.html`. Copy the Task 1 document structure into it, then change its title and heading to `Hello from page two`.
4. In `index.html`, add `<p><a href="hello.html">Visit my second page</a></p>` before `</body>`.
5. In the body of `hello.html`, add `<p><a href="index.html">Return to my learning hub</a></p>`. Test both links.

> Every `id` must be unique within one page. Use descriptive link text; “Read the HTML guide” is more helpful than “Click here”.

### Checkpoint

- [ ] My image displays, with a caption.
- [ ] Its filename, extension, and letter case match the actual file.
- [ ] I can move between my two local pages.

## Task 5 — Give your page a clear structure

**Time: 10 minutes**

### Learn

**Semantic HTML** uses elements that explain the purpose of content.

| Element | Use it for |
| --- | --- |
| `<header>` | Introductory content, such as a page heading. |
| `<nav>` | A group of major navigation links. |
| `<main>` | The page's main content; use one visible main area here. |
| `<section>` | A related group of content, normally with a heading. |
| `<article>` | A self-contained item, such as a news post. |
| `<aside>` | Related but secondary content. |
| `<footer>` | Closing information, such as contact or copyright details. |

### Try it

You will now organise your existing work. **Keep the `<!DOCTYPE html>`, `<html>`, and `<head>` from Task 1. Reorganise only the content inside `<body>`.**

1. Move your existing `<h1>` into the `<header>` below.
2. Move **all the other content currently in your body** into the first `<section>`, where the comment says to put it. This includes your first paragraph, About heading, lists, links, and figure.
3. Keep `id="about"` on the existing About heading. Do not create a second element with that same ID.
4. Add the navigation and footer shown below.

```html
<body>
  <header>
    <h1>Welcome to My Learning Hub</h1>
    <nav aria-label="Main navigation">
      <a href="#about">About</a>
      <a href="#schedule">Schedule</a>
      <a href="#join">Join</a>
    </nav>
  </header>

  <main>
    <section>
      <!-- Move your existing body content here, except the h1. -->
    </section>
    <!-- New sections from the next tasks go here. -->
  </main>

  <footer>
    <p><small>&copy; 2026 My Learning Hub</small></p>
  </footer>
</body>
```

The comments are placement instructions. Do not leave your previous work out! There must be only one `<body>` in the finished file.

The Schedule and Join links will work after you create their target sections in Tasks 6 and 7. `aria-label` gives the navigation region an accessible name. Native HTML already supplies much accessibility information, so do not add ARIA attributes everywhere.

`<small>` marks small-print information. `&copy;` displays ©.

### Your turn

Change the footer to include your name. Then use the keyboard's **Tab** key to move through the links, and **Enter** to activate one.

### Checkpoint

- [ ] My previous text, lists, and image are still visible.
- [ ] My document contains one header, one main area, and one footer.
- [ ] I can reach links using the keyboard.

## Task 6 — Build a timetable

**Time: 10 minutes**

### Learn

Use a table for data with rows and columns. Do not use tables to position an entire page.

### Try it

Insert this new section **inside `<main>`, after your first section and before `</main>`**:

```html
<section id="schedule">
  <h2>My weekly study timetable</h2>
  <table>
    <caption>Two short practice sessions</caption>
    <thead>
      <tr>
        <th scope="col">Day</th>
        <th scope="col">Topic</th>
        <th scope="col">Minutes</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="row">Monday</th>
        <td>Headings and paragraphs</td>
        <td>20</td>
      </tr>
      <tr>
        <th scope="row">Wednesday</th>
        <td>Links and images</td>
        <td>30</td>
      </tr>
    </tbody>
  </table>
</section>
```

| Element or attribute | Meaning |
| --- | --- |
| `<table>` | The whole table. |
| `<caption>` | The table's title or description. |
| `<thead>`, `<tbody>` | Groups of heading rows and body rows. |
| `<tr>` | One row. |
| `<th>` | A header cell. |
| `<td>` | A data cell. |
| `scope="col"` / `scope="row"` | Identifies whether the header describes a column or a row. |

The table may have no visible borders. That is normal. Borders belong in CSS; do not add the old `border` attribute for this lab.

### Your turn

1. Add a Friday row for `Forms`, lasting `25` minutes.
2. Update the caption to describe three sessions.
3. Click the Schedule navigation link.

### Checkpoint

- [ ] My table has three columns and three data rows.
- [ ] Column headings use `<th>`.
- [ ] The Schedule link reaches the table section.

## Task 7 — Create a form

**Time: 17 minutes**

### Learn

A form lets a person enter information. HTML creates the controls and can ask the browser to check simple rules. A server or another service is needed to receive and store submissions.

In this lab, the form is a **local demonstration**. It does not register anyone, store data, or send an email. Use made-up details.

### Try it

Insert this section **inside `<main>`, after the schedule section**:

```html
<section id="join">
  <h2>Join my learning club</h2>
  <p>Practice form only. Please use made-up details.</p>

  <form action="#join" method="get">
    <p>
      <label for="full-name">Full name (required)</label>
      <input type="text" id="full-name" name="fullName" required>
    </p>
    <p>
      <label for="email">Email (required)</label>
      <input type="email" id="email" name="email" required>
    </p>
    <p>
      <label for="minutes">Daily practice minutes</label>
      <input type="number" id="minutes" name="minutes" min="10" max="120" value="20">
    </p>

    <fieldset>
      <legend>Preferred session</legend>
      <input type="radio" id="morning" name="session" value="morning" checked>
      <label for="morning">Morning</label>
      <input type="radio" id="evening" name="session" value="evening">
      <label for="evening">Evening</label>
    </fieldset>

    <p>
      <label for="topic">Topic to practise</label>
      <select id="topic" name="topic">
        <option value="text">Text and headings</option>
        <option value="images">Links and images</option>
        <option value="forms">Forms</option>
      </select>
    </p>
    <p>
      <label for="message">My learning goal</label>
      <textarea id="message" name="message" rows="3" cols="30"></textarea>
    </p>
    <p>
      <input type="checkbox" id="reminders" name="reminders" value="yes">
      <label for="reminders">I would like practice reminders</label>
    </p>
    <button type="submit">Try submitting</button>
  </form>
</section>
```

### Understand the important parts

| Part | Why it matters |
| --- | --- |
| `<label for="email">` and `id="email"` | Matching values connect the label to its control. Clicking the label focuses that control. |
| `name="email"` | The key used when submitting that control's value. A normal input without a name is not included in the submitted name/value pairs. |
| `type="email"` | Enables a basic email-format check; it cannot prove that an address exists. |
| `required` | The browser asks for a value before a normal submission. |
| `min`, `max` | Limit the valid number range. |
| `value` | An initial text/number value, or the submitted value of a selected radio/checkbox. |
| Radio buttons with the same `name` | Form a group in which one option can be selected. |
| Checkbox | Can be switched on or off independently. An unchecked checkbox is normally omitted from submission. |
| `<fieldset>` and `<legend>` | Group related controls and give the group a label. |
| `<select>` and `<option>` | A drop-down choice. |
| `<textarea>` | A multi-line text box. |
| `<button type="submit">` | Attempts to submit the form. |
| `action="#join"` | Targets this same document and its Join section; it is not a registration service. |
| `method="get"` | Places submitted values in the URL query. Do not use it for passwords or private data. |

`required`, `checked`, and `disabled` are examples of **boolean attributes**. Their presence means true. For example, `required="false"` still makes a control required; remove the attribute to turn it off.

For a real form, a suitable server endpoint must process the submission. `method="post"` sends form data in the request body, but does not itself encrypt it. Real systems need HTTPS and server-side validation too.

### Your turn: test before changing

1. Leave the required fields empty and click **Try submitting**. The browser should ask for a value.
2. Enter `abc` in the email field and try again. It should fail the email-format check.
3. Enter `5` in daily practice minutes. It should fail the minimum-value check when you submit.
4. Use `Test Student`, `student@example.com`, and `20`. Submit again. The page may navigate or reload and show the submitted values in the URL. There is no saved registration or success message.
5. Select Morning, then Evening. Only one should stay selected.
6. Add a new drop-down option for `Tables`.

> Browser error messages differ. A valid form means the browser accepted its rules, not that any information was saved. A placeholder is only a hint and must not replace a visible label.

### Checkpoint

- [ ] Every control has a visible, connected label.
- [ ] Empty required fields and invalid values are rejected.
- [ ] I understand the different jobs of `id` and `name`.

## Task 8 — Add media and a question box

**Time: 10 minutes**

### Learn

HTML can show audio and video controls. It also has a built-in expandable question box that works without JavaScript.

### Try it: an expandable answer

Add this section **inside `<main>`, after the Join section**:

```html
<section id="resources">
  <h2>Learning resources</h2>
  <details>
    <summary>Do I need CSS to write HTML?</summary>
    <p>No. HTML gives the page its structure. CSS changes its presentation.</p>
  </details>
</section>
```

Click the question to open and close it. Try focusing it with **Tab**, then pressing **Enter** or **Space**.

### Try it: audio and video

Add the following code **inside the resources section, after `</details>`**. These public sample files need internet access; playback also depends on browser support and source availability.

```html
<h3>A sample sound</h3>
<audio controls preload="none">
  <source src="https://interactive-examples.mdn.mozilla.net/media/cc0-audio/t-rex-roar.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>
<p>Sound description: a loud dinosaur roar.</p>

<h3>A sample video</h3>
<video controls width="300" preload="none">
  <source src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4" type="video/mp4">
  Your browser does not support the video element.
</video>
<p>Video description: a close-up view of a flower.</p>
```

- `controls` asks the browser to display playback controls.
- `<source>` gives a media location and format. It is a void element.
- Multiple sources can provide alternative formats.
- The fallback sentences above help browsers that do not support the media elements. They are not reliable missing-file error messages.
- For local media, use a path such as `media/welcome.mp4` and put that actual file in a `media` folder beside `index.html`.
- Spoken audio needs a transcript. Video with speech or meaningful sounds needs appropriate captions; a `<track>` element can load a WebVTT caption file. A short description alone does not replace captions.

If the sample files do not load, continue with the question box and read the media code. You are not expected to create recordings during this lab.

### Your turn

Add a second `<details>` box asking `What should I do after changing my code?` Write your own answer inside a paragraph.

### Checkpoint

- [ ] Both question boxes open and close.
- [ ] I recognise `<audio>`, `<video>`, `<source>`, and `controls`.
- [ ] I tested playback if the online media was available.

## Task 9 — Check and repair

**Time: 7 minutes**

Spend **3 minutes** checking your page, **2 minutes** fixing the small example, and **2 minutes** answering the questions.

### 1. Check your page

- [ ] The browser title describes the page, and `lang="en"` is set.
- [ ] Headings follow a logical order.
- [ ] Links and images use correct paths.
- [ ] Informative images have useful `alt` text.
- [ ] Form controls have labels and work with the keyboard.
- [ ] IDs are unique, and navigation destinations exist.
- [ ] There is one `<html>`, one `<head>`, and one `<body>`.

If internet is available, open the [Nu HTML Checker](https://validator.w3.org/nu/), choose **text input**, and paste your complete HTML document. Fix any errors it reports. Warnings may need review rather than automatic removal. The checker does not prove that every link works or that the page is fully accessible, so still test it yourself.

### 2. Find the mistakes

This is an intentionally incorrect example. Write a corrected version on paper or in a temporary editor tab; do not replace your whole page with it.

```html
<h2>My hobbies</h3>
<p>I enjoy <strong>coding.</p></strong>
<img href="images/club.jpg">
<label for="student-email">Email</label>
<input type="email" id="email">
```

Fix the heading, nesting, image attributes, and label connection. Add a submission name to the input too.

<details>
<summary>Open after trying: one corrected version</summary>

```html
<h2>My hobbies</h2>
<p>I enjoy <strong>coding.</strong></p>
<img src="images/club.jpg" alt="A drawing of a computer used for learning">
<label for="student-email">Email</label>
<input type="email" id="student-email" name="email">
```

Use the actual image filename and an appropriate description for your picture.

</details>

### 3. Answer without looking back

1. How is `<title>` different from `<h1>`?
2. Which attribute gives a link its destination?
3. Why does an image need `alt` text?
4. What connects a label to a form control?
5. Does an HTML form automatically store a registration?

<details>
<summary>Open after answering: quick answers</summary>

1. `<title>` names the document in the browser tab; `<h1>` is the main heading in the page content.
2. `href`.
3. It supplies a text alternative when the image cannot be seen or contributes information that needs a text equivalent. Decorative images can use an empty alternative.
4. The label's `for` value must match the control's `id`.
5. No. A processing service or server is needed to receive and store it.

</details>

---

## Final task — Student Club Open Day

**Time: 30 minutes · Start at minute 90 · File: `open-day.html` · Total: 20 marks**

### Your challenge

Your student club is holding an open day. Create a complete HTML page that introduces the event, shows the programme, and lets visitors try a registration form.

Create `open-day.html` **beside `index.html`** so you can reuse the same `images` folder. Keep your guided page intact.

**Work independently.** You may use this README as a reference and reuse the basic document structure from Task 1. Write the event content and assemble the page yourself. Do not simply rename your completed Learning Hub page. Use HTML only; colours and decoration earn no extra marks.

### Content you can use

Use these details so that you can spend your time on HTML. You may invent a different club if you prefer.

| Item | Content |
| --- | --- |
| Club | Creative Computing Club |
| Event | Student Club Open Day |
| Date | 20 November 2026 |
| Venue | Computer Lab 1 |
| Introduction | Meet other students, try a small web activity, and discover our club. |
| Activities | Build a web page; try a quiz; meet the team. |
| Visitor steps | Arrive at the lab; choose an activity; join a group. |
| Programme | 9:00 AM — Welcome — 15 minutes; 9:15 AM — HTML activity — 30 minutes; 9:45 AM — Quiz — 15 minutes. |
| FAQ | Do I need experience? No. Beginners are welcome. |
| Footer | Created by your name. Practice page only. |

### Requirements and marking checklist

Award each listed point separately. A feature earns its point when it is present, meaningful, and works as described.

| Area | Required evidence | Marks |
| --- | --- | ---: |
| Document | Correct HTML skeleton with doctype and `lang` (1); meaningful title, charset, and viewport metadata (1). | 2 |
| Page structure | Appropriate header, main, and footer (1); navigation with at least two working internal links to unique IDs (1). | 2 |
| Text | One main heading and logical section headings (1); introduction and event details with one meaningful `<strong>` or `<em>` phrase (1). | 2 |
| Lists | At least three activities in an unordered list (1); at least three visitor steps in an ordered list (1). | 2 |
| Image and link | A working image with suitable `alt` text (1); a meaningful external learning link (1). | 2 |
| Programme table | Caption and appropriate header cells with `scope` (1); three programme rows with time, activity, and duration (1). | 2 |
| Registration form | Labelled required name and email inputs, with correct types (1); a labelled activity select and a labelled notes textarea (1); a labelled checkbox and a submit button (1); unique matching label/control IDs, submission names, and a clear practice-only notice (1). | 4 |
| Question box | A working `<details>` and `<summary>` FAQ with an answer. | 1 |
| Functional checks | Demonstrate required-field and email validation (1); demonstrate keyboard access to links, form controls, and the FAQ (1). | 2 |
| Source quality | Sensible indentation, one useful comment, and no known mismatched or incorrectly nested tags. | 1 |
| **Total** | | **20** |

Use `action="#register"` and `method="get"` for the practice form, and give its containing section `id="register"`. Use only made-up information. As in the guided task, submission does not save a real registration.

**Scope of this check:** The task assesses the core skills above. Audio/video, description lists, and some additional controls were introduced in guided practice but are not required in this 30-minute challenge.

### Suggested 30-minute workflow

| Minutes | What to do |
| --- | --- |
| 0–5 | Create the document, header, navigation, main area, and footer. |
| 5–13 | Add event text, lists, image, and external link. |
| 13–19 | Add the programme table and FAQ. |
| 19–25 | Build the practice registration form. |
| 25–30 | Save, refresh, test, and fix mistakes. |

### Final tests

1. Open `open-day.html` directly in your browser.
2. Click every link. Check that the image appears.
3. Submit the form empty; check that required information is requested.
4. Enter a name and the email `abc`; check that submission is blocked.
5. Use `Test Student` and `student@example.com` to test a valid entry.
6. Move through the page using **Tab**. Open the FAQ with the keyboard.
7. Check your code with the HTML checker if time and internet allow.
8. Give yourself a score out of 20 using the table. Write down one thing to improve.

### What to submit

Submit your `html-lab` folder or its repository link. Include:

- `index.html` — your guided practice page.
- `hello.html` — your second-page link exercise.
- `open-day.html` — your independent final page.
- `images/` — the image file used by your pages.

Do not submit only a screenshot: your HTML and image files are needed for checking. A screenshot may be included as extra evidence.

**Self-study guide:** 17–20 means a strong start; 13–16 means revisit the missed items; 0–12 means repeat the relevant guided tasks before trying again. These are suggested practice bands, not an official grading policy.

---

## HTML quick reference

Use this section when you forget a tag. You do not need to memorise everything today.

| Purpose | HTML |
| --- | --- |
| Document | `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>` |
| Document information | `<title>`, `<meta>`, `<link>` |
| Headings | `<h1>` to `<h6>` |
| Text | `<p>`, `<strong>`, `<em>`, `<mark>`, `<small>` |
| Text details | `<sub>`, `<sup>`, `<br>`, `<hr>` |
| Lists | `<ul>`, `<ol>`, `<li>`, `<dl>`, `<dt>`, `<dd>` |
| Links | `<a href="destination">Useful link text</a>` |
| Image and caption | `<img>`, `<figure>`, `<figcaption>` |
| Page regions | `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>` |
| Tables | `<table>`, `<caption>`, `<thead>`, `<tbody>`, `<tfoot>`, `<tr>`, `<th>`, `<td>` |
| Forms | `<form>`, `<label>`, `<input>`, `<select>`, `<option>`, `<textarea>`, `<button>` |
| Form groups | `<fieldset>`, `<legend>` |
| Media | `<audio>`, `<video>`, `<source>`, `<track>` |
| Expandable content | `<details>`, `<summary>` |
| Generic grouping | `<div>` for a generic flow container; `<span>` for a generic text-level container. Prefer meaningful elements when they fit. |

### Useful attributes

| Attribute | Main use |
| --- | --- |
| `id` | A unique identifier within the document. |
| `class` | Reusable group names, commonly used by CSS and JavaScript. |
| `lang` | The language of the document or an element. |
| `href` | A link destination. |
| `src` | An image, media, or script resource location. |
| `alt` | An image's text alternative. |
| `for` | Connects a label to a control's ID. |
| `name` | A form control's submission key. |
| `required` | Requires a value before normal form submission. |
| `placeholder` | A short input hint; not a replacement for a label. |
| `checked` / `selected` | Initial state of a checkbox/radio or an option. |
| `disabled` | Makes a control unavailable; its value is not submitted. |
| `readonly` | Prevents editing in supported controls; the value can still be submitted. |
| `min`, `max`, `step` | Range and step constraints for applicable input types. |
| `minlength`, `maxlength`, `pattern` | Text constraints on supported controls. |

### More input types to try later

| Type | Purpose |
| --- | --- |
| `text`, `email`, `number` | General text, email-format input, and numeric input. |
| `radio`, `checkbox` | One choice within a group, or an independent selection. |
| `password` | Masks the displayed characters; does not encrypt or securely store them. |
| `date`, `time`, `datetime-local` | Date/time entry; `datetime-local` does not include a time zone. |
| `tel`, `url`, `search` | Telephone, URL, or search entry; `tel` does not enforce a universal phone format. |
| `range`, `color` | A slider or colour picker. |
| `file` | File selection; actual uploading requires a receiving service. |
| `hidden` | A submitted value that is not displayed; it is not secret or protected. |

## Common problems and easy fixes

| Problem | Check this |
| --- | --- |
| The browser shows code as text | Check that the file ends in `.html`, not `.txt`, and open the actual file in the browser. |
| My changes do not appear | Save, refresh, and confirm you opened the file you are editing. |
| The image is missing | Check `src`, folder location, extension, and exact letter case. Renaming `.png` to `.jpg` does not convert an image. |
| My internal link does nothing | Match `href="#join"` with `id="join"`; make sure the ID is unique. |
| My form label does not focus the input | Match the label's `for` with the input's `id`. |
| Both radio buttons stay selected | Give radio buttons in one group the same `name`. |
| The browser accepts an empty email | `type="email"` checks a non-empty value's format; add `required` if a value is mandatory. |
| My table has no lines | This is normal without CSS borders. |
| My page looks plain | HTML provides meaning and structure; learn CSS next for presentation. |
| The page looks okay, but the checker reports errors | Browsers repair many mistakes automatically. Fix the source instead of depending on that repair. |
| My valid form did not send an email | HTML alone does not supply an email or registration service. |

## Continue learning after the lab

These topics complete a broader HTML learning path. Work through them over later sessions; they are not requirements for the two-hour lab.

| Topic | Small next activity |
| --- | --- |
| More text meaning | Mark up a quotation with `<blockquote>` or `<q>`, an abbreviation with `<abbr>`, a date with `<time>`, and code with `<code>` and `<pre>`. |
| More page structure | Create a news page with two `<article>` elements and a related `<aside>`. |
| Nested lists | Put a second list inside one `<li>` to show subtopics. |
| More table features | Add a `<tfoot>` total; explore `colspan` and `rowspan` only when the data needs them. |
| More form features | Explore autocomplete, date/file inputs, `<datalist>`, grouped options, and validation patterns. |
| Responsive images | Learn `<picture>`, `srcset`, and `sizes`; provide images appropriate to the display. |
| Accessible media | Create a transcript and a real WebVTT captions file, then connect it with `<track>`. |
| Embedded content | Explore an `<iframe>` with a meaningful `title`; learn embedding permissions and `sandbox` restrictions. |
| Metadata | Add a description meta tag and a favicon with `<link rel="icon">`. |
| International text | Try Sinhala text with UTF-8; mark a Sinhala passage with `lang="si"`. Learn `dir` for text direction. |
| Native interaction | Explore `<dialog>` and popovers; learn which behaviours need JavaScript. |
| Graphics | Learn the difference between SVG markup and `<canvas>`, which usually needs JavaScript for drawing. |
| Templates and custom elements | Explore `<template>`, `<slot>`, and Web Components after learning JavaScript. |
| Accessibility | Practise keyboard testing, meaningful heading order, appropriate alternatives, and screen-reader checks. |
| HTML with CSS and JavaScript | Link a stylesheet and a script; understand which language handles each responsibility. |
| Publishing | Learn relative paths on a hosted site and publish your static pages with GitHub Pages. |

**Avoid outdated layout tags:** Do not use `<font>`, `<center>`, or `<marquee>`. Learn CSS for presentation. Also, a single rendered page cannot demonstrate that you know all HTML; keep building and checking different kinds of pages.

### Learning references

The tasks and scenarios in this lab are original teaching exercises. Use these documentation sources to check syntax and explore further:

- [MDN: Basic HTML syntax](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/Basic_HTML_syntax)
- [MDN: Your first form](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Forms/Your_first_form)
- [WHATWG: HTML Living Standard](https://html.spec.whatwg.org/multipage/)
- [Nu HTML Checker](https://validator.w3.org/nu/)

### For the instructor or repository owner

Place this file at the repository root as **`README.md`**. GitHub will display it as the repository's instruction page. The sample HTML belongs in separate `.html` files; GitHub's README view is not a live preview of those pages.

Have the editor and an image ready before the timed session. Give students a minute-90 reminder, then let them work independently. Check the final file against the 20-mark checklist. The expandable answers are for guided practice; the final challenge intentionally has no completed model page to copy.

