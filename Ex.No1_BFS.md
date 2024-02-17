# Ex.No: 1  Implementation of Breadth First Search 
### DATE: 17/02/2024                                                                           
### REGISTER NUMBER : 212221040039
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
~~~
graph = {
  '5' : ['3','7'],
  '3' : ['2', '4'],
  '7' : ['8'],
  '2' : [],
  '4' : ['8'],
  '8' : []
}

visited = [] # List for visited nodes.
queue = []    

def bfs(visited, graph, node): #function for BFS
  visited.append(node)
  queue.append(node)

  while queue:          
    m = queue.pop(0) 
    print (m, end = " ") 

    for neighbour in graph[m]:
      if neighbour not in visited:
        visited.append(neighbour)
        queue.append(neighbour)

bfs(visited, graph, '5')   

~~~


### Output:

![WhatsApp Image 2024-02-17 at 11 36 57_235df77d](https://github.com/DrUmaRaniV/AI_Lab_2023-24/assets/136783487/a502fa6e-08a5-443b-a96f-29bc6053e3ef)



### Result:
Thus the breadth first search order was found sucessfully.
