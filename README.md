**How to Play**
Open the game in your browser.
Click on a card to flip it and reveal its content.
Click another card to find a match.
If the cards match, they remain revealed; otherwise, they flip back.
Repeat until all pairs are matched.
**Project Structure**
index.html: Contains the basic structure of the game.
tailwindcss: Defines the styles for the game, including the card designs and animations.
script: Includes the game logic, such as flipping cards, matching logic, and tracking stats.
**Logic Explanation**(Javascript)
Card Flipping
Matching Logic
Tracking Stats
Restart Functionality
**Card Flipping**
 The click event listener flips a card by adding a class or applying a CSS transform.
**Matching Logic**
 When two cards are flipped, their contents are compared. If they match, they stay revealed; otherwise, they flip back after a delay
 If they match:
       Cards stay flipped.
       Pointer events are disabled to prevent further interaction.
If they don't match:
       A delay is introduced before flipping the cards back to allow the player to memorize their positions.
**Tracking Stats**
Functions update the number of moves and the timer to provide feedback to the player.
    Moves counter increments every time two cards are flipped.
    The timer starts when the game begins and stops when all pairs are matched.
**Restart Functionality**
 A function shuffles the cards and resets stats to start a new game.
        Shuffles the card deck.
        Resets stats (moves and timer).
        Flips all cards back to their initial state.
**Shuffling the Cards**: A simple algorithm like the Fisher-Yates shuffle is used to randomize the card positions.
**Game Completion**: When all pairs are matched, a completion check is triggered:
 
