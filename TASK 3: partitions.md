
# TASK 3: Increasing Sequences

## Statement

Soumyaditya Choudhuri is well-renowned as a good mathematician. When thinking about numbers, he thinks of a problem. For a number `N`, he wants to find the number of strictly increasing arrays that add to `N`. For example, `[1,3,6]` is a valid array for `N=10`, but `[3,6,1]`, `[1,4,6]`, and `[3,3,4]` are not. He wants to do this `T` times.

Given `T` integers `N`, can you find the number of strictly increasing arrays that add up to `N`. As the answer can be very large, output the answer modulo `10^9+7`.

Note: all the numbers in the array must be **positive**.

## Input format

On the first line, one integer `T`.

`T` space-separated integers on the second line, the `i`th one corresponds to the `i`th value of N.

## Output format

`T` space-separated integers, the `i`th one corresponds to the output for the  `i`th value of `N`.

## Constraints

| Subtask # | Constraints | Points | Testcase number |
| --- | --- | --- | --- |
| 1 | T=4, N<=4 | 15 | 0 |
| 2 | T=20, N<=20 | 20 | 1 |
| 3 | T=200, N<=200 | 30 | 2 |
| 4 | T=2000, N<=2000 | 35 | 3 |

## Sample Testcases

### Sample 1:

#### Input

```
1 4
```

#### Output

```
2
```

#### Explanation

The following partitions are valid for this: `[1, 3]` and `[4]`. Therefore, we output `2`.

 * Note that `[0, 4]` is **not** valid as `0` is not positive.
 * Note that `[2, 2]` is **not** valid as the array is not strictly increasing.
 
### Sample 2:

#### Input

```
2 4 5
```

#### Output

```
2
3
```

#### Explanation

The first query is the same as the last testcase.

The following partitions are valid for this case:
 * `[5]`
 * `[1, 4]`
 * `[2, 3]`
