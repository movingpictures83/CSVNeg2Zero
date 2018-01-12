# CSVNeg2Zero
# Language: Python
# Input: CSV (file with negative values)
# Output: EDA (edge attribute file for Cytoscape)

PluMA plugin to take a network represented as a CSV file and produce
an EDge Attribute (EDA) file for Cytoscape, with all negative-weight
edges having weight zero.  Note the plugin does NOT remove these
edges from the CSV file.

The input CSV file should contain an input network, with nodes
represented as rows and columns and entry (i, j) the edge from node i
to node j.

The output file will be an EDA file for Cytoscape, which contains
every edge from the CSV file and its corresponding weight if it is positive,
but weight zero if it is negative.

This file can be useful when running visualization algorithms like Fruchterman-Reingold
(Fruchterman and Reingold, 1991) which require positive or zero edge weights.


