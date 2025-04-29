# mit-6-0002-problem-set-2--fastest-way-to-get-around-mit-solved
**TO GET THIS SOLUTION VISIT:** [MIT-6.0002 Problem Set 2- Fastest Way to Get Around MIT Solved](https://www.ankitcodinghub.com/product/mit-6-0002-problem-set-2-fastest-way-to-get-around-mit-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116066&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;MIT-6.0002  Problem Set 2- Fastest Way to Get Around MIT Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Introduction

In this problem set you will solve a simple optimization problem on a graph. Specifically, you will find the shortest route from one building to another on the MIT campus given that you wish to constrain the amount of time you spend walking outdoors (in the cold).

Getting Started

Download Files

1. ps2.py: code skeleton

2. graph.py: a set of graph-related data structures (Digraph, Node, and Edge) that you must use

3. mit_map.txt: a sample data file that holds the information about an MIT campus map.

Introduction

Here is the map of the MIT campus that we all know and love. From the text input file, mit_map.txt, you will build a representation of this map in Python using the graph-related data structures that we provide.

Each line in mit_map.txt has 4 pieces of data in it in the following order separated by a single space (space-delimited): the start building, the destination building, the distance in meters between the two buildings, and the distance in meters between the two buildings that must be spent outdoors. For example, suppose the map text file contained the following line:

10 32 200 40

This means that the map contains an edge from building 10 (start location) to building 32 (end location) that is 200 meters long, where 40 of those 200 meters are spent outside. During the day, routes are crowded and only allow for you to travel in one direction.

Problem 1: Creating the Data Structure Representation

In this problem set, we are dealing with edges that have different weights. In the figure below, the blue numbers show the cost of traversing an edge in terms of total distance traveled, while the green numbers show the cost of traversing an edge in terms of distance spent outdoors. Note that the distance spent outdoors for a single edge is always less than or equal to the total distance it takes to traverse that edge. Now the cost of going from “a” to “b” to “e” is a total distance traveled of 22 meters, where 14 of those meters are spent outdoors.

In graph.py, you’ll find the Node, and Edge classes, which do not store information about weights associated with each edge. You will also find skeletons of the WeightedEdge and Digraph classes, which we will use in the rest of this problem set. Complete the WeightedEdge and Digraph classes such that the unit tests at the bottom of graph.py pass. Your WeightedEdge class will need to implement the __str__ method (which is called when we use str() on a WeightedEdge object) as follows:

Suppose we have a WeightedEdge object e containing by the following information:

Source node name: ‘a’

Destination node name: ‘b’

Total distance along the edge: 15

Outdoor distance along the edge: 10

Then str(e) with the above information should yield: a-&gt;b (15, 10)

For Digraph, you will need to implement the add_node and add_edge methods.

Problem 2: Building up the Campus Map

For this problem, you will be implementing the load_map(map_filename) function in ps2.py, which reads in data from a file and builds a directed graph to properly represent the MIT campus map according to the data. Think about how you plan on representing your graph before implementing load_map.

Problem 2a: Designing your graph

Decide how the campus map problem can be modeled as a graph. Write a description of your design approach as a comment under the Problem #2 heading in ps2.py. What do the graph’s nodes represent in this problem? What do the graph’s edges represent in this problem? Where are the distances represented?

#Problem 2a: Designing your graph

#

# What do the graph’s nodes represent in this problem? What # do the graph’s edges represent? Where are the distances # represented?

#

Problem 2b: Implementing load_map

https://docs.python.org/3/tutorial/inputoutput.html

Problem 2c: Testing load_map

“a”, “b”, and “c” and edges WeightedEdge(a, b, 10, 9), WeightedEdge(a, c, 12, 2), and WeightedEdge(b, c, 1, 1), if you were to print out your graph, you would see something like:

Loading map from file…

a-&gt;b (10, 9) a-&gt;c (12, 2) b-&gt;c (1, 1)

Submit test_load_map.txt. Also, include the lines used to test load_map at the location specified in ps2.py, but comment them out.

Problem 3: Find the Shortest Path using Optimized Depth First Search

We can define a valid path from a given start to end node in a graph as an ordered sequence of nodes

[n1 , n 2, … n k] , where n1 to n k are existing nodes in the graph and there is an edge from n i to n i+1 for i=1 to k – 1. In Figure 2, each edge is unweighted, so you can assume that each edge has distance 1, and then the total distance traveled on the path is 4.

Figure 2. Example of a path from start to end node.

In our campus map problem, the total distance traveled on a path is equal to the sum of all total distances traveled between adjacent nodes on this path. Similarly, the distance spent outdoors on the path is equal to the sum of all distances spent outdoors on the edges in the path.

Problem 3a: Objective function

Write a sentence describing what is the objective function for this problem.

# Problem 3a: Objective function

#

# What is the objective function for this problem? What are the constraints?

#

Problem 3b: Implement get_best_path

Implement the helper function get_best_path. Assume that any variables you need have been set correctly in directed_dfs. Below is some pseudocode to help get you started.

if start and end are not valid nodes:

raise an error elif start and end are the same node: update the global variables appropriately else: for all the child nodes of start

construct a path including that node

recursively solve the rest of the path, from the child node to the end node

return the shortest path

Notes:

1. Graphs can contain cycles. A cycle occurs in a graph if the path of nodes leads you back to a node that was already visited in the path. When building up possible paths, if you reach a cycle without knowing it, you could get stuck indefinitely by extending the path with the same nodes that have already been added to the path.

Figure 3. Example of a cycle in a graph.

2. If you come across a path that is longer than your shortest path found so far, then you know that this longer path cannot be your solution, so there is no point in continuing to traverse its children and discover all paths that contain this sub-path. You must include this optimization in your solution in order to receive full credit.

3. While not required, we strongly recommend that you use recursion to solve this problem.

Problem 3c: Implement directed_dfs

Implement the function directed_dfs(digraph, start, end, max_total_dist, max_dist_outdoors) that uses this optimized depth first search to find the shortest path in a directed graph from start node to end node under the following constraints: the total distance travelled is less than or equal to max_total_dist, and the total distance spent outdoors is less than or equal to max_dist_outdoors. If multiple paths are still found, then return any one of them. If no path can be found to satisfy these constraints, then raise a ValueError exception.

All you are doing in this function is initializing variables, calling your recursive function, and returning the appropriate path. Don’t write too much code–our solution has less than 10 lines! Test your code by uncommenting the code at the bottom of ps5.py.

Hand-In Procedure

1. Save

Save your solutions as graph.py, ps2.py, and test_load_map.txt

2. Time and Collaboration Info

At the start of each file, in a comment, write down the number of hours (roughly) you spent on the problems in that part, and the names of the people you collaborated with. For example:

# 6.0002 Problem Set 2

#

… your code goes here …

3. Sanity checks

After you are done with the problem set, do sanity checks. Run the code and make sure it can be run without errors and passes our test cases as well as your own.

MIT OpenCourseWare https://ocw.mit.edu

6.0002 Introduction to Computational Thinking and Data Science

For information about citing these materials or our Terms of Use, visit: https://ocw.mit.edu/terms.
