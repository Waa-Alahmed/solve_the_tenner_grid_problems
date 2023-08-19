# solve_the_tenner_grid_problems

# Description:
We can solve the tenner grid problems in many ways such as Backtracking and Backtracking
with MRV, forward checking, and more.

# First: Backtracking
In the beginning, the program assigns a random value from zero to nine so that it
fulfills the rules of the game in the first empty place. The search starts from the first
row, the first column, then the second row, the second column, until it reaches row n
column n. After he reaches the first empty place, he starts checking the available
values for the assignment, starting from zero to nine. If he finds a valid value and the
rules of the game are met, he returns true, and if he does not find a valid value for the
assignment, he returns false, then backtracks to the previous and changes the values
down to a solution that fulfills the rules for each game.

# Second: Backtracking with MRV
Like backtracking, the difference is in the process of choosing the place to start from.
The code first determines whether the filled method is true before it begins and since it
starts in the cell with the lowest probability and fills it first, its objective is to find the
minimum remaining value.

# Third: Forward Checking 
The forward checking method is a method that takes four parameters (grid, row, Column, possibilities) grid is 2 dominions array and
possibilities in three dimensions array and return a Boolean value that is true or false at first
check if the row is the last row and return false if the sum of the columns does not equal the
last row then check if the row was the second row and the column is out of bounds it will
return true it will go to for loop witch assigned the possibilities value to the cells then call the
method that update domain to its neighbors by using 3 dimension array that we received it
as a parameter after that it will call the forward checking method again and increments the
column and let it in if statements if it goes to the last cell and returns true that’s mean the
method find the solution otherwise it will update the neighbors and then unassigned the cell
and try another value
