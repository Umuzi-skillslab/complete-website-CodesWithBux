[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/YDjuDFNG)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23198434&assignment_repo_type=AssignmentRepo)
# Portfolio Website Starter Code
 Issues Found in the Starter Code
 
•	All pages missing lang="en" on the <html> element — screen readers cannot detect page language
•	All pages missing <meta charset="UTF-8"> — character encoding was undefined
•	All pages missing <meta name="viewport"> — mobile layout was broken
•	<div class="header"> used instead of semantic <header> on all pages
•	<div class="footer"> used instead of semantic <footer> on all pages
•	No <main> element on any page — missing ARIA landmark region for screen readers
•	Navigation entirely missing on index.html
•	No <nav> element on any page — navigation not semantically marked
•	Content sections used <div> instead of <section> throughout
•	Project blocks used <div> instead of semantic <article>
•	About page: table was noted as missing, no <table> existed
•	Table missing <thead>, <tbody>, <th scope>, and <caption>
•	All <img> tags missing alt attributes
•	Contact form had no <label> elements for any input
•	Form only had text and textarea inputs — needed 5+ types
•	No HTML validation attributes (required, minlength, pattern) anywhere
•	Radio/checkbox inputs lacked <fieldset> and <legend>
•	No aria-label, aria-current, or aria-required on any element
•	No id attributes to link labels to inputs
•	No skip-to-main-content link for keyboard users
•	Footer text-align was left instead of centred

CSS Issues

•	Only 2–3 selector types used — needed 5+
•	No pseudo-classes (:hover, :focus, :nth-child) used anywhere
•	No descendant selectors (e.g. nav ul li a)
•	No ID selectors
•	No pseudo-elements (::before, ::after)
•	Navigation styling completely absent
•	Table styling completely absent
•	Form styling incomplete — only display:block on inputs
•	No box model demonstration (margin, padding, border)
•	Font declared as Arial with no proper fallback stack
•	No :focus styles — keyboard navigation inaccessible
•	No hover transitions on interactive elements
•	Inconsistent formatting and no logical organisation in CSS file

 Fixes Implemented
 
Every page now has lang,, viewport, and description meta. Replaced all div.header with <header> and div.footer with <footer>. Added <nav>, <main>, <section>, <article> throughout all pages. Added consistent navigation with 4 working links on all 4 pages. All images have descriptive alt text. Built a full skills table with thead, tbody, th scope, and caption on the About page. Contact form rebuilt with 5 input types (text, email, select, checkbox, textarea), every input has a label, and validation uses required, minlength, and pattern. Added a skip-to-content link. Footer fixed to text-align: center.
CSS was rewritten using CSS custom properties. Added selectors types including element, class, ID, descendant, pseudo-class, and pseudo-element. Added :hover, :focus, :nth-child on the skills table, and card hover animations. Full box model demonstrated. Navigation, table, and form all fully styled. 

HTML Structure & Semantic Choices

Every page follows this landmark structure: <header> with site logo and <nav>, <main> wrapping all page content, <section> for grouped content areas, <article> for self-contained blocks like project cards and the about grid, and <footer> for copyright and contact.
This structure ensures screen readers can navigate by landmark, search engines understand the content hierarchy, and the document outline is logical and consistent across all four pages.

 CSS Styling Approach
 
CSS define the colour palette and typography, making the design easy to maintain. The stylesheet is organised into 16 labelled sections: Reset, Base Styles, Layout Helpers, Skip Link, Header & Navigation, Buttons, Hero Section, , Page Banner, About Page, Data Table, Certifications, Projects, Contact Form,  and Footer..
Selector types used: element (body, h1, table), class (.project-card, .cert-card), ID (#main-nav, #site-logo), descendant (header .container, .skills-table thead), attribute (input[type="text"]), and pseudo-class (:hover, :focus, :nth-child). Bootstrap is loaded for its utility resets, while all design is implemented in the custom styles.css.

Accessibility Improvements

•	lang="en" added to all HTML elements
•	Skip-to-main-content link added on every page
•	:focus styles on all interactive elements (buttons, links, inputs)
•	Semantic HTML landmarks for screen reader navigation
•	Table caption and th scope added for data table accessibility

7. How to View Locally

1. Download or clone the repository to your computer.
2. Open the project folder in File Explorer (Windows) or Finder (Mac).
3. Double-click index.html — it will open in your default browser.
4. Use the navigation menu to move between pages. All links are relative so they work without a server.

The most challenging part was the CSS. The starter file had placeholder comments marked as errors, but many underlying declarations were structurally valid ,the real problem was: no selector variety, no pseudo-classes, no box model, no layout system. Rebuilding around CSS custom properties made everything consistent and easy to scale.
On the HTML side, replacing generic div containers with semantic elements required careful attention to document structure and heading hierarchy. The accessibility work, skip links, aria attributes, focus styles, form labels, was the most rewarding, because it makes the site genuinely usable for everyone, not just mouse users.
I also added a certifications section, a professional hero design with a photo, and Bootstrap as a utility reset, which were improvements beyond the starter requirements. These are documented here so the assessor can see they were intentional 

