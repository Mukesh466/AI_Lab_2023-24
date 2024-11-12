# Ex.No: 2  Implementation of Depth First Search
### DATE: 12/08/2024                                                                        
### REGISTER NUMBER : 212222060281
### AIM: 
To write a python program to implement Depth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function dfs and take the set “visited” is empty 
4. Search start with initial node. Check the node is not visited then print the node.
5. For each neighbor node, recursively invoke the dfs search.
6. Call the dfs function by passing arguments visited, graph and starting node.
7. Stop the program.
### Program:
#breadth first Search in python </br>
graph = {</br>
 'A' : ['B','C'],</br>
 'B' : ['D', 'E'],</br>
 'C' : ['F'],</br>
 'D' : [],</br>
 'E' : ['F'],</br>
 'F' : []</br>
 }</br>

visited = set() # Set to keep track of visited nodes of graph.</br>
def dfs(visited, graph, node):  #function for dfs</br>
    if node not in visited:</br>
        print (node)</br>
        visited.add(node)</br>
        for neighbour in graph[node]:</br>
            dfs(visited, graph, neighbour)</br>
#### Driver Code
print("Following is the Depth-First Search")</br>
dfs(visited, graph, 'A')</br>











### Output:

![image](https://github.com/user-attachments/assets/8a0ce37f-e27b-403b-8de6-881c7cdc6d4d)


### Result:
Thus the depth first search order was found sucessfully.
