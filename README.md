# Fantastic-roads225

- Organization: 
    - Link to 10k Matrix: https://drive.google.com/file/d/1WfgX9HDBK0wrgJcXPwWdNcL0xOTRAkCI/view?usp=sharing
    - Link to video presentation: https://youtu.be/lnGS0h0pUO8

    - Development Logs contain weekly goals and updates across the team
    - src directory contains: 
        - data225.cpp: file that processes and cleans the road network dataset -- also constructs the adjacency matrix with that data.
        - Graph.h/Graph.cpp: contains Graph class and functions for adding/removing edges, and BFS, Dijkstra's and Pagerank algorithms.
        - Utils.cpp/Utils.h: contains algorithms not related to graph class that allowed us to run tests on the adjacency matrix and simple BFS/Dijkstra's tests.
        - main.cpp: core implementation of our program-- construction of the adjacency matrix, implementing a graph from it, and then running BFS, Dijkstra and Pagerank algorithms based on user preference of preferred route. 
        - tests.cpp: contains simple and not so simple tests for our 3 algorithms. To test them, move into main.cpp and comment out main code. This allows us to have a simple makefile, and allows us to focus on core implementation, and then tests second when necessary. 

- To compile the program, simply navigate inside the "src" directory, and type "make" into terminal. 
- To run, type ./main to produce the output of main.cpp.
    - When running, you will receive different prompts. You will be asked your location, as well as desired destination (Examples will be given if you would like to use them, as well as a valid range of vertices). You will then be prompted to input a number, 0-2 based on your preferred route-- (BFS)least nodes (Cities) passed through, (Dijkstra) shorted distance, (Pagerank) best possible route given all data. You will then receive the output to the chosen algorithm based on the user's preffered route, and you can "proceed" down this route. 
    - To run tests, comment out "main" code, and move tests from tests.cpp into main function in main.cpp.