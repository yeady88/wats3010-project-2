# Golden Ratio

**Responsive Web Design | Layout Techniques | Working with Media**  

In this assignment we build a multi page responsive website. It will require flex, grid and column layouts.  The pages and assets are included in this repo.  There are `TODO`s in each page that provide pointers to what needs to be done in order to complete the HTML in the page.  There is also an empty style sheet `css/style.css` that we'll work on.

***Learning Objectives***  

1. Multi page layout with external links
2. Tabular data content: table element/tag
3. Embed video
4. Host video
5. Host audio
6. Layout: display column, relative, absolute, fixed
layout,	flex, grid
7. Responsive Web: Media queries
8. Icons: font awesome
9. Typography: google fonts
10. Interactive CSS	:target, :hover
11. Variable property values in CSS: colors 
12. Reading designs


See the design folder for comps and wireframes.  All interpage navigation takes place through a nav bar. The information architecture diagram indicates that every page is available from every other page and this is all via the nav bar.  It is a mobile first nav bar with a hamburger.  

![Information Architecture Diagram](design/golden-ratio-info-architecture.png).

## HTML
See `TODO`'s for location of HTML changes
1. Add `<title>` to all 4 pages. 
 - index.html: "Golden Ratio"
 - fibonacci.html: "Golden Ratio: Fibonacci"
 - media.html: "Golden Ratio: Media"
 - about.html: "Golden Ratio: About"

2. Add favicon to all pages.  
```
<link rel="icon" type="image/png" href="images/phi_640.png">
```
3. Add list items for social links to `icon-bar` on all pages
```
 <li>
    <a target="_blank" href="https://www.facebook.com" class="facebook"><i class="fab fa-facebook"></i></a>
    </li>
    <li>
        <a target="_blank" href="https://www.twitter.com" class="twitter"><i class="fab fa-twitter"></i></a>
    </li>
    <li>
        <a target="_blank" href="https://www.github.com" class="github"><i class="fab fa-github"></i></a>
  </li>
```
4. Add hamburger and brand to all headers.
```
  <a class="toggle open" href="#nav">&#9776;</a>
  <h1 class="brand"><a href="./index.html">Golden Ratio</a></h1>
```
5. Add list items with navigation and set current page active.  The example below is setting the Home page (index.html) to active.
```
 <li class="active">
    <a href="#">Home</a>
  </li>
  <li class="">
      <a href="fibonacci.html">Fibonacci</a>
  </li>
  <li>
      <a href="media.html">Media</a>
  </li>
  <li>
      <a href="about.html">About</a>
  </li>
  ```
6. Add contents to Footer on all pages.  Use the code below, but update the copyright date and use your name for the author.
```
<ul class="copyright">
  <li>Copyright &copy; 2018</li>
  <li> Ima Webcontentwriter</li>
</ul>
```
7. Wrap `header` thru `footer` tags in a `<div>`.  Add class `container` to the div on `index.html` and `fibonacci.html`.  Add class `single-col-container` to the dev on `media.html` and `fibonacci.html`. This will be used for applying grid layout. 
8. Masonry effect on `index.html`: Wrap all `article` elements in a `div` with class `golden-mason`.
9. Credits on `index.html`: Wrap the `ul` in the `aside` in a `div` with the class `credits`.
10. On the `fibonacci.html` page, add a `table` elements with 3 columns. The first column should contain the value of the row (0-6), the second should contain the sum of i and the previous value of i (1,1,2,3,5,8). The third columns should contain the value of the second column divided by the second column in the previous row (na, 1, 2, 1, 1.5, 1.7, 1.6, 1.625).  See the comp for questions about the data.  On the first rows use `<th>` and  `scope="col"` on the columns 2 and 3.  On the remaining rows set use `<th>` and `scope="row"` on the first column.  This is to improve accessibility.
11.  On th `fibonacci.html` pages, add picture of Fibonacci, the man, and his book.
```
 <figure class="fibonnaci">
      <img src="images/fibonacci.jpg" alt="Leonardo Bonacci,aka Fibonacci">
      <figcaption>Leonardo Bonacci, aka Fibonacci</figcaption>
  </figure>
  <figure class="book-of-calc">
      <img src="images/book-of-calculation.jpg" alt="from The Book of Calculation">
      <figcaption>The Book of Calculation <br>by Fibonacci</figcaption>
  </figure>
```
12. On the `media.html` page wrap the audio in a `div` with class `audio-container`.  The div should enclose both the head and audio elements.  Then wrap each video iframe responsive container and head element in a `div` with class `frame-container`.
13. On the `about.html` page add the XKCD clickable comic in a container.
```
    <div class="xkcd-container">
      <a href="https://xkcd.com/spiral/" target="_blank">
        <img src="https://imgs.xkcd.com/comics/flowcharts.png" />
      </a>
    </div>
```
14. On the `about.html` page add class `learning-objectives` to the ordered list.

## CSS






