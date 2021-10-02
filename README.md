# pokedex
Check out the live version on GH Pages!

This is a simple 4 component React App which takes an array of Pokemon , divides them in two teams, and has them battle based on experience!
The method behind this was to render a "Pokegame" component in the App level. The Pokegame is the one containing the most state, this is where I stored the total EXP points,
calculated with a reducer function for each "pokehand," where the total exp is added up and then later displayed.

The Pokegame component passes down a couple of props to the Pokedex component below, including isBattling(whether or not the cards in the deck were still "shuffling"), pokemon(the prop that was passed as each of the pokemon in that specific hand),totalExp,
and finally isWinner(did this Pokedex end up having the higher EXP points).

Finally, we start getting to the less stateful components, Pokedex and Pokecard. These two components use the ternary operator to conditionally display 
green on all of the winning pokemon and red on all of the losing pokemon. I like using the ternary operator in my react render methods to to quickly get my logic up and running!
