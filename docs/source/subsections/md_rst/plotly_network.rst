==============
plotly_network
==============

:Date: 2022-10-06

https://github.com/drieslab/Giotto/tree/suite/R/auxiliary_visuals.R#L1874

===========

provide network segment to draw in 3D plot_ly()

Usage
=====

.. code:: r

   plotly_network(
     network,
     x = "sdimx_begin",
     y = "sdimy_begin",
     z = "sdimz_begin",
     x_end = "sdimx_end",
     y_end = "sdimy_end",
     z_end = "sdimz_end"
   )

Arguments
=========

=========== ========================
Argument    Description
=========== ========================
``network`` network object
``x``       default to “sdimx_begin�
``y``       default to “sdimy_begin�
``z``       default to “sdimz_begin�
``x_end``   default to “sdimx_end�
``y_end``   default to “sdimy_end�
``z_end``   default to “sdimz_end�
=========== ========================

Value
=====

edges in network as data.table()
