=======
plotICG
=======

:Date: 2022-10-06

https://github.com/drieslab/Giotto/tree/suite/R/spatial_interaction_visuals.R#L1666

   :format: latex
..

Description
===========

Create barplot to visualize interaction changed features

Usage
=====

.. code:: r

   plotICG(...)

Arguments
=========

+-------------------------------+--------------------------------------+
| Argument                      | Description                          |
+===============================+======================================+
| ``...``                       | Arguments passed on to               |
|                               | ```plotICF`` <#ploticf>`__           |
|                               | list(“:raw-latex:`\n`�, � “,         |
|                               | list(list(list(�gobject�)),          |
|                               | list(“giotto object�)),              |
|                               | “:raw-latex:`\n`�, � “,              |
|                               | list(list(list(�icfObject�)),        |
|                               | list(“ICF (interaction changed       |
|                               | feature) score object�)),            |
|                               | “:raw-latex:`\n`�, � “,              |
|                               | list(list(list(�source_type�)),      |
|                               | list(“cell type of the source        |
|                               | cell�)), “:raw-latex:`\n`�, � “,     |
|                               | list(list(list(�source_markers�)),   |
|                               | list(“markers for the source cell    |
|                               | type�)), “:raw-latex:`\n`�, � “,     |
|                               | list(list(list(�ICF_feats�)),        |
|                               | list(“named character vector of ICF  |
|                               | features�)), “:raw-latex:`\n`�, � “, |
|                               | list(list(list(�cell_color_code�)),  |
|                               | list(“cell color code for the        |
|                               | interacting cell types�)),           |
+-------------------------------+--------------------------------------+

::

   "\n", "    ", list(list(list("show_plot")), list("show plots")), "\n", "    ", list(list(list("return_plot")), list("return plotting object")), "\n", "    ", list(list(list("save_plot")), list("directly save the plot [boolean]")), "\n", "    ", list(list(list("save_param")), list("list of saving parameters from ", list(list("all_plots_save_function")))), "\n", "    ", list(list(list("default_save_name")), list("default save name for saving, don't change, change save_name in save_param")), "\n", 
   "  ")

Seealso
=======

```plotICF`` <#ploticf>`__
