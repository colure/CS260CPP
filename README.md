# CS260CPP
Data structures and algorithms organized and explored in C++. 

Utilizing abstract data types [a data type described by pre-defined user operations without indicating how each operation is implemented] to organize and iterate through information from a CSV file containing bid information. Each bid's data was stored in a bid structure containing information parsed in from the CSV file. 

Hash tables store undordered items by mapping them to a location in an array / vector. I created a node structure to hold the bids in a vector. The hash function returns a key that is based off of the table size. Inserting a bid into the table sets the key to the hash function's result, checks for existing nodes at that key, and will either put the new entry in that slot or check each slot until the next open slot is reached to enter it. When searching for a particular bid node, it will also use the hash function to locate it or walk through entries until it is found.

Linked List is doubly linked and initialize with the head and tail variables to be null. Appending to the end of the list sets the node as the head if there are no others, or sets the previous tail to the current node, and always set the node as the tail. A prepend always sets the new node as the head and sets the next node's head as the new node. Iterating through the list will go one by one for printing and checking for removals, proceeding from the head to the tail.

The Vector Sorter reflects two different sorting methods. The quick sort partitions the vector of the bids into two parts, selecting the middle element as the pivot point. Swaps the high and low bids and moves end points closer if 'low' section item is greater than the 'high' section. The selection sort iterates through the index and swaps the minimum with the position (current) bid if it's less than the current bid. The timer function also reflects the amount of time it takes to go through using each sorter.
