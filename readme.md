# Sudoku solver

## Introduction:

[According to Guinness World Records, the fastest time to complete a “Very Easy” difficulty Sudoku puzzle was 1 minute 23.93 seconds.](https://sudoku.com/how-to-play/who-has-the-guinness-world-record-for-fastest-sudoku-player/#:~:text=According%20to%20Guinness%20World%20Records,Snyder%2C%20an%20American%20Sudoku%20champion.) There are people who have beaten this record, some of whom can be found on the [enjoysudoku forum.](http://forum.enjoysudoku.com/did-i-just-break-the-world-record-of-speed-sudoku-t35563.html). 
The record for a computer solving a standard 9x9 sudoku puzzel of any difficulty is in the nano seconds (so quick our timmers return 0.0), but this wasnt always true. To solve a standard 9x9 sudoku puzzel you would need to 1: fill every cell of the puzzel, 2: each row must have 9 unique numbers, 3: each column must have 9 unique numbers from 1-9, 4: each Box in must have 9 unoque numbers from 1-9. given these contratints solving a standard sudoku puzzel with a computer in a brute force way would take a long time, given that it would pick a number between 1-9 for each empty square in the puzzel; we can expect to have 9^(number of empty squares) number of actions. 

for a puzzel like the one below:

<img src="images/sudoku.png" style="width: 50%;"/>


we would expect the computer to do $9^{n}\ checks,\ where\ n\ is\ the\ number\ of\ empty\ cells\ $ With brute force this solution ma take years to come, which is musch clower than a human. With the ues of AI concepts, backtracking, constraints propagation and searching we are able to drastically redues the time taken to solve the sudoku in figure1.

