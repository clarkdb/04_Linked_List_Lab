04_Linked_List_Lab
==================

Implement a simple linked list using pointers and classes.

Requirements
------------

1. Add, remove, get, and set should be O(1) if `i == 0` or if `i == size()-1`
2. Add, remove, get, and set should throw a string exception if `i >= size()`. Find should throw a string exception if `i > size()`
3. Do not leak memory (make sure remove and the destructor do the right thing)
4. `size()` is O(1) time (keep track of the numItems when you add or remove, so you can just return the variable)

Reading
=======
"Open Data Structures," Chapter 3, up through section 2 (DLList), http://opendatastructures.org/ods-cpp/3_Linked_Lists.html

Questions
=========

#### 1. Which of the above requirements work, and which do not? For each requirement, write a brief response.

1. Add, remove, get and set all are constant time.
2. The methods throw a string exception if a bad value if given.
3. The destructor deletes data contained in the array and nullifies the pointer to the array.
4. The size method simply returns the number of items in the list.

#### 2. If we did an ArrayList instead of a LinkedList, which of the public methods would be faster, and which would be slower? Explain your answer.

In an ArrayList, the add and remove would be a bit slower because the add and remove functions would need to be in linear time rather than being able to make them work in constant time with the help of the nodes.

#### 3. What is one question that confused you about this exercise, or one piece of advice you would share with students next semester?

I am still a bit confused about how the nodes work, do they in fact store three variables? I understand they have a next and a previous, but are those initialized and how would a node look in memory?
