# K-Mean Clustering
#MachineLearning 
Let $C_1,...,C_K$ be a set of observations
**Assumptions**:
- Each observations belongs to at least one cluster
- Each observations belongs to at most one cluster

Given a data set, define $K$ and $W(C_{k})$, and apply
$$\text{minimize for }C_1,...,C_{k}\{\sum_{k=1}^{K}{W(C_{k})}\}$$
where $W(C_{k})$ for the squared Eculidian distance is the sum of inertia of all clusters:
$$\text{--INSERT MATH FUNCTION FROM NOTES HERE--}$$

### Algorithm
*The number of clusters the algorithm will work on must be defined beforehand*
1. Randomly assign a number, from I to K, to each of the observations (they'll serve as the initial cluster assignments).
2. Iterate until cluster assignments stop canging:
	1. For each of the K clusters, compute the cluster *centroid*
	2. Assign each observation to the vluster whose centroid is closest (due to chosen metric)
