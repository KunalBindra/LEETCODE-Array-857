# LEETCODE-Array-857
This code implements a solution to the "Minimum Cost to Hire K Workers" problem. It calculates the minimum total cost to hire K workers, where each worker has a certain quality and expects a certain wage. The idea is to select K workers with the minimum ratio of wage to quality while ensuring that the total quality of the selected workers is at least K.

Let's consider an example:

```java
int[] quality = {10, 20, 5};
int[] wage = {70, 50, 30};
int k = 2;
```

1. For the first worker, wagePerQuality = 70/10 = 7.
2. For the second worker, wagePerQuality = 50/20 = 2.5.
3. For the third worker, wagePerQuality = 30/5 = 6.

The sorted array of workers based on wagePerQuality: [(2.5, 20), (6.0, 5), (7.0, 10)].

Now, iterate through the sorted workers:

- Select the first worker with quality 20. Total quality = 20.
- Select the second worker with quality 5. Total quality = 25. Total cost = 25 * 2.5 = 62.5.

Thus, the minimum cost to hire 2 workers is 62.5.
