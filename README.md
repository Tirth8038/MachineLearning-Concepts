# MachineLearning-Intrinsic Dimensionality(ID)
The Intrinsic Dimensionality(ID) is theoretically exact in uniformly distributed datasets which provides consistent results in general. Even after running some test on estimating ID of a d-dimensional Hypercube using a sample size of 2500 uniform random data points, we observe (fig.(3a)) that for the large value of ‘d’ the Intrinsic Dimensionality becomes inaccurate.

Even though all the data generated here is uniform, the Two-NN technique results in less number of ID which depicts that certain features are not significant. 
However in this article, A dataset of sample size 2500 is drawn from uniform distribution on a hypercube in dimension ‘d’=14 is analyzed by Periodic Boundary Conditions (pbc). The hypercube with (pbc) is the Probability Distribution Function(pdf) that best resembles a uniform distribution on a linear space; nevertheless it has to be noticed that the (pbc) introduce correlations in the distances whenever the typical distance of the second neighbor is comparable with the box size
Here,  as the data for Hypercube ID testing is non uniform w.r.t linear space, the value of measured Intrinsic Dimensionality becomes overestimated due to lack of  Periodic Boundary Condition (pbc) and on Gaussian Two-NN, due to the presence of sharp boundaries.

The main cause of the measured ID to be inaccurate for large ‘d’ is in distributions characterized by heavy tails there is a significant probability of having r2>>r1 and a large value of the ratio r2/r1(cumulative distribution of the ratio of the second distance to the first one). Due to this, the fit is unstable. As a solution to make the procedure more robust, we can discard the 10% of the points characterized by highest values of μ from the fitting.

Moreover, what makes the notion of ID well defined is the stability of the measure with respect to changes in the scale of interest.But in Nearest Neighbors-Based ID estimators the reference scale is the size of the neighborhood involved in the estimation; this depends on the density of points in the sample and does not necessarily coincide with the scale of interest. So, the more data points are used for the estimate, the smaller the average distance of the second neighbor will become, and the larger the ID.

Hence, as the number of points grows, the noisy dimensions are also sampled, and the value of the estimated ID increases.
Intrinsic Dimensionality of ‘number 1’ and ‘number 2’ from the MNIST Dataset:
In this Article, the experiment was performed on ‘Number 2’ from the MNIST Dataset. Similarly, we can perform the experiment on ‘Number1’ with 2 various sample sizes of (300-500) and 1000 to analyze the result reported in the article. We found;

According to the result, an ID of ‘number 2’ for Sample size of (300-500) and 1000 is found about 11.358687 and 14.004677 respectively, which is close to the result shown with the help of graph in the Article.
Whereas, the ID of ‘number 1’ for Sample size of (300-500) and 1000 is found about 8.823548 and 11.569854 respectively.
Consider the graph (fig.3(c)) to analyze the behaviour of Intrinsic Dimensionality of number1 and number2 dataset.

        
Visualizing the graph, In the case of MNIST dataset for ‘number1’ and ‘number2’ the plateau is located in a range between 400 and 600 points, and the measure of the ID corresponding to the plateau is between the range of ‘8.5 to 10.5’ and ‘11 to 13.5’ respectively, which is almost similar to the result derived in the Article for ‘number2’.
Hence, we can also state that the test conducted on MNIST ‘number2’ is also congruent to the MNIST dataset ‘number1’.
