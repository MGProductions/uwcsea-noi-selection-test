
# TASK 4: Azuki and Game

## Statement

Azuki is scared of being the main character again in the upcoming NEKOPARA Volume 4 video game. Lucky for her, NEKOPARA's developer team are kind and let her play a game to determine if she will be the main character. (Yes, video game characters in NEKOPARA are sentient and communicate regularly with their developer team, headed by the great Santi Cazorla. One would ask why the devs don't swap them out for non-sentient characters and save the hassle, but apparently having sentient characters provides more realism ... is what they tell their investors. Really, they just feel uneasy about killing even virtual characters.)

The game works like so: Azuki is given an integer array `A` (A for Azuki!) with length `N`. She has to choose indices of the array to form a sequence of length `k`. The elements at these indices must be strictly non-decreasing (i.e. where S is the sequence, `A[S[0]] >= A[S[1]] >= A[S[2]] >= … >= A[S[k-1]]`.) Note that indices of the sequence may be repeated (e.g. `0` may be used twice). The score Azuki gets is the minimum difference in indice between adjacent elements of the sequence (i.e. `min(|S[0]-S[1]|, |S[1]-S[2]|, … , |S[k-1]-S[k]|)`. ) If she gets a high enough score, she does not have to be main character. Azuki does not want to cheat, so she will play the game by herself, however she needs to be sure that the developers are not scamming her by giving her a game she cannot win. Therefore, she asks you this: what is the maximum possible score she can get? If the developers are mega-cheat and there is no way for her to make any sequence of length `K`, output -1.

Azuki promises, if you help her, she will bake you a delicious cake.

## Input format

On the first line, two space-separated integers `N` and `k`. On the second line, the elements of array `A`, space-separated, in order (`A[0] A[1] … A[N-1]`).

## Output format

One integer, the maximum possible score Azuki can get, or `-1` if it is impossible to form any valid sequence.

## Constraints

| Subtask # | N | Other Constraints | Points | Testcase numbers |
| --- | --- | --- | --- | --- |
| 1 | <=200 | A[0]>A[1]>...>A[N-1] | 3 | 0-4 |
| 2 | <=200 | A[0]>=A[1]>=...>=A[N-1] | 5 | 5-7 |
| 3 | <=200 | All elements of `A` are distinct. | 15 | 8-10 |
| 4 | <=200 | None. | 10 | 11-13 |
| 5 | <=2000 | All elements of `A` are distinct. | 18 | 14-17 |
| 6 | <=2000 | None. | 14 | 18-20 |
| 7 | <=100,000 | All elements of `A` are distinct. | 24 | 21-23 |
| 8 | <=100,000 | None. | 11 | 24 |

Note that for each subtask in addition to the testcases given you should also correctly solve all prior testcases within the same constraints to get the points.

## Sample Testcases

### Sample 1:

#### Input

```
5 3
7 3 8 5 1
```

#### Output

```
2
```

### Sample 2:

#### Input

```
6 4
8 4 3 5 2 7
```

#### Output

```
3
```
