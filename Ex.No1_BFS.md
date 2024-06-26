# Ex.No: 1  Implementation of Breadth First Search 
### DATE: 12-02-24                                                                           
### REGISTER NUMBER : 212221040188
### AIM: 
To write a python program to implement Breadth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function bfs and take the set “visited” is empty and “queue” is empty
4. Search start with initial node and add the node to visited and queue.
5. For each neighbor node, check node is not in visited then add node to visited and queue list.
6.  Creating loop to print the visited node.
7.   Call the bfs function by passing arguments visited, graph and starting node.
8.   Stop the program.
### Program:
```
graph = { 
 '1': ['2', '3', '4'], 
 '2': ['5', '6'],
 '3': [],  
 '4': [],  
 '5': [],  
 '6': []
}

visited = []
queue = []

def bfs(visited, graph, node):
    visited.append(node)
    queue.append(node)
    while queue:
        m = queue.pop(0)
        print(m,end = " ")
        for neighbour in graph[m]:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)

print("Following is the Breadth-First Search:")
bfs(visited, graph, '1')

```

### Output:

![image](https://github.com/YuvasreeKS/AI_Lab_2023-24/assets/142140003/1c2ff7f4-8874-4267-9561-156a574ea2c7)


### Result:
Thus the breadth first search order was found sucessfully.
