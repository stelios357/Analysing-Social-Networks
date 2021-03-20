# Analysing-Social-Networks
Social Network Analysis
 
Department of Computer Science Engineering
The LNM Institute of Information Technology, Jaipur


DATASET DESCRIPTION

Dataset 1: Caenorhabditis elegans (metabolic)
The statistics for the the dataset is given below:

Size
 n=453
Volume 
 m=2025
Loop Count
 l=0
Wedge Count
 s=79173
Claw Count
 z=3352172
Cross Count
 x=153983040
Triangle Count
 t=3284
Square Count
 q=50289
Maximum Degree
 dmax=237
Average Degree
 d=8.94040
Fill
 p=0.0197796
Diameter
 δ=7
50- percentile effective diameter
 δ0.5=2.14350
90- percentile effective diameter
 δ0.9=3.16935
Median distance
 δM=3
Mean distance
 δm=2.67627
Gini Coefficient 
 G=0.494803
Balanced Inequality Ration
P=0.321481
Relative edge distribution entropy
Her=0.898264
Power law exponent
Y=1.56569
Tail power law exponent
Yt=2.63100
Tail power law exponent with p
Y3=2.63100
p-value
p=0.0470000
Spectral norm
𝛼=26.3085
Algebraic connectivity
a=0.258000
Non-bipartivity
bA=0.429332
Normalized non-bipartivity
bN=0.200551
Algebraic non-bipartivity
X=0.293557
Spectral bipartite frustration
bK=0.00820872
Controllability
C=7
Relative controllability
Cr=0.0154525






Graph (visual) for Dataset 1:





Dataset 2: Jazz Musicians
The statistics for the the dataset is given below:

Size
 n=198
Volume 
 m=2742
Loop Count
 l=0
Wedge Count
 s=103212
Claw Count
 z=1583352
Cross Count
 x=21666963
Triangle Count
 t=17899
Square Count
 q=406441
Maximum Degree
 dmax=100
Average Degree
 d=27.6970
Fill
 p=0.140594
Diameter
 δ=6
50- percentile effective diameter
 δ0.5=1.64700
90- percentile effective diameter
 δ0.9=2.79355
Median distance
 δM=2
Mean distance
 δm=2.20604
Gini Coefficient 
 G=0.345989
Balanced Inequality Ration
P=0.373450
Relative edge distribution entropy
Her=0.961549
Power law exponent
Y=1.32928
Tail power law exponent
Yt=5.27100
Tail power law exponent with p
Y3=5.27100
p-value
p=0.610000
Spectral norm
𝛼=40.0274
Algebraic connectivity
a=0.571994
Non-bipartivity
bA=0.782583
Normalized non-bipartivity
bN=0.460437
Algebraic non-bipartivity
X=0.692773
Spectral bipartite frustration
bK=0.00625314
Controllability
C=1
Relative controllability
Cr=0.00505051








Graph (visual) for Dataset 2:








NETWORK DESCRIPTION

Dataset 1: Caenorhabditis elegans (metabolic)
This  metabolic network represents the metabolic pathways in 43 organisms.
The nodes represent the substrate and the edge between two nodes represent existence of a metabolic reaction between them.
The network is unipartite and edges are undirected.
The edges are not weighted and the network has no multiple edges.
The given network has no loops.
Code Notebook for Dataset 1

Dataset 2: Jazz Musicians
This network is a collaboration network between Jazz musicians.
The nodes represent the musicians and the edge between two nodes represent that the two musicians have played together in a band.
The network is unipartite and edges are undirected.
The edges are not weighted and the network has no multiple edges.
The given network has no loops.
Code Notebook for Dataset 2
CENTRALITY MEASURES STUDIED
Degree Centrality: 
Degree Centrality measures the importance of a node with respect to its degree. It is a good centrality measure when the goal is to find connected, popular individuals or those who are probably going to hold more information in a network.

Degree Centrality of Dataset 1
Degree Centrality of Dataset 2

Eigenvector Centrality:
Eigenvector centrality generalizes degree centrality. The general idea is: Having more important friends (incoming edge in case of a directed graph) also makes me important.Eigenvector centrality is a good measure for understanding human social networks.

Eigenvector Centrality of Dataset 1
Eigenvector Centrality of Dataset 2


