# Hamiltonian cycles finder/Buscador de ciclos Hamiltonianos-Enunciado:
<img src="/enunciado/img1.jpg" alt="enunciado">

# Algorithms and Data Structures Final Assignment
The students who passed Algorithms and Data Structures are planning to take a trip to Europe to celebrate. The plan is to arrive in Madrid and tour a total of 8 cities, returning to Madrid. Since the budget is limited, they must not repeat cities and also analyse various options to make a decision on how to make the journey more economical. The cost of travel between cities is symmetric. The cities to visit are (along with their initials):

Madrid      (MA)       Paris      (PA)       Rome     (RO)       Zürich       (ZU)
Berlin      (BE)       Amsterdam  (AM)       Warsaw (WA)         Vienna      (VI)

The costs of travelling between cities are as follows:
![imagen](https://github.com/EzeErlicher/Hamiltonian-cycles-finder/assets/103656263/90425928-cc66-4205-adfa-16b487543101)

The representation of the costs is triangular since the graph is undirected. Rows are the origin and columns are the destination. The problem is traditionally known as the "Hamiltonian cycle." You can watch an explanatory video about the algorithm at https://www.youtube.com/watch?v=-AX-U6Ok0is (the video is in Spanish).

However, given the multiple connections between the desired cities, there might be more than one possible Hamiltonian cycle. Therefore, you'll need to find all possible cycles and determine the one with the lowest cost.

To find all cycles, you should apply a breadth-first search algorithm, using an m-ary tree rooted at a starting point, and each child representing the next city that can be accessed and is a valid option for the cycle. 

Keep in mind the properties that Hamiltonian cycles must fulfill as outlined in the previous link, as it helps minimize the number of options to evaluate and consequently, the total processing time of the algorithm. 

For all determined Hamiltonian cycles, you should print the sequence of cities that form it and the total cost of it.


