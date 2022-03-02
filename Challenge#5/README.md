# Singly Linked List
<!-- Short summary or background information -->
where the nodes are sequntially ordered. Each node point to the next one.  
Each node has value and pointer.  
The head pointer point to the first node. And the last node point to null.  

## Challenge
<!-- Description of the challenge -->
* create two Classes Node and LinkedList.  
* create four Method in the LinkedList:
        newLinkedList.AddToHead(10);   
        System.out.println(newLinkedList.ToString());
        System.out.println(newLinkedList.VlaueExist(10));
        newLinkedList.PrintElements();

## Approach & Efficiency
<!-- What approach did you take? Why? What is the Big O space/time for this approach? -->
* AddToHead : create a new node and a pointer equal to the head and then node.next equal the head.    
The big O(1) time no looping / big O(1) space no need to store data    
* ToString() : return a string which concatinate the all values in the node as Format "{ a } -> { b } -> { c } -> NULL".  
The big O(n^2) time for loop throug the Linked list and initilize string each time / big O(n) space for concatinate the String.   
* VlaueExist(10) : create a new node and a pointer equal to the head, and while until the pointer equal null, and check each time if the pointer.value equal to the value we seach for then return true, otherwise make the pointer = pointer.next. And return false if there is no value in the node equal to the value we search for.    
The big O(n) time while loop through the nodes / big O(1) space no need to store data.      
* PrintElements() : create a new node and a pointer equal to the head, and while until the pointer equal null and each time print the pointer.value and make the pointer = pointer.next.  
The big O(n) time while loop through the nodes / big O(1) space no need to store data.      


## API
<!-- Description of each method publicly available to your Linked List -->
* AddToHead : create a new node and a pointer equal to the head and then node.next equal the head.    
* ToString() : create a new node and a pointer equal to the head, then while throught the nodes until the pointer equal to null. return a string which concatinate the all values in the node as Format "{ a } -> { b } -> { c } -> NULL".  
* VlaueExist(10) : create a new node and a pointer equal to the head, and while until the pointer equal null, and check each time if the pointer.value equal to the value we seach for then return true, otherwise make the pointer = pointer.next. And return false if there is no value in the node equal to the value we search for.    
* PrintElements() : create a new node and a pointer equal to the head, and while until the pointer equal null and each time print the pointer.value and make the pointer = pointer.next.  
