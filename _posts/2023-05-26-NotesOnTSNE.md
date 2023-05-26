# NotesOnTSNE
T-distributed Stochastic Neighbour Embedding (T-SNE) is a tool used to visualise high dimensional data in two or three dimensional scatter plot such that similar data points will be nearby each other, and dissimilar data will be more distant. For our purposes, we will be only considering the two-dimensional plot.  
Avoiding most of the math, I will try and put the steps of creating a T-SNE plot simply. 
1.	Pairwise similarities are calculated, creating a similarity matrix – this may be done in a variety of ways including Euclidean distance. 
2.	Initialise embedding of data points onto the 2D scatter plot – at this point, the embedding does not tell us anything. 
3.	Use a Gaussian distribution to create a similarity distribution in the 2D space that matches the high dimensionality similarity distribution. 
4.	Adjust the embedding iteratively to improve the replication of the similarity distribution of the high dimension onto the 2D.  Do this until the embedding converges to a solution. 

Throughout this process, a given perplexity aids in the adjustment of the embedding. This perplexity is not calculated but given and reflects the amount of points that should neighbour a data point. 

T-SNE plots are a great way to visualise high dimensional data, but can also be misleading depending on the given perplexity, learning rate and iterations. This is greatly discussed <a href="https://distill.pub/2016/misread-tsne/"> here </a>, but to summarise, perplexity should be within a 5-50 range, and the step size and iterations should be set such that the final plot is a stable configuration.  

