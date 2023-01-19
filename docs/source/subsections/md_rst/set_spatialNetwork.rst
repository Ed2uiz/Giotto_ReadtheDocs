==================
set_spatialNetwork
==================

:Date: 1/19/23

https://github.com/drieslab/Giotto/tree/suite/R/accessors.R#L1596



======================

Set spatial network

Description
-----------

Function to set a spatial network

Usage
-----

.. code:: r

   set_spatialNetwork(
     gobject,
     spat_unit = NULL,
     name = NULL,
     spatial_network,
     verbose = TRUE,
     set_defaults = TRUE
   )

Arguments
---------

+-------------------------------+--------------------------------------+
| Argument                      | Description                          |
+===============================+======================================+
| ``gobject``                   | giotto object                        |
+-------------------------------+--------------------------------------+
| ``spat_unit``                 | spatial unit (e.g. “cell�)           |
+-------------------------------+--------------------------------------+
| ``name``                      | name of spatial network              |
+-------------------------------+--------------------------------------+
| ``spatial_network``           | spatial network                      |
+-------------------------------+--------------------------------------+
| ``verbose``                   | be verbose                           |
+-------------------------------+--------------------------------------+
| ``set_defaults``              | set default spat_unit and feat_type. |
|                               | Change to FALSE only when            |
+-------------------------------+--------------------------------------+

Value
-----

giotto object

Seealso
-------

Other spatial network data accessor functions:
```get_spatialNetwork`` <#getspatialnetwork>`__

Other functions to set data in giotto object:
```get_cell_id`` <#getcellid>`__ , ```get_feat_id`` <#getfeatid>`__ ,
```set_NearestNetwork`` <#setnearestnetwork>`__ ,
```set_cell_id`` <#setcellid>`__ ,
```set_cell_metadata`` <#setcellmetadata>`__ ,
```set_dimReduction`` <#setdimreduction>`__ ,
```set_expression_values`` <#setexpressionvalues>`__ ,
```set_feat_id`` <#setfeatid>`__ ,
```set_feature_info`` <#setfeatureinfo>`__ ,
```set_feature_metadata`` <#setfeaturemetadata>`__ ,
```set_giottoImage`` <#setgiottoimage>`__ ,
```set_multiomics`` <#setmultiomics>`__ ,
```set_polygon_info`` <#setpolygoninfo>`__ ,
```set_spatialGrid`` <#setspatialgrid>`__ ,
```set_spatial_enrichment`` <#setspatialenrichment>`__ ,
```set_spatial_locations`` <#setspatiallocations>`__
