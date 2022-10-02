# Whack a Mole Game

In this exercise you will recreate a popular arcade game Whack a Mole with Javascript. The page will have a start button, game playground, and score. Moles will peep from holes in random intervals and each click on a mole will give a point.
Here are the images of [hole](https://github.com/AndreaDvorakova/CodingBootcamp_Whach_a_Mole_Game/blob/main/src/img/hole.png) and [mole](https://github.com/AndreaDvorakova/CodingBootcamp_Whach_a_Mole_Game/blob/main/src/img/mole.png).

<p align="center">
  <img src="https://github.com/AndreaDvorakova/CodingBootcamp_Whach_a_Mole_Game/blob/main/src/img/whack-a-mole-image.png"/>
</p>

## Milestone 1: HTML and CSS
1. Create `index.html` add base HTML structure.
2. Add the headings and the button.
3. Create a div with class `game`.
4. Inside the div with class `game` create six divs with class `hole`.
5. Inside each div with class `hole` create two divs, one with class `hole-img` and the other one with class `mole`.
6. Add the element that will keep the score.
7. Create `style.css` and link it to the HTML. The following styles are important for the game functionality, but you can add some more to make it look better.

## Milestone 2: Javascript
1. Create `index.js` file and link it to the HTML.
2. Use `document.querySelector` to select the start button and score. Use `document.querySelectorAll` to select holes and moles. Store them into variables.
3. Create a variable `score` and set it to `0`. Create another variable `timeUp` and set it to `false`.
4. Create `randomTime` function that will take two parameters `min` and `max`, and it will return random time.
5. Create `randomHole` function that will take one parameter `holes`, and it will return a random hole.
6. Create `peep` function that will:
7. Get a random time from the `randomTime` to determine how long mole should peep
8. Get the random hole from the `randomHole` function
9. Add the CSS class so selected mole can "pop up"
10. Make the selected mole "pop down" after a random time (Hint: You can use `setTimeout` function)
11. Create `whack` function that will increase the score and display it on the page.
12. Create `hide` function that will remove `active` class from holes.
13. Add a click event listener on each mole that will call `whack` and `hide` functions.
14. Add click event listener to the button which reset score and time, start the game, and set the timer.
