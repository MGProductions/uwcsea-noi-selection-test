
# TASK 1: Eat Your Vegetables

## Statement

Mihir hates eating his vegetables, but for the good of his health, his parents force him to eat vegetables. After the great revolt in his house (against eating vegetables of course), he and his parents came up with a compromise - Mihir would have to eat exactly `K` vegetables to satisfy his nutritional requirements from a plate of `N` vegetables. His parents insisted on choosing all the vegetables he ate, but fearing another revolt, his parents and he now alternatate between choosing the vegetables. His parents pick the first vegetable, then he picks the second, then his parents pick the third, and so on, until K vegetables are picked and eaten. 

Every vegetable has a nutritional value `V[i]`. His parents still don't think that he's getting the nutritional value he needs to be playing all the sports he plays. For this reason, his parents always choose the vegetable with the highest nutritional value (`V[i]`) which is still uneaten, and asks him to eat it. 

Mihir is intelligent, and sensing his parents' plan, he does the opposite - every time he gets to pick a vegetable, he picks the one with the lowest nutritional value (`V[i]`) and eats it.

Today, he wants to find out the total nutritional value he will gain from eating the `K` vegetables. More formally, given `V`, the list of nutritional values, and `K`, the number of vegetables he must eat, find out the total nutritional value of his meal.

## Input format

The first line contains two space-separated integers, `N` and `K`. `N` represents the number of vegetables on the plate, and `K` represents the number of vegetables Mihir must eat.

The second line contains `N` space-separated integers, each integer corresponds to the nutritional value of a vegetable on the plate - representing `V[i]` for each `i`.

## Output format

Print one single number, representing the total nutritional value of the vegetables Mihir will eat.

## Constraints

`K` will always be less than or equal to `N` (it will always be possible to select `K` vegetables).

Each nutritional value of a vegetable, `V[i]`, will satisfy `0 ≤ V[i] ≤ 1000`.

| Subtask # | Constraints | Points | Testcase number |
| --- | --- | --- | --- |
| 1 | N = 2, K = 1 | 5 | 0 |
| 2 | N = 2, K = 2 | 5 | 1 |
| 3 | N = 10, K = 2 | 10 | 2 |
| 4 | N = 100, K ≤ 100 | 10 | 3 |
| 5 | N = 100, K = 100 | 5 | 4 |
| 6 | N = 1000, K ≤ 1000 | 20 | 5 |
| 7 | N = 1000, K = 1000 | 10 | 6 |
| 8 | N = 1000000, K ≤ 1000000 | 35 | 7 |

## Sample Testcases

### Sample 1:

#### Input

```
2 1
4 5
```

#### Output

```
5
```

#### Explanation

Mihir must eat `1` vegetable from the two available. As his parents make the first pick and choose `5`, he ends up gaining a total nutritional value of `5`, so we print `5`.

### Sample 2:

#### Input

```
5 2
8 4 1 3 5
```

#### Output

```
9
```

#### Explanation

Mihir must eat 2 vegetables from the 5 provided. His parents make the first choice, and select the vegetable with nutritional value of 8. Mihir makes the second choice and picks the vegetable with nutritional value of 1. His total nutritional value gained is 8+1 = 9, so we print `9`.

### Sample 3:

#### Input

```
10 5
8 5 1 3 2 8 9 2 2 1
```

#### Output

```
27
```

#### Explanation

Mihir must eat 5 of the 10 vegetables. For this case:
 * His parents pick the vegetable with value 9,
 * He picks one of the vegetables with value 1,
 * His parents pick one of the vegetables with value 8,
 * He picks the other vegetable with value 1
 * His parents pick the other vegetable with value 8

In total, he gains 9 + 1 + 8 + 1 + 8 = 27 nutritional value, so we print `27`.
