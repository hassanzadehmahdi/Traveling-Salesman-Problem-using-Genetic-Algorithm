# Traveling-Salesman-Problem-using-Genetic-Algorithm
Genetic algorithms are heuristic search algorithms inspired by the process that supports the evolution of life. The algorithm is designed to replicate the natural selection process to carry generation, i.e. survival of the fittest of beings. Standard genetic algorithms are divided into five phases which are: 
 

    1.Creating initial population.
    2.Calculating fitness.
    3.Selecting the best genes.
    4.Crossing over.
    5.Mutating to introduce variations.

These algorithms can be implemented to find a solution to the optimization problems of various types. One such problem is the Traveling Salesman Problem. The problem says that a salesman is given a set of cities, he has to find the shortest route to as to visit each city exactly once and return to the starting city. 
Approach: In the following implementation, cities are taken as genes, string generated using these characters is called a chromosome, while a fitness score which is equal to the path length of all the cities mentioned, is used to target a population.
Fitness Score is defined as the length of the path described by the gene. Lesser the path length fitter is the gene. The fittest of all the genes in the gene pool survive the population test and move to the next iteration. The number of iterations depends upon the value of a cooling variable. The value of the cooling variable keeps on decreasing with each iteration and reaches a threshold after a certain number of iterations.

### Algorithm: 
 

      1. Initialize the population randomly.
      2. Determine the fitness of the chromosome.
      3. Until done repeat:
          1. Select parents.
          2. Perform crossover and mutation.
          3. Calculate the fitness of the new population.
          4. Append it to the gene pool.


### Pseudo-code: 
 
        Initialize procedure GA{
            Set cooling parameter = 0;
            Evaluate population P(t);
            While( Not Done ){
                Parents(t) = Select_Parents(P(t));
                Offspring(t) = Procreate(P(t));
                p(t+1) = Select_Survivors(P(t), Offspring(t));
                t = t + 1; 
            }
         }
         

An example of running the program:


![222](https://user-images.githubusercontent.com/45950266/153172517-3a157d43-1521-4b81-afc1-6bf7cc53ff4f.png)

         
The description was from geeksforgeeks website.
