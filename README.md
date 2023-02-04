double Q learning
maximization bias - uncertainty is actually a spread in the values and that spread causes it to have a some amount of positive bias.
the max of the true value is 0 but the max of the capital Q value is positive, hence a positive bias.

This happens because of using the same set of samples to determine the maximizing action as well as the value of that action.

One way to solve this problem is to use 2 seperate q functions to determine the max action and the value, set up a relationship between and alternate between them as you play the game to eliminate the bias over time.

