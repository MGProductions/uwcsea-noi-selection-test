# TASK 2: Odd or Even

## Statement

Jishnu is planning to build a city. The city can be represented as a graph with `N` locations - which are houses, airports, shopping malls or tourist attractions of some kind. There are `N-1` roads which connect some pair of locations. There are no one-way roads, so a road from `A` to `B` with weight `D` means that there is also a road of equal weight `D` from `B` to `A`. It is only possible to travel between locations by using roads, but it is also guaranteed that it is possible to travel from any location to another one using some sequence of 1 or more roads.

This city is futuristic, so it will have a bus service which is one of a kind. The bus service does not care about how far you travel - or more accurately, it only cares about the parity of the distance you travel. Essentially, the bus service charges you $1 if you travel an odd distance, or $0 if you travel an even distance.

Jishnu wants to make the city as economical to travel as possible, but the first step to doing that is finding out the cost of `Q` existing journeys by bus. Each query will have two locations, `A` and `B`. For each journey, print out whether the service will charge you $1 or $0 (without the `$` sign).

## Input format

All locations are numbered from `1` to `N` (1-indexed, not 0-indexed).

The first line will contain `N`, the number of locations on the graphs.

The next `N-1` lines will contain three space separated integers, `A`, `B` and `D`. `A` and `B` represent the locations connected by a road, and `D` represents the distance between these two locations (or the length of this road).

The next line will contain another integer, `Q`, representing the number of queries. 

The next `Q` queries contain two space separated integers, `A` and `B`.

## Output format

For each query of `A` and `B`, print out `1` if the distance is odd, or `0` if the distance is even. Please do so on new lines for each query. Refer to the sample output for more details.

## Constraints

| Subtask # | Constraints | Points | Testcase number |
| --- | --- | --- | --- |
| 1 | N = 2, Q = 1 | 5 | 0 |
| 2 | N = 10, Q = 1, and the graph can be represented as a line graph. | 5 | 1 |
| 3 | N = 500, Q ≤ 1000 | 10 | 2 |
| 4 | N = 500, Q ≤ 1000, and all road lengths will be `2`. | 10 | 3 |
| 5 | N = 1000, Q ≤ 1000 | 20 | 4 |
| 6 | N = 1000000, Q ≤ 1000000 | 20 | 5 |
| 7 | N = 1000000, Q ≤ 1000000, and all road lengths will be `2`. | 10 | 6 |
| 8 | N = 10000000, Q ≤ 10000000 | 20 | 7 |


## Sample Testcases

### Sample 1:

#### Input

```
2
1 2 5
1
1 2
```

#### Output

```
1
```

#### Explanation

There are two locations, `1` and `2`. These locations are connected by a road of length `5`. As `5` is odd, we output `1` to the console.

### Sample 2:

#### Input

```
3
1 2 5
1 3 3
2
1 3
2 3
```

#### Output

```
1
0
```

#### Explanation

There are three locations, `1`, `2` and `3`.

For the first query, `1` and `3` are connected by a road of length `3`, which is odd, and `1` is output.

For the second query, `2` and `3` are connected indirectly via a road of length `5` (connecting `1` and `2`) and another road of length `3` (connecting `1` and `3`). `5`+`3` is even, so we print `0`.