Katz Centrality:
The eigenvector centrality proves to be a bad centrality measure in the special case of a directed acyclic graph where the centrality becomes zero even though the node may have many edges. We add a bias term 𝛃 to all the nodes which is added to the centrality measure of all nodes irrespective of how they are placed in a network.

Katz Centrality of Dataset 1
Katz Centrality of Dataset 2

Pagerank Centrality:
Pagerank centrality measure is a well known and widely used measure. The major issue with Katz Centrality is that once a node becomes central, it passes its centrality along all of its outlinks, but this is not ideal in the real world sometimes as not everyone known by a popular individual is also popular. This centrality measure can be very helpful to study citations and authority as it takes the edge direction and connection weight into account.

Pagerank Centrality of Dataset 1
Pagerank Centrality of Dataset 2
Betweenness Centrality:
Till now all the centrality measures we discussed, talked about node centrality with respect to the structure of the network but betweenness centrality measures the importance of a node in terms of connecting other nodes via path connections. This measure can be very helpful to study which individuals influence flow in a system.

Betweenness Centrality of Dataset 1
Betweenness Centrality of Dataset 2

Closeness Centrality:
According to this centrality measure, important nodes are the ones from where we can reach other nodes in the network more quickly, that is, the nodes with the smallest average path length to other nodes. 

Closeness Centrality of Dataset 1
Closeness Centrality of Dataset 2




CLUSTERING COEFFICIENT OF DATASETS
Clustering Coefficient is a measure of transitivity. It also gives us an idea about whether the network is sparse or dense.

Local Clustering Coefficient:
Local clustering Coefficient measures a given nodes’ neighbors’ level of connectivity. It varies in the range between 0 and 1. It represents transitivity for a given node. 

Local Clustering Coefficient of Dataset 1
Local Clustering Coefficient of Dataset 2

Global Clustering Coefficient:
It measures the transitivity of the entire network. 

Global Clustering Coefficient of Dataset 1:
0.12443636088060324

Global Clustering Coefficient of dataset 2:
0.5202592721776538
RELEVANT CENTRALITY MEASURES

Dataset 1: Caenorhabditis elegans (metabolic)
Degree Centrality: As the dataset contains metabolic reactions in between multiple substrates, degree centrality would help us to understand the reactive nature of the substrate. Immediate neighbours are of more importance rather than neighbours of neighbours.

Dataset 2: Jazz Musicians
Degree Centrality: In collaborative networks such as this Jazz Network, degree centrality is relevant as the nodes with high degree centrality will help us find famous and popular Jazz musicians that have collaborated with the most number of musicians.

Closeness Centrality: The closeness centrality of the Jazz network tells us how close a musician is to other musicians in the network. This gives us information about the independence and autonomy of the musician. 
INFERENCES

Dataset 1: Caenorhabditis elegans (metabolic)
It is observed that the node designated as ‘3’ has the highest Degree Centrality (0.52433). This shows it is the most reactive substrate.
It is observed that the node designated as ‘3’ has the highest Eigenvector Centrality (=0.3799). This shows that it is connected to many substrates who are themselves reactive.
It is observed that the nodes designated as ‘7’ and ‘8’ have the highest Katz Centrality (=0.2097). This shows that these nodes have the highest influence over other nodes in the graph.
It is observed that the node designated as ‘3’ has the highest Pagerank Centrality (=0.0550). This shows that it is important because it is connected to the other important nodes.
It is observed that the node designated as ‘3’ has the highest Betweenness Centrality (=0.4783). This shows that this substrate comes in between the maximum number of metabolic pathways between any other two nodes.
It is observed that the node designated as ‘3’ has the highest Closeness Centrality (=0.6541). This shows that it is closest to every other node, i.e. has the least sum of metabolic paths to every other node.
There are 109 nodes with local clustering coefficients equal to 1. This means that all their neighbours can react among each other.
Transitivity determines how close the networks are to being complete. We measure it with clustering coefficients. The global clustering coefficient came out to be 0.124436, which shows that the network is more on the incomplete side, rather than complete.
Average clustering coefficient is 0.6464, which shows that either majority of the nodes have high clustering coefficient, or some have extremely high clustering coefficients.
The reciprocity is found to be 0. This is to be expected as there are no closed cycles of length 2 in the network since it is undirected.

