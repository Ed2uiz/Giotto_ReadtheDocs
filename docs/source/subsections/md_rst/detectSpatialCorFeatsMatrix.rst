===========================
detectSpatialCorFeatsMatrix
===========================

:Date: 2022-10-06

https://github.com/drieslab/Giotto/tree/suite/R/spatial_genes.R#L3109


.. role:: raw-latex(raw)
   :format: latex
..

Description
===========

Detect genes that are spatially correlated

Usage
=====

.. code:: r

   detectSpatialCorFeatsMatrix(
     expression_matrix,
     method = c("grid", "network"),
     spatial_network,
     spatial_grid,
     spatial_locs,
     subset_feats = NULL,
     network_smoothing = NULL,
     min_cells_per_grid = 4,
     cor_method = c("pearson", "kendall", "spearman")
   )

Arguments
=========

+-------------------------------+--------------------------------------+
| Argument                      | Description                          |
+===============================+======================================+
| ``expression_matrix``         | provided expression matrix           |
+-------------------------------+--------------------------------------+
| ``method``                    | method to use for spatial averaging  |
+-------------------------------+--------------------------------------+
| ``spatial_network``           | provided spatial network             |
+-------------------------------+--------------------------------------+
| ``spatial_grid``              | provided spatial grid                |
+-------------------------------+--------------------------------------+
| ``spatial_locs``              | provided spatial locations           |
+-------------------------------+--------------------------------------+
| ``subset_feats``              | subset of features to use            |
+-------------------------------+--------------------------------------+
| ``network_smoothing``         | smoothing factor beteen 0 and 1      |
|                               | (default: automatic)                 |
+-------------------------------+--------------------------------------+
| ``min_cells_per_grid``        | minimum number of cells to consider  |
|                               | a grid                               |
+-------------------------------+--------------------------------------+
| ``cor_method``                | correlation method                   |
+-------------------------------+--------------------------------------+

Details
=======

For method = network, it expects a fully connected spatial network. You
can make sure to create a fully connected network by setting minimal_k >
0 in the ```createSpatialNetwork`` <#createspatialnetwork>`__ function.

-  list(“1. grid-averaging:�) list(“average gene expression values
   within a predefined spatial grid�)

-  | list(“2. network-averaging:�) list(“smoothens the gene expression
     matrix by averaging the expression within one cell:raw-latex:`\n`�,
     � by using the neighbours within the predefined spatial network. b
     is a smoothening factor:raw-latex:`\n`“,� that defaults to 1 - 1/k,
     where k is the median number of k-neighbors in
     the:raw-latex:`\n`“,� selected spatial network. Setting b = 0 means
     no smoothing and b = 1 means no contribution:raw-latex:`\n`“,� from
     its own expression.�)
   | The spatCorObject can be further explored with
     showSpatialCorGenes()

Value
=====

returns a spatial correlation object: “spatCorObject�

Seealso
=======

```showSpatialCorFeats`` <#showspatialcorfeats>`__
