# CIS 311 · Homework 2 — Semantic Rescue

*AI Usage* : Don't use AI to code on this assigment. You may use AI as a tutor to ask for an explanation. Don't copy/paste out of AI into your code. Just the process of typing helps you learn. 

---

## The situation
The Elm Street Food Pantry has a website. It looks fine. It is structurally meaningless — every element on the page is a `<div>` or a `<span>`, headings are fake, links aren't links, and **every single form control is `<input type="text">`**, including the ones that are asking for a date, a file, a yes/no answer, and a pick-one-of-three.

Your job is to rebuild the structure so that the page means what it looks like, and so that the form asks for what it's actually asking for.

## What you're given
- `index.html` — the page, in div soup
- `styles.css` — the design, written entirely against **classes**

Every CSS selector targets a class, never an element name. You can change every tag in the file and the page will still look the same. **Keep the classes. Change the elements.** You may add CSS selectors if a real element brings default styling you need to reset (list bullets, table borders, `fieldset` borders, `button` and `select` defaults). Your job is NOT to redesign the page, but you may make improvements if you wish.

**The form is the one exception to "it should look the same."** A date picker looks different from a text box. That's the point. Redesign the form using as much additional CSS as you want. 

---

## Requirements

### Structure
1. **Landmarks.** The page uses `header`, `nav`, `main`, `footer`, `search`, and at least one `aside` or `section` used correctly — not sprinkled decoratively.
2. **Heading outline.** Exactly one `<h1>`. No skipped levels. Reading the headings alone should outline the document. (The starter has *zero* real headings — deciding what the `<h1>` is, is part of the assignment.)
3. **Real interactive elements.** Anything that navigates is an `<a>`. Anything that performs an action is a `<button>`. No `onclick` on a `div` or `span` anywhere in your submission.
4. **Lists and tabular data.** Content that is a list is marked up as a list. Content that is a grid of rows and columns with headers is a `<table>` with real `<th scope>`.
5. **Images.** Meaningful images get useful alt text. Decorative images get `alt=""`. There is at least one of each on this page — find them.
6. **Specialized elements** where the content calls for them. The page contains at least a quotation, a figure with a caption, and a physical address. There are more.

### The form — the heart of this assignment
7. **Wrap it in a `<form>`.** There isn't one.
8. **Choose the right control for every field.** Fifteen controls on this page are `<input type="text">`. **Exactly one of them is already correct.** For the other fourteen, read what the field is asking for and decide:
   - Does a more specific **input type** fit? (There are seven of these.)
   - Or does the question call for a **different element entirely** — a group of radios, a group of checkboxes, a dropdown, a multi-line box?
   - Add the attributes that make your choice real: `min`, `max`, `step`, `accept`, `multiple`, `required`, `autocomplete`.
9. **Label everything.** Every control has an associated `<label>`. The divs currently sitting above the fields are not labels. Placeholders are not labels. Where a field has *only* a placeholder, you must write a label.
10. **Group what belongs together.** Any set of mutually exclusive or multi-select options is wrapped in a `<fieldset>` with a `<legend>`. The legend is the question.
11. **A real submit button.**


## What you submit
Post **your live URL to your site on GitHub Pages** on Canvas. 

