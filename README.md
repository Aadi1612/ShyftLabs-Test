# ShyftLabs Assignment

## Problem Statement
You are given an unbounded array, which contains positive integers and -1. After a certain index x, all the elements are -1. You need to find this index x.

For example:
- Input: 3, 4, 1, 2, 7, 8, 20, 33, -1, -1, -1, -1
  Output: 8
- Input: -1, -1, -1, -1
  Output: 0

### Constraints
- The array will always have -1 at some index.
- The array will never be empty.
- Once -1 appears, a positive integer will never appear.

## Approach
We can solve this problem efficiently using binary search. The algorithm works as follows:
1. Initialize `low` to 0 and `high` to 1.
2. Double `high` until we find a value of -1.
3. Apply binary search between `low` and `high` to find the exact index of the last positive integer.

## Implementation
The solution is implemented in Python. It takes input from the user and uses binary search to find the index of the last positive integer.

## Usage
1. Clone the repository.
2. Run the Python script `find_index.py`.
3. Enter the array separated by commas when prompted.
4. The script will output the index of the last positive integer.
