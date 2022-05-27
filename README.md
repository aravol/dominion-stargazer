# Dominion Stargazer
Stargazer Card Randomizer for the Dominion card game.

This will use a nodemap of card synergies to construct high combo sets; as nodemaps often resemble star constellations, it has been nicknamed Stargazer.

## Compilation
Compilation will include building a database from the [Dominion Strategy Wiki](http://wiki.dominionstrategy.com/index.php/Main_Page) by parsing notes on known card synergies.

## Execution
Execution will draw a set of 10 to 14 cards, based on the following parameters
* Seeds
  * Seeds are the starting cards from which synergetic cards are drawn
  * Seeds may be drafted; that is, set manually
  * Number of seeds may vary from 1 to 4
  * Random seeds may be set to non-synergies
  * Random seeds may be set to minimum distance from each other per Djikstra algorythm
* Requirements
  * Requirements affect the drafting algorythm by creating zero-distance searches
  * Requirements are checked after draw and may trigger a redraft from the same, original parameters
  * Attacks require Reactions, Attacks require Moat, Minimum number of potions, etc
