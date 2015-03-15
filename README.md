Project 4: Website Optimization
===============================

The project can be run by following the link: http://maromishan.github.io/webOptim/

The following opimizations were made to the file: views/js/main.js:
1. The number of pizzas redered were reduced to 30
2. Used requestAnimationFrame to update animations before upcoming repaints
3. Took out static calculations for pizza animation outside of for loop
4. Took out defining of variables outside of for loop (Do not need to redefine things over and over again)
5. Used getElementsByClassName instead of querySelectorAll because it is faster
   see https://jsperf.com/getelementsbyclassname-vs-queryselectorall/15

In views/css/style.css, I changed style for .mover class: Added the lines:
  -webkit-backface-visibility: hidden;
  -webkit-perspective: 1000;
  These improve the way the page is layered