# Tuples

## What is a tuble?
* Used to store multiple items in a single variable
  * Similar to a list 
  * Tuple: (1, 2, 3, 4) , List [1, 2, 3, 4]
* They are ordered and unchangeable/immutable and allow duplicates
* They also can contain any data type, even a mixture of data types
  * ( 1, 4, "hello", True, 4.0)
* There is a handy tuple constructor to create a tuple from existing data, tuple()
  * list = [1, 2, 3, 4]
  * my_tuple = tuple(list)
  * We have now created a tuple called my_tuple that consists of all the values from list

## Why use a tuple?
* Tuples are a very effective way to store data that you do not plan on changing ever. 
* Due to them being immutable, you should not use a tuple when you have data that could potentially change
* Tuples can be an effective way to return more than one variable from a function
