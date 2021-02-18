# Sampling from High Dimensional Space

Python program for sampling from high dimensional space with complex, non-linear constraints. The program provides a choice of selecting one from the following four methods

1) Sequential Monte Carlo (SMC)
2) Gibbs Sampler (Gibbs)
3) Adaptive Metropolis (AdaptiveMetropolis)
4) Metropolis Random Walk (Metropolis)

The choice of the method can be provided as the input while running the program and choice are provided in the brackets

### To use the Code:

#### Required python packages to run the code

* numpy
* matplotlib
* tqdm
* scipy
* seaborn

#### Input file format

```
#Dimension of the problem
2
#Initial starting point
0.0 0.0
# Constraints start from herr
1.0 - x[0] - x[1] >= 0.0
```

#### To use the package

1. Paste the input file inside the code folder
2. Open the terminal and go to the code colder
3. To sample from the space with the nonlinear constraints, run below arguments

      ``` python sampler.py <input file> <output file> <nsamples> <method: optional> ```
  
      Eg: ```python sampler.py mixture.txt mixture_out.txt 1000 SMC```

4. The optional method is provided as input at the end of the arguments. If the method is not mentioned, sequential Monte Carlo (SMC) will be selected as the default choice.
5. The results and plots will be generated in the results folder
