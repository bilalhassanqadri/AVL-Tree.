Class Attributes: 
Node: A private, nested struct used to represent a part in inventory. 
o partnum: an int that stores the part number. A key value that uniquely identifies the part. 
o description: a string that describes the part. 
o qty: an int that stores the number of the part on hand. 
o price: the price of the part. 
o left: stores the address of the left child node. 
o right: stores the address of the right child node. 
• root: a private Node pointer that stores the memory address of the root node. 
constructor: sets root to null. 
destructor: frees all memory used can simply call the public clear() method. 
clear(): public version calls the private version, passing the the root pointer as an argument. The private version frees all memory 
used by the object. 
height(): private method that returns the height of the (sub)tree. Accepts a Node pointer as an argument. 
• rotate methods: private and accept a Node pointer as an argument, by reference. Perform appropriate rotations. 
difference(): accepts a Node pointer as an argument and returns the difference in height between two subtrees. Does this by 
calling height on each subtree. 
balance(): accepts a Node pointer by reference and determines what, if any rotations should be applied to subtrees. Does this by 
calling difference and rotate methods. 
append(): public version accepts a part's number, qty, description, and price as arguments. Passes this information, along with the 
root pointer, to the private append method which adds the part to the tree. 
• remove(): public version accepts a part's number and calls the private version, passing this and the root pointer (by reference). 
This causes the matching part to be removed from the tree. 
getOutOfStock() - calls the private version, passing it the root pointer as an argument. Returns the string returned by the private 
version. The private version searches the tree for all parts with qty 0, building a string of parts as it goes. For each part, the 
description, qty, price, and number is added to the string. 
getPart() - the public version accepts a part's number as it's only argument and calls the private version, passing it the number and 
, and number. 
If it doesn't find it, it returns an appropriate error message such as "OUT OF STOCK". The publi 
Go to PC settings to activate Wind0M 
