## Website Performance Optimization portfolio project

Open index.html and views/pizza.html in the web browser to examine optimizations.
Source files are placed inside `src` folder and production files inside `dist` folder.

###Optimizations made in index.html.
1. Use Web Font Loader to load google font asynchronously.
2. Added async attribute to analytics.js since it's not needed to render the page.
3. Inlined styles from style.css.
4. Specify media print for print.css so it doesn't rendor block the CRP.
5. Converted `profilepic.jpg` to png and performed compression.
6. Resized and compressed the pizzeria.jpg used as the preview image.
7. Minified index.html to reduce size.

###Optimizations made in views/js/main.js for views/pizza.html.
1. Removed the unnecessary `determineDx` function and refactored `changePizzaSizes` function to handle the pizza resizing.
2. Replace all instances of `querySelectorall` to `getElementsByClassName`.
3. Declared 'var items' as global variable so it can be referenced inside the anonymous function that runs when DOMContentLoaded event is triggered.
4. Refactored `for loops` inside `updatePositions` function to boost performance.
5. Reduced number of background pizzas generated to 35.

