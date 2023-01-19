============
get10Xmatrix
============

:Date: 1/19/23

https://github.com/drieslab/Giotto/tree/suite/R/general_help.R#L936



================

get10Xmatrix

Description
-----------

This function creates an expression matrix from a 10X structured folder

Usage
-----

.. code:: r

   get10Xmatrix(
     path_to_data,
     gene_column_index = 1,
     remove_zero_rows = TRUE,
     split_by_type = TRUE
   )

Arguments
---------

+-------------------------------+--------------------------------------+
| Argument                      | Description                          |
+===============================+======================================+
| ``path_to_data``              | path to the 10X folder               |
+-------------------------------+--------------------------------------+
| ``gene_column_index``         | which column from the features or    |
|                               | genes .tsv file to use for row ids   |
+-------------------------------+--------------------------------------+
| ``remove_zero_rows``          | removes rows with sum equal to zero  |
+-------------------------------+--------------------------------------+
| ``split_by_type``             | split into multiple matrices based   |
|                               | on 3rd column of features.tsv(.gz)   |
+-------------------------------+--------------------------------------+

Details
-------

A typical 10X folder is named raw_feature_bc_matrix or
filtered_feature_bc_matrix and it has 3 files:

-  barcodes.tsv(.gz)

-  features.tsv(.gz) or genes.tsv(.gz)

-  | matrix.mtx(.gz)
   | By default the first column of the features or genes .tsv file will
     be used, however if multiple annotations are provided (e.g. ensembl
     gene ids and gene symbols) the user can select another column.

Value
-----

sparse expression matrix from 10X
