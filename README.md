# CS260CPP
Data structures and algorithms organized and explored in C++.

Organized and iterated through information from a CSV file containing bid information. Each bid's data was stored in a bid structure.

Hash tables store undordered items by mapping them to a location in an array / vector. I created a node structure to hold the bids in a vector. The hash function returns a key that is based off of the table size. Inserting a bid into the table sets the key to the hash function's result, checks for existing nodes at that key, and will either put the new entry in that slot or check each slot until the next open slot is reached to enter it. When searching for a particular bid node, it will also use the hash function to locate it or walk through entries until it is found.
