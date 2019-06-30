# rockPaperScissorsVanillaJs

Traversy Media tutorial.

https://www.youtube.com/watch?v=WR_pWXJZiRY&list=PLYyGnWAjIQwS0NcKqpNK8YaWhy0UU0VEh&index=4&t=200s

### Ideas to Improve the game

- ~~Show **You Lose** in a different color~~
- Hide the **Restart Game** till there is a score
- Add a maximum total score count so the game doesn't continue indefinitely
- Add Rounds if there is a max total score count

## Javascript Steps

1. Get all the selectors, there is more than one type. Choice / Score / Result / Restart / Modal
   make a scorboard object that keeps track of scores

2. Make a function called play(). It should select the target based on id <-- store in a variable. Need an event listener with a foreach loop. The function should also display the Restart Button

3. Need to get computer choice. store in a variable computerChoice in play function the result of getComputerChoice(); Use a math random function.

4. Need to determine winner. Make a variable in play() that calls getWinner(); use if statement to determine indvidual winning scenarios. Return 'computer' or 'player'

5. Make a function called showWinner(). This will show the winner + the computerChoice.

   1. Use if statements.
   2. The function increases the score.
   3. It also inserts the innerHtml for result seletor.
   4. Need to also insert the innerHtml for score within this function for the score seletor.
   5. Need to change the display style to show the modal.

6. Add an event listener on the window that will close the modal. it calls a function called clearModal(); that hides the modal. Need to set the display back to it's original

7. Need to restart the score back to zero if the restart game button is pressed. Use an event listener that calls a function restartGame()that resets the score and also sets the innerHTML for the scores.

8. Make the first letter of computerChoice in the modal upper case. Use charAt() and slice()
