# Google-HashCode-2019

The idea of this year's HashCode was to determine the most beautiful slideshow of pictures. Given a list of pictures,
their orientation and some tags that describe it the goal is to find a permutation of these pictures that generates
the highest beauty score. This score is calculated by observing each pair of consecutive pictures and adding the minimum
between the number of tags they have in common and the number of tags each has and the other doesn't.

My implementation considered each picture as a node in a clique. Starting from each node available the program tries to find
the longest road through the graph without entering the same node twice. The weight of each edge is computed by calculating
the beauty score between the 2 pictures. Each time a new road with a higher weight is found, the longest road is updated.

After iterating though all the starter nodes, the longest road found is printed along its length.

To run the program just run the class. To change the input a change in the source code is needed and the recompiling of main.java.
