# CAC-Compression
Optimization for Constant Area Coding compression method using :dna: Gentic Algorithm
## Method 
Genetic Algorithms (GA) optimize the kernel size for compressing binary images. By evaluating different kernel sizes based on compression quality, GA finds the optimal size. It iteratively applies genetic operations, evaluates fitness, and selects individuals until convergence. GA is an effective method to enhance binary image compression by finding the best kernel size.



## Steps:

- Chromosome structure:
Window size in binary format where the bigger dimension is the number of bits for a single chromosome
i.e 400w x 200h 
110010000 x 11001000
9 bits x 8 bits
chromsome = 18 bits where the first half is the width and the other is the height


- GA:
Randomly initialize Populations
Evolution: Determine fitness of Population and ranking them

Repeat:

Select Mating Pools (Parents) from Populations
Perform crossover on Mating Pools resulting Offsprings
Perform mutation on Offsprings resulting Mutants
Set Mutants as the next generation Populations
Evolution: Determine fitness of Population and ranking them

Until Exit Condition

May be:

Reach maximum number of generations
Reach to a solution is good enough (Δ Error Convergence)



- Compression ratio:
Cr = n1 / n2
where :
    n1 --> number of bits in orginal image
    n2 --> number of bits in compressed image
