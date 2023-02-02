cellProximitySpatPlot3D
-----------------------

.. link-button:: https://github.com/drieslab/Giotto/tree/suite/R/spatial_interaction_visuals.R#L2914
		:type: url
		:text: View Source Code
		:classes: btn-outline-primary btn-block

Last Updated: |today|

Description
~~~~~~~~~~~

Visualize 3D cell-cell interactions according to spatial coordinates in
plotly mode

Usage
~~~~~

::

   cellProximitySpatPlot3D(
     gobject,
     interaction_name = NULL,
     cluster_column = NULL,
     sdimx = "sdimx",
     sdimy = "sdimy",
     sdimz = "sdimz",
     cell_color = NULL,
     cell_color_code = NULL,
     color_as_factor = T,
     show_other_cells = T,
     show_network = T,
     show_other_network = F,
     network_color = NULL,
     spatial_network_name = "Delaunay_network",
     show_grid = F,
     grid_color = NULL,
     spatial_grid_name = "spatial_grid",
     show_legend = T,
     point_size_select = 4,
     point_size_other = 2,
     point_alpha_other = 0.5,
     axis_scale = c("cube", "real", "custom"),
     custom_ratio = NULL,
     x_ticks = NULL,
     y_ticks = NULL,
     z_ticks = NULL,
     show_plot = NA,
     return_plot = NA,
     save_plot = NA,
     save_param = list(),
     default_save_name = "cellProximitySpatPlot3D",
     ...
   )

Arguments
~~~~~~~~~

+-----------------------------------+-----------------------------------+
| ``gobject``                       | giotto object                     |
+-----------------------------------+-----------------------------------+
| ``interaction_name``              | cell-cell interaction name        |
+-----------------------------------+-----------------------------------+
| ``cluster_column``                | cluster column with cell clusters |
+-----------------------------------+-----------------------------------+
| ``sdimx``                         | x-axis dimension name (default =  |
|                                   | 'sdimx')                          |
+-----------------------------------+-----------------------------------+
| ``sdimy``                         | y-axis dimension name (default =  |
|                                   | 'sdimy')                          |
+-----------------------------------+-----------------------------------+
| ``sdimz``                         | z-axis dimension name (default =  |
|                                   | 'sdimz')                          |
+-----------------------------------+-----------------------------------+
| ``cell_color``                    | color for cells (see details)     |
+-----------------------------------+-----------------------------------+
| ``cell_color_code``               | named vector with colors          |
+-----------------------------------+-----------------------------------+
| ``color_as_factor``               | convert color column to factor    |
+-----------------------------------+-----------------------------------+
| ``show_other_cells``              | decide if show cells not in       |
|                                   | network                           |
+-----------------------------------+-----------------------------------+
| ``show_network``                  | show spatial network of selected  |
|                                   | cells                             |
+-----------------------------------+-----------------------------------+
| ``show_other_network``            | show spatial network of not       |
|                                   | selected cells                    |
+-----------------------------------+-----------------------------------+
| ``network_color``                 | color of spatial network          |
+-----------------------------------+-----------------------------------+
| ``spatial_network_name``          | name of spatial network to use    |
+-----------------------------------+-----------------------------------+
| ``show_grid``                     | show spatial grid                 |
+-----------------------------------+-----------------------------------+
| ``grid_color``                    | color of spatial grid             |
+-----------------------------------+-----------------------------------+
| ``spatial_grid_name``             | name of spatial grid to use       |
+-----------------------------------+-----------------------------------+
| ``show_legend``                   | show legend                       |
+-----------------------------------+-----------------------------------+
| ``point_size_select``             | size of selected points           |
+-----------------------------------+-----------------------------------+
| ``point_size_other``              | size of other points              |
+-----------------------------------+-----------------------------------+
| ``point_alpha_other``             | opacity of other points           |
+-----------------------------------+-----------------------------------+
| ``axis_scale``                    | scale of axis                     |
+-----------------------------------+-----------------------------------+
| ``custom_ratio``                  | custom ratio of axes              |
+-----------------------------------+-----------------------------------+
| ``x_ticks``                       | ticks on x-axis                   |
+-----------------------------------+-----------------------------------+
| ``y_ticks``                       | ticks on y-axis                   |
+-----------------------------------+-----------------------------------+
| ``z_ticks``                       | ticks on z-axis                   |
+-----------------------------------+-----------------------------------+
| ``show_plot``                     | show plots                        |
+-----------------------------------+-----------------------------------+
| ``return_plot``                   | return plotly object              |
+-----------------------------------+-----------------------------------+
| ``save_plot``                     | directly save the plot [boolean]  |
+-----------------------------------+-----------------------------------+
| ``save_param``                    | list of saving parameters from    |
|                                   | ``all_plots_save_function``       |
+-----------------------------------+-----------------------------------+
| ``default_save_name``             | default save name for saving,     |
|                                   | don't change, change save_name in |
|                                   | save_param                        |
+-----------------------------------+-----------------------------------+
| ``...``                           | additional parameters             |
+-----------------------------------+-----------------------------------+

Details
~~~~~~~

Description of parameters.

Value
~~~~~

plotly
