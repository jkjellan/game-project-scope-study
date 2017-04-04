# Game Project Scope Study

## Required Readings

-   [Game Project](https://github.com/ga-wdi-boston/game-project)
-   [Game API](https://github.com/ga-wdi-boston/game-project-api)
-   [What is a User Story](https://www.mountaingoatsoftware.com/agile/user-stories)

## Deliverables

After reading the `game-project` prompt and the `game-project-api` documentation
please do the following and be prepared to share and discuss during our next
class.

Submit detailed answers to the following in this file via a pull request:

-   A wireframe of what your game project will look like.
desktop:  <http://imgur.com/1xwuf1b>,
mobile:   <http://imgur.com/rFRisS6>

-   The data structure you plan to use.
series: {[
  game: {
    id: 1,
    gameboard: ['x', 'o', 'x', 'x', 'o', 'x', 'o', 'o', 'x',],
    playerX: {
      id: 1,
      username: 'unqueUserName',
      email: 'email@gmail.com'
    }
    playerO: {
      id: 2,
      username: 'uniqueUserName',
      email: 'email@gmail.com'
    }
    winner: function () {win logic check}
  }
]}

-   How you will take the markup of the game board and represent it in JS

I play to give numbers id's to each of the 9 divs of my gameboard (0-9), and I plan to loop through my js gameboard array, rendering each index to the 9 divs based on ID, i.e. $('#' + i).html(gameboard[i])

-   How you plan to approach this project.

I want to hack together a spaghetti code version so that I understand how to build the basic game logic.  Then I need to refactor the code around my entity objects i.e. game object, player objects, series object. Then I need to figure out how to interact with the API to get online play working.

-   4-8 user stories for your game project.
As User, I want to be able to select my own unique marker that I use for all my games.
As User, I want to be able to see a history of each completed Game Board for every past match.
1. As User, I want to be able to see match statistics, filterable by opponent:  win %, loss %, tie %, % first mover, total games, won, lost, tied.
2. As Player, I want to select local or remote game, so that I can play on either same of different device as opponent.
3. As Player, I want to be randomly assigned Player One or Player Two status, with my opponent assigned the inverse, so that there is a level playing field
4. As Player, I expect for it to be clear when it is my turn
5. As Player One, I expect to move first for Game 1 of a series, alternating for each subsequent game in the series.
6. As Player Two, I want to be allowed to go first for game 2 of the series, alternating for every subsequent game of the series

-   How you plan to keep your code modular.
Module 1: PlayerX turn
Module 2: PlayerY turn
Module 3: Win logic
Module 4: draw logic
Module 5: render gameboard
Module 6: keep score in game
Module 7: track games in series
Module 8: player statics

-   What creative spin will you add to your project?

I want a lot of feedback given to the users during play. i.e. I want them to see how many remaining X's and O's remain to be played each turn, I want it to prompt the user when it is their turn, I'd like to add some basic animations, etc.

-   How will you use version control to backup / track your project?

I play to make a branch for every feature, and merge in to master when complete.  I play to commit often.

-   Do you plan to attempt any of the bonuses?

I really want to get play from separate devices working.  I'd love to have a waiting room, with chat for pairing up opponents. Definitely play on keeping track of multiple rounds with a win counter.  We'll see how much time I have, though.

You may want to submit pictures for your wireframes and/or user stories.
[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
has instructions to link to a picture you've uploaded to a service like [Imgur](http://imgur.com/).
