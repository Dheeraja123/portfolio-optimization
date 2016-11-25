# portfolio-optimization## Website Performance Optimization portfolio project

### Getting started
## Website Performance Optimization portfolio project

### How to Run
1. Open Indext.html in your browser.

2. Go to https://github.com/excelandaccess/mobile-portfolio-master.git to view or download

### Minify resource
Used http://www.minifier.org/ to minify css and js files


####Part 1: Optimize PageSpeed Insights score for index.html
###Items updated
1. Index.html
  * Inlined style.css since referenced just once
  * Move Google analytics to bottom and added async for rendering
  * Added media="jprint" for print.css
  * referenced css, js files to minified version 
  * Inlined font-face

2. js\__perfmatters.js__ - minified

3. css\__print.css__ - minified

4. __project-2048.html__, __project-mobile.html__, __project-webperf.html__
  * Inlined style.css since referenced just once
  * Move Google analytics to bottom and added async for rendering
  * Added media="jprint" for print.css
  * referenced css, js files to minified version 
  * minified pics


####Part 2: Optimize Frames per Second in pizza.html

5. views\__pizza.html__
  * referenced css, jpg, png files to minified version
  * added viewpoint meta tag


6.I made the following optimizations to the code (All changes are in ```views/js/main.js``` unless otherwise indicated):
* Refactored the ```changePizzaSizes()``` function to eliminate a forced synchronous layout.
* Refactored the ```updatePositions()``` function to eliminate another forced synchronous layout.
* Incorporated a ```requestAnimationFrame``` into the scroll function to smooth rendering.
* Used a more efficient DOM selector to select the moving pizzas in ```updatePositions()```
* Refactored the code for generating moving pizzas (See the ```eventListener``` code for ```DOMContentLoaded```) to create only as many moving pizzas as fit on the screen.
* Since there are now many fewer moving pizzas, I put each one into its own layer with a ```will-change``` directive in ```views/css/style.css```.

7. views\images\
  * minified picture files

8. views\css\__style.css__
  * added backface-visibility: hidden; to .mover

9. views\css\
  * minified files

### Customization with Bootstrap
The portfolio was built on Twitter's <a href="http://getbootstrap.com/">Bootstrap</a> framework. All custom styles are in `dist/css/portfolio.css` in the portfolio repo.

* <a href="http://getbootstrap.com/css/">Bootstrap's CSS Classes</a>
* <a href="http://getbootstrap.com/components/">Bootstrap's Components</a>
