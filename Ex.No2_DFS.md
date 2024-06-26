# Ex.No: 2  Implementation of Depth First Search
### DATE: 12-02-24                                                                           
### REGISTER NUMBER : 212221040188
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
```
# Using a Python dictionary to act as an adjacency list 
graph = { 
 '1': ['2', '3', '4'], 
 '2': ['5', '6'],
 '3': [],  
 '4': [],  
 '5': [],  
 '6': []
}
visited = set() # Set to keep track of visited nodes of graph. 
def dfs(visited, graph, node): #function for dfs 
    if node not in visited: 
        print (node,end=" ") 
        visited.add(node) 
        for neighbour in graph[node]: 
            dfs(visited, graph, neighbour) 
# Driver Code 
print("Following is the Depth-First Search") 
dfs(visited, graph, '1') 

```








### Output:
![image](https://github.com/YuvasreeKS/AI_Lab_2023-24/assets/142140003/349a4f67-a267-4fcf-9cd9-f07aa36c22de)



### Result:
Thus the depth first search order was found sucessfully.
