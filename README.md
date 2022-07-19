# AcceleratedBA
Implementation of an accelerated version of the Blahut Arimoto algorithm.
A full description of the algorithm and its steps are provided in the attached notebook.

On each iteration we perform the two following calculations:

![alt text](https://github.com/DorTsur/AcceleratedBA/blob/main/ba_alg_steps.png)

The algorithm is implemented in python, by constructing a trainer class that has initialization, channel matrxi construction, training and visualization methods.

I've decided to visualize the results by evaluating several metrics.

1. The mutual information induced by the current PMF vs. iteration:

![alt text](https://github.com/DorTsur/AcceleratedBA/blob/main/MI_ba_alg.png)

2. The [total variation](https://en.wikipedia.org/wiki/Total_variation_distance_of_probability_measures) distance between input PMFs on two conseccutive iterations:

![alt text](https://github.com/DorTsur/AcceleratedBA/blob/main/TV_ba.png)

3. The [KL divergence](https://en.wikipedia.org/wiki/Kullback%E2%80%93Leibler_divergence) between input PMFs on two conseccutive iterations:

![alt text](https://github.com/DorTsur/AcceleratedBA/blob/main/KL_ba.png)
