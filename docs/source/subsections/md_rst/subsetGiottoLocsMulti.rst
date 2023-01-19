=====================
subsetGiottoLocsMulti
=====================

:Date: 1/19/23

https://github.com/drieslab/Giotto/tree/suite/R/auxiliary_giotto.R#L1577



=========================

Subset by spatial locations – multi

Description
-----------

Subsets Giotto object based on spatial locations

Usage
-----

.. code:: r

   subsetGiottoLocsMulti(
     gobject,
     spat_unit = NULL,
     feat_type = NULL,
     spat_loc_name = NULL,
     x_max = NULL,
     x_min = NULL,
     y_max = NULL,
     y_min = NULL,
     z_max = NULL,
     z_min = NULL,
     poly_info = NULL,
     return_gobject = TRUE,
     verbose = TRUE
   )

Arguments
---------

+-------------------------------+--------------------------------------+
| Argument                      | Description                          |
+===============================+======================================+
| ``gobject``                   | giotto object                        |
+-------------------------------+--------------------------------------+
| ``spat_unit``                 | spatial unit                         |
+-------------------------------+--------------------------------------+
| ``feat_type``                 | feature type to use                  |
+-------------------------------+--------------------------------------+
| ``spat_loc_name``             | name of spatial locations to use     |
+-------------------------------+--------------------------------------+
| ``x_max, x_min,               | minimum and maximum x, y, and z      |
|  y_max, y_min, z_max, z_min`` | coordinates to subset to             |
+-------------------------------+--------------------------------------+
| ``poly_info``                 | polygon information to use           |
+-------------------------------+--------------------------------------+
| ``return_gobject``            | return Giotto object                 |
+-------------------------------+--------------------------------------+
| ``verbose``                   | be verbose                           |
+-------------------------------+--------------------------------------+

Details
-------

Subsets a Giotto based on spatial locations for multiple spatial units
if return_gobject = FALSE, then a filtered combined metadata data.table
will be returned

Value
-----

giotto object
