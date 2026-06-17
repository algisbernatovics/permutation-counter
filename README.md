# Permutation Counter

A PHP command-line solution for counting permutations with exactly `k` inversions using dynamic programming.

## Learning Goal

Practice transforming a combinatorics problem into a tabular dynamic programming solution with predictable input/output handling.

## Problem

For each dataset, given `n` and `k`, count how many permutations of `1..n` contain exactly `k` inversions. An inversion is a pair `(i, j)` where `i < j` and `a[i] > a[j]`.

## Approach

The program builds `dp[i][j]`, where `i` is the permutation length and `j` is the inversion count. Each state sums valid counts from the previous length.

## Complexity

- Time: `O(n * k * n)` with the current nested-loop recurrence.
- Space: `O(n * k)` for the DP table.

## Example

```text
Input
1
4 1

Output
3
```

## Tech Stack

- PHP
- CLI input/output
- Dynamic programming

## Run

```bash
php app/count_permutations.php
```

## Project Structure

- `app/count_permutations.php` - solver and CLI entry point

## License

MIT License. See [LICENSE](./LICENSE).
