Leading Question:
How can we give people the shortest route to their destination, given two locations (example, LA to San Francisco)? Given the Road Network of North America dataset “Road Networks and Points of Interest” (https://www.cs.utah.edu/~lifeifei/SpatialDataset.htm), our goal is to allow the user of our application to find the shortest path between their current location, and a target destination, as well as the busiest roads to avoid. This application allows a driver to save time and money, as they do not get stuck in traffic by avoiding busy roads, and saving time by taking the shortest path (losing the least amount of time) to their destination.  

Dataset Acquisition and Processing:
Data Format:
We would be using the ‘Road Networks of North America (NA)’ dataset from the Real Datasets for Spatial Databases: Road Networks and Points of Interest’ from Utah University. The dataset consists of more than 179,000 edges and is in the format of (Edge ID, Start Node ID, End Node ID, L2 Distance) thus giving us the different points on the North American map with the distance between them. The Utah Dataset we would be using is previously acquired from the Digital Chart of the World Server. The dataset also provides us with an additional file with x and y coordinates of each node ID, which can further help us in determining the name of a city which the user can interact with. 

We plan to use the whole dataset making it an extensive project allowing users to get a fastest route from one city to the another in all of North America.

Data Correction:
There are two ways we would be checking for missing values in this dataset. Firstly, if any node ID is missing an X or a Y coordinate, we would remove that from our dataset. Additionally in the graph, if an Edge ID is missing a start node or an end node, we would remove that edge. Any start node that does not have an end node and vice versa would also be removed. This ensures that our graph is all connected and does not have any missing edges.

Data Storage:
We plan to store the data in the form of a graph. Every node represents a location and every weighted edge between two nodes represents the distance the two places from our dataset. This data storage method is very convenient as it connects all the cities in a network and using traversal, shortest path finding and other algorithms like page rank, we can find the fastest way from a single point to the other while taking into account the route’s busyness etc. This would give us an efficient way to traverse through a big dataset given a location and what rating we are looking for. 


Graph Algorithms:
Function Inputs:
Dijkstra’s Algorithm: Since our goal is to give people the shortest route between any two given locations, our project will use Dijkstra’s Algorithm to find the shortest path between the locations. This will essentially serve the role of a GPS in our program and allow us to identify the fastest way to get from one location to another in the USA. Furthermore, since the weight of each edge is the distance between the two locations, we should not have any problems regarding negative weights in our graph. 

Breadth-First Search: Along with this, we will use Breadth-First Search to determine whether there exists a path between any two locations in the dataset. This will be incredibly helpful if our graph representation consists of numerous small connected components instead of a single large connected graph. 

PageRank: Finally, we plan on implementing a way to find the most popular cities or locations in our final project. As such, PageRank will be incredibly helpful when it comes to measuring the popularity of a specific location in comparison to the rest of the locations present in the dataset.

Function Outputs:
Dijkstra’s Algorithm: The expected output for our implementation of Dijkstra’s Algorithm is the shortest path between two given locations in our dataset, represented as a graph of the nodes and edges traversed on this path.

Breadth-First Search: Given a starting location, Breadth-First Search will output a list of locations that can be accessed through a Breadth-First Search traversal.

PageRank: Looking at our graph representation as a whole, PageRank will output the most popular location located within our dataset. Given a starting location, PageRank will also output the most popular location that can be reached from that specific location.

Function Efficiency:
Dijkstra’s Algorithm: The target time complexity for Dijkstra’s Algorithm is O((V + E)log(V)) when implemented with a minimum heap priority queue, where V is the number of nodes and E is the number of edges.

Breadth-First Search: The target time complexity for Breadth-First Search is O(V + E), where V is the number of nodes and E is the number of edges.

PageRank: The target time complexity for PageRank is O(V + E), where V is the number of nodes and E is the number of edges. This is due to PageRank having to traverse over every node in the graph at least once to find the most popular location and over every edge some number of times depending on the graph traversal.

Timeline:

- Tasks: Implement Data Structure, Data acquisition in that data structure, first algorithm, second algorithm, third algorithm, documentation, results 

- Week of October 31st: 
	- Complete Project proposal
	- Clean data/get rid of missing values. Implement data structure chosen for the project. Must be 	able to build data structure, traverse it, and do simple changes on it with standard data (not with dataset yet).  
	- Implement the first algorithm on the simple data and test if it works before we start 		transferring the actual dataset into our application 
	- Start data acquisition, little by little figuring out and implementing how we will put our data into our first algorithm 
- Week of November 7th: 
	- Complete data acquisition, allowing us to do all of the simple algorithms and manipulations that are expected with our data structure, except on a larger dataset. 
	- Compare efficiency to what we expect, and make changes based on inefficiencies that we find 
	- Complete the first algorithm on our data structure with our dataset, and implement tests that clearly show how our program runs that algorithm with flying colors 
- Week of November 14th:
	- Test for inefficiencies, and if we are going to make any last changes to data structure and organization of datasheet, do it by the end of this week
	- Start implementing remaining 2 algorithms, starting off with basic data, and moving to our full size datasheet 
	- Start documentation on both running the program, and detailed description of how we implemented the first algorithm 
- Thanksgiving break: 
	- Complete remaining 2 algorithms, and have almost all documentation done for those 2 algorithms 
- Final Week: 
	- Write out final report with results 
	- Final tests, and make sure that our program has minimum inefficiencies 
	- Complete documentation, and make sure our Github Repository is organized and professional 