Dataset 2: Jazz Musicians
It is observed that the node designated as ‘67’ has the highest value of degree centrality and betweenness centrality among all nodes in the graph. This means that node ‘67’ has the highest degree in the graph.
Since the betweenness centrality is also highest among all nodes, this means that node 67 is well connected and lies on the shortest path of the most number of node pairs.
The highest betweenness centrality is just 0.151. Thus we can infer that there are not many bridge like nodes in this graph.
Node 7 has the highest eigenvector centrality among all nodes, implying that it is connected to the most central nodes in the graph.
The node 158 has a local clustering coefficient of 1. This means that all of the neighbours of node 158 are completely connected and have an edge between each other.
The reciprocity is 0, which is to be expected as there are no closed cycles of length 2 in our graph as the graph is undirected.
The node 67 has the highest closeness centrality. This means that node 67 has the shortest distance to all of the other nodes.
The average clustering coefficient is greater than 0.5. This means that there are more nodes with high clustering coefficients or that some nodes have extremely high clustering coefficients.
Since transitivity can be defined as the probability that the neighbours of a node are interconnected and given the transitivity of our graph is  0.52, we can say that 52% of the nodes in the graph will have interconnected neighbors.
PROBLEM 2: Try to get an algorithm package in Python to find the maximum connected component (called a giant component in the class) in a given graph G. Let us denote the number of nodes in the giant component of a graph G as N_G. Vary ⟨k⟩ from 0 to 5 with increment of 0.1. For each value of ⟨k⟩ find the ratio N_G/N where N is the number of nodes in the graph. Plot this ratio with respect to ⟨k⟩. Take ⟨k⟩ as x-axis and ratio N_G/N as y-axis.
Code Notebook



The required datasets are imported.
Networkx: NetworkX is a Python package for the creation, manipulation, and study of the structure, dynamics, and functions of complex networks.
Matplotlib: Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python.



We are assuming/taking N = 1000, then we made an empty list for degree and Ng/N.
Then the while loop increments k (average degree) at an interval of 0.1 from 0 to 5.



Inside the while loop we append the same degree k to all nodes and pass it through the function expected_degree_graph, which takes a list as a parameter and we have to pass the degree of all nodes in this case k. It gives a random graph G as an output with average degree k.



For connected components, we use the inbuilt function nx.connected_components, which gives us all the connected components in the graph ‘G’. ‘giant’ here is the maximum of all the connected components 



Ng is the length of the giant component i.e, the number of nodes in the giant component. With this we find Ng/N.
Each value of Ng/N is appended to the list NgbyN.


We plot the graph of Ng/N vs the Degree of the graph :

Figure 1
Theory:
The largest connected component is also called a clique. 
The probability (henceforth denoted by P) if it is equal to zero then there will be no connected component and the value of Ng/N will tend to zero, on the other extreme; if the P is 1 the value of Ng/N will tend to 1.

In our case, the probability is between 0 and 1. 

From the graph, we can infer that the value of Ng/N remains close to zero till <k> is 1 because we need at least one link per node to see a giant component. The graph shows a sudden rise in Ng/N at around k == 1.3, keeps on increasing and reaches saturation around k == 3.5.

The value of N is small (i.e, 1000) is our computation but to generalize for larger datasets/ real life datasets that have a billion nodes, even if the average degree is 2 i.e, a node  is connected to only two more nodes at random, the giant component occupies 75% of the network (from the graph) .

The graph can be divided into 4 regions:
Subcritical : 0 <= <k> < 1 : Nothing much happens here.
Critical Point : k = 1: This marks the point where the probability of link between nodes becomes one. 
Supercritical region : 1 < <k> < 4.5 : The Ng/N value keeps increasing .
Connected Region : <k> > ln(Number of Nodes) : The entire graph is connected.

So, when we compare it with our graph, we see that Ng/N is not 0 for the subcritical region, it is because the average degree is between zero and 1, which means that some nodes will still be connected hence contributing to the Ng part.

The graph shows the expected behavior in the critical and subcritical region.

The  Ng/N is very very close to 1 in the connected region (<k> > 3) so it fits accurately with what we discussed in class.

-------------------------------
End Of The Report
