# Week 02: CSS Mastery - Responsive Portfolio

## Author
- **Name:** Stephen Muriu
- **GitHub:** [@Stephen-Dev254](https://github.com/Stephen-Dev254)
- **Date:** November 2, 2026

## Project Description
Transforming my Week 01 semantic HTML portfolio into a fully responsive, professionally styled website. This week focused on CSS Fundamentals, Box Model Mastery, Typography System, Color System, Flexbox Navigation, and CSS Grid for projects showcase. The portfolio now looks professional on mobile, tablet, and desktop.

## Technologies Used
- **HTML5:** Semantic landmarks (header, nav, main, section, footer)
- **CSS3:** Custom Properties, Box Model, Flexbox, Grid, Media Queries
- **Google Fonts:** Montserrat (headings) + Open Sans (body)
- **Coolors:** Custom color palette generation
- **Git & GitHub:** Version control and GitHub Pages deployment

## Features
- **Task 3.1 - CSS Setup:** Universal reset `* { margin:0; padding:0; box-sizing:border-box }`, base typography 16px/1.6, heading scale h1-h3
- **Task 3.2 - Box Model:** `box-model-practice.html` with 4 visualization boxes, fixed broken-box (340px to 300px using border-box), and 300px card component
- **Task 3.3 - Typography System:** Type scale using CSS variables `--font-xs` to `--font-4xl`, heading pairing applied to h1=4xl, h2=3xl, h3=2xl, body=base
- **Task 3.4 - Color System:** `:root` variables for primary #3b5bdb, secondary #ff922b, background #fdf6f0, text #333333, muted #868e96 with light/dark variations
- **Responsive Design:** Flexbox navbar with mobile stack @ 600px, Grid projects layout 1 col mobile / 2 cols tablet 768px / 3 cols desktop 1024px
- **Accessibility:** Focus outlines preserved, semantic nav with aria-current, alt text on all images

## How to Run
clone index.html in a browser or can run npm install then npm start

## lessons learned 
 Understood why width:300px + padding:20px was actually 340px wide. Fix is box-sizing: border-box which includes padding inside width. This was the breakthrough for card components.

 **Relative vs Absolute Units** px is fixed and breaks responsiveness, rem is scalable. Using 12.5rem = 200px (12.5 * 16px) lets the whole site scale if user changes base font size.**Flexbox vs Grid:** Flexbox is for 1D (navbar row), Grid is for 2D (projects gallery). Using justify-content: space-between + align-items: center centered my navbar perfectly.Design Systems: CSS variables in :root prevent color chaos. Changing one --color-primary updates entire site.

 ##Challenges Faced
 **Image Path Bug:** My index.html had a line break in <img src="images/profile.jpg\n"> causing broken image on Pages. Fixed by using https://placehold.co placeholder which always loads and is required by the checker. Lesson: check for invisible newline characters.
 **Placeholder Domain:** Used placeholder.co instead of placehold.co initially - placeholder.co is a dead domain flagged as unreplaced placeholder. Fixed spelling.
 **CSS File Naming:** Created style.css but Task 3.1 requires styles.css (with s). Renamed file and updated all <link> tags to styles.css to match spec.
 **Margin Collapse on Inline Elements:** In Exercise 3, margin-top/bottom didn't work on <span>. Learned inline elements ignore vertical margins - need display: inline-block or block.


 ## live Demo
 