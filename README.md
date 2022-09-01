# Devil's Grip is a cardgame that plays similar to solitaire, with a more complex rule set.

You will need node.js installed to be able to run this app locally: https://nodejs.org/en/

Once node is installed, you can run "npm install" in both the client and server files.

In the server file, you will also need to run "npm run seeds" to setup the leaderboard database, and "npm run server:dev:" to host the server locally.

In the client file, you just need to run "npm start" to start the server.

On the home page for Devil's Grip, there should be a start game option, a difficulty drop down menu, and a ruleset at the bottom.  Clicking on start game will create a deck using a deck api, and will load 24 cards into a grid, which is stored in a 3d array.  From here you can choose 2 cards to either swap, or stack by clicking on them.  If the first card clicked is stackable onto the second card, they will stack, otherwise they will swap.  Empty spaces are automatically filled from the deck.  Clicking on the deck draws 3 cards into your talon, with which you can stack onto cards on the grid.  If you fully empty the deck by repeatedly drawing from it into the talon, the talon is flipped over and becomes the deck.  The cards remain in the same order.  The end goal is to have every card held in the grid, with no cards remaining in the deck/talon.

Clicking on give up will end the game, displaying the leaderboard and give you the option to save your name, score, and difficulty to the leaderboard.  The leaderboard is stored in the backend, held separately from the game.

For this javascript project it was worked on in a group of 4, and I built the backend server, the game logic, the selectable difficulties, and the 3d array that stores the grid.

If I were to work on something like this again, I would've liked to have done more of the css styling myself, to become more comfortable with it.  I currently don't enjoy using css as it is frustrating in how you can change or add mutliple lines of css, and the page either not changing at all, or not looking how you expected it to.

Overall I am really happy with how the project turned out, especially given that it was my first group project, and we only had 1 week to build it.
