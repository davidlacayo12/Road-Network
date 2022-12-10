# Development Log (Date: 11/18//22 -- 12/02/22)

## Weekly Goals
    - Complete one of the 2: BFS & Dijkstra's 
    - Organize data and start implementing adjacent matrix on it 
    - Start creating prompts for program, and continue to create new tests 

## Specific Tasks Completed (and by who)
    - Jason: Completed the major parts of pagerank, and starting running tests on a subset of the 
    50,000 node dataset. This subset of a few thousand nodes will likely be the only set tested with pagerank, due to time efficiency for the program. 
    - David: Finished Dijkstra and BFS for small dataset of weighted nodes, and was able to map nodes to digits to be used in questions asked to the user to return specific data catered to their location and desired destination 
    - Mankeerat: Processed 50,000 lines of data from the 100,000 line dataset, and implemented an adjacency matrix with them. Started tests using the dataset as well. 

## Problems Encountered 
    - BFS is struggling with a weighted graph. There will always be problems with BFS on a weighted graph, so we may change implementation by treating it like multiple edges between 2 nodes representing the same path. If this doesn't work, then BFS will represent the least amount of stops you will make in other cities. So, if you are not worried about running out of gas, and would just like to get to A-B without going through any other paths (even if they are shorter distances), BFS will work best for this. Could still be implemented in our prompts (ex: Would you like the shortest path, or least amount of stops? Dijkstra's vs. BFS). Pagerank will also contribute to this, and we feel like it could be the best of both worlds, factoring in both nodes and distances to create the perfect route for the user. 

## Plans for next week
    - Finish tests with road map dataset on Dijkstra's, BFS, and pagerank 
    - Finish program with prompts that allows user to get distances to a desired location 
    - Finish slideshow and video presentation for our final project 

## Optional: Questions for mentor