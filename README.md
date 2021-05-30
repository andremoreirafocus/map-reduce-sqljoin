Simple map reduce example that demonstrates how to count word occurrences in a a thousand text files

It requires python 2.7 or above

First run:
python .\join.py

It will extract:
-  amount sold for each sales order as values and the store code as the key for the map function.
-  branch name as values and the branch code as the key for the map function.

The reduce function will perform a group by branch code and sum all sales orders for each branch, adding the branch name

Run as many instances of the client as possible to make it faster
python mincemeat.py -p changeme localhost

In this example, the client and the server runs at the same machine. To change it, replace the "localhost" parameter to the host where the server (name server is running)

This code has been derived from the course from PUC Minas on Big Data Architecture, which is part of a PG in Distributed Systems Architecture