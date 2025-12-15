Day 3 — Layout Foundations: Containers, Wrappers & Page Structure
🔹 1. Why Layout Matters Before CSS

Before styling anything, a website needs a strong HTML structure.

Good layout structure:

makes styling easier

avoids messy CSS later

allows the site to scale

prepares the project for React or any framework

helps other developers understand your code

For AfriBuildTrack, layout structure is critical because:

the landing page will grow

dashboards will be complex

components must be reusable

🔹 2. The .container Pattern (Very Important)

A .container is used to control the width of content and center it on the page.

✔️ Purpose of .container:

prevents content from stretching too wide

improves readability

keeps spacing consistent across sections

creates a professional layout

✔️ Typical usage:
<div class="container">
    <!-- Section content -->
</div>

🔹 Key rule:

Almost every major section should contain a .container.

This includes:

header

hero section

features

pricing

footer

🔹 3. The .wrapper Pattern

A .wrapper is used inside a container to control how elements are arranged.

✔️ What .wrapper is used for:

grouping related elements

placing items side-by-side

preparing layouts for Flexbox or Grid

structuring hero sections and feature lists

✔️ Example:
<div class="wrapper">
    <div>Text content</div>
    <div>Image or media</div>
</div>

✔️ Difference between .container and .wrapper:
Container	Wrapper
Controls width	Controls layout
Centers content	Aligns content
Used everywhere	Used when needed
🔹 4. Section-Based Page Structure

Modern websites use <section> to group related content.

✔️ Why use <section>:

improves accessibility

helps screen readers

improves SEO

keeps code organized

✔️ Example:
<section id="features">
    <div class="container">
        <h2>Features</h2>
    </div>
</section>

🔹 5. Hero Section Structure

The hero section is the most important part of a landing page.

✔️ Common hero pattern:
<section id="hero">
    <div class="container">
        <div class="wrapper">
            <div class="hero-text">
                <h1>Main headline</h1>
                <p>Short explanation</p>
            </div>
            <div class="hero-media">
                <!-- image or illustration -->
            </div>
        </div>
    </div>
</section>


This structure allows:

responsive layouts

side-by-side content

easy styling later

🔹 6. Feature Section Structure

Features are usually displayed in a grid or cards.

✔️ Structure example:
<section id="features">
    <div class="container">
        <h2>Features</h2>
        <div class="wrapper">
            <div class="feature-card"></div>
            <div class="feature-card"></div>
            <div class="feature-card"></div>
        </div>
    </div>
</section>


This prepares the section for:

CSS Grid

animations

reusable components

🔹 7. Footer Structure

Even the footer should follow layout rules.

✔️ Best practice:
<footer>
    <div class="container">
        <p>© 2025 AfriBuildTrack Africa. All rights reserved.</p>
    </div>
</footer>


This keeps footer width consistent with the rest of the page.

🔹 8. Common Beginner Mistakes

Forgetting .container in sections

Misspelling class names (e.g. warpper)

Styling before structure is complete

Mixing layout and content responsibilities

Using <div> instead of semantic elements

🔹 9. Key Takeaways

Always think about structure before styling

.container controls width and alignment

.wrapper controls layout and grouping

<section> organizes content meaningfully

Clean structure makes CSS and JS easier

This foundation prepares the project for React and dashboards