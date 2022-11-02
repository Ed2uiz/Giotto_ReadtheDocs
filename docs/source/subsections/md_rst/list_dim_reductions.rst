===================
list_dim_reductions
===================

:Date: 2022-10-06

https://github.com/drieslab/Giotto/tree/suite/R/accessors.R#L2237

===========

return the available dimension reductions

Usage
=====

.. code:: r

   list_dim_reductions(
     gobject,
     data_type = NULL,
     spat_unit = NULL,
     feat_type = NULL,
     dim_type = NULL
   )

Arguments
=========

============= =================================================
Argument      Description
============= =================================================
``gobject``   giotto object
``data_type`` “cells� or “feats� data used in dim reduction
``spat_unit`` spatial unit (e.g. “cell�)
``feat_type`` feature type (e.g. “rna�, “dna�, “protein�)
``dim_type``  dimensional reduction method (e.g. “pca�, “umap�)
============= =================================================

Value
=====

names and locations of dimension reduction as a data.table
