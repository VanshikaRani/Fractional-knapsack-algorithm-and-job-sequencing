# Fractional-knapsack-algorithm-and-job-sequencing

Fractional Knapsack Problem Solution

This Java code solves the Fractional Knapsack problem using a greedy algorithm.

*Key Steps:*

1. *Sort items by value-to-weight ratio*: Sort items in descending order based on their value-to-weight ratio (`value/weight`).
2. *Iterate and take items*: Iterate through sorted items and take as much as possible (up to `W` capacity) of each item.
3. *Calculate total value*: Add the value of taken items to `totalValue`.

*Code Highlights:*

- `Item` class represents an item with `weight` and `value`.
- `getMaxValue` method sorts items and calculates maximum value.
- `main` method demonstrates usage with example items and capacity (`W = 50`).


Job Sequencing Problem Solution

This Java code solves the Job Sequencing problem using a greedy algorithm.

*Key Steps:*

1. *Sort jobs by profit*: Sort jobs in descending order based on their profit.
2. *Find maximum deadline*: Find the maximum deadline among all jobs.
3. *Create slot array*: Create an array to keep track of available time slots.
4. *Assign jobs*: Iterate through sorted jobs and assign each job to the latest available time slot before its deadline.

*Code Highlights:*

- `Job` class represents a job with `id`, `deadline`, and `profit`.
- `jobSequencing` method sorts jobs, assigns them to time slots, and calculates total profit.
- `main` method demonstrates usage with example jobs.



This means the selected jobs are Job1, Job2, and Job5, with a total profit of 134.

*How it works:*

- Job1 (deadline 2, profit 100) is assigned to slot 1.
- Job3 (deadline 2, profit 27) is skipped (slot 1 is taken).
- Job4 (deadline 1, profit 25) is skipped (slot 0 is taken by Job2).
- Job2 (deadline 1, profit 19) is assigned to slot 0.
- Job5 (deadline 3, profit 15) is assigned to slot 2.

