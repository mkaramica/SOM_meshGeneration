# SOM_meshGeneration
Implementation of self-organizing maps for mesh generation

The implementation of the self-organizing maps (SOMs) for mesh generation is investigated for 2-D geometries. For the SOM implementation, the positions of the winner neurons are modified continuously over iterations based on their lateral coefficient (related to how much they are close to the introduced datapoint) as well as the learning rate which is gradually decreasing during the iterations. For rectangular domains, two independent standard variables are engaged for mesh generation. The boundary nodes are fixed while the positions of the internal neurons are modified based on the selected random points from the domain introduced to SOM at each iteration. The nonuniform mesh distribution is obtained by applying some mathematical modifications on the probability functions. For domains with an arbitrary shape, the datapoint are selected from the domain by picking them from a pre-defined probability distribution function, which is achievable by either inverse method or rejection method. Some samples for uniform and nonuniform mesh distributions are provided for simply connected geometries as well a domain with a hole inside to show the capability of SOM for mesh generation.

All MATLAB scripts are attached (as a zipped file).

There is a text file, named 'domain_notSorted.txt', which is used as an arbitrary domain shape to implement the algorithm on.

For calculating the results regenerating the figures, please follow the following steps:

1- All the figures can be obtained by running the corresponding scripts.
2- To regenerate figure 29 to 38, the domain shape should be stored in "domain_notSorted.txt" file. This file should be located in the same folder as the figures script are running. There is no need to sort the domain boundary.
3- The simulations for arbitrary-shape domain are time-demanding due to the required time to generate the distribution functions. 
4- The script 'figure31_32.m' requires file 'rndDomain.mat' which is created by 'figure30.m'. The user need to activate Line#50 of 'figure30.m' to let the script generate and save the required PDF which is mandatory for 'figure31_32.m'.
5- The script 'figure34_35.m' requires file 'rndDomain_density' which is created by 'figure33.m'. The user need to activate Line#94 of 'figure33.m' to let the script generate and save the required PDF which is mandatory for 'figure34_35.m'.
6- The script 'figure37_38.m' requires file 'rndDomainHallow.mat' which is created by 'figure36.m'. The user need to activate Line#50 of 'figure36.m' to let the script generate and save the required PDF which is mandatory for 'figure37_38.m'.
