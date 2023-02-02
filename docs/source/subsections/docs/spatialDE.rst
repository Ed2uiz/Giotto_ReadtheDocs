spatialDE
---------

.. link-button:: https://github.com/drieslab/Giotto/tree/suite/R/spatial_genes.R#L1855
		:type: url
		:text: View Source Code
		:classes: btn-outline-primary btn-block

Last Updated: |today|

Description
~~~~~~~~~~~

Compute spatial variable genes with spatialDE method

Usage
~~~~~

::

   spatialDE(
     gobject = NULL,
     feat_type = NULL,
     spat_unit = NULL,
     spat_loc_name = "raw",
     expression_values = c("raw", "normalized", "scaled", "custom"),
     size = c(4, 2, 1),
     color = c("blue", "green", "red"),
     sig_alpha = 0.5,
     unsig_alpha = 0.5,
     python_path = NULL,
     show_plot = NA,
     return_plot = NA,
     save_plot = NA,
     save_param = list(),
     default_save_name = "SpatialDE"
   )

Arguments
~~~~~~~~~

+-----------------------------------+-----------------------------------+
| ``gobject``                       | Giotto object                     |
+-----------------------------------+-----------------------------------+
| ``feat_type``                     | feature type                      |
+-----------------------------------+-----------------------------------+
| ``spat_unit``                     | spatial unit                      |
+-----------------------------------+-----------------------------------+
| ``spat_loc_name``                 | name for spatial locations        |
+-----------------------------------+-----------------------------------+
| ``expression_values``             | gene expression values to use     |
+-----------------------------------+-----------------------------------+
| ``size``                          | size of plot                      |
+-----------------------------------+-----------------------------------+
| ``color``                         | low/medium/high color scheme for  |
|                                   | plot                              |
+-----------------------------------+-----------------------------------+
| ``sig_alpha``                     | alpha value for significance      |
+-----------------------------------+-----------------------------------+
| ``unsig_alpha``                   | alpha value for unsignificance    |
+-----------------------------------+-----------------------------------+
| ``python_path``                   | specify specific path to python   |
|                                   | if required                       |
+-----------------------------------+-----------------------------------+
| ``show_plot``                     | show plot                         |
+-----------------------------------+-----------------------------------+
| ``return_plot``                   | return ggplot object              |
+-----------------------------------+-----------------------------------+
| ``save_plot``                     | directly save the plot [boolean]  |
+-----------------------------------+-----------------------------------+
| ``save_param``                    | list of saving parameters, see    |
|                                   | ``showSaveParameters``            |
+-----------------------------------+-----------------------------------+
| ``default_save_name``             | default save name for saving,     |
|                                   | don't change, change save_name in |
|                                   | save_param                        |
+-----------------------------------+-----------------------------------+

Details
~~~~~~~

This function is a wrapper for the SpatialDE method originally
implemented in python. See publication
`doi:10.1038/nmeth.4636 <https://doi.org/10.1038/nmeth.4636>`__

Value
~~~~~

a list of data.frames with results and plot (optional)
