combineSpatialCellMetadataInfo
------------------------------

.. link-button:: https://github.com/drieslab/Giotto/tree/suite/R/auxiliary_giotto.R#L4684
		:type: url
		:text: View Source Code
		:classes: btn-outline-primary btn-block

Last Updated: |today|

Description
~~~~~~~~~~~

Combine cell metadata with spatial cell information (e.g. polygon)

Usage
~~~~~

::

   combineSpatialCellMetadataInfo(gobject, spat_unit = NULL, feat_type = NULL)

Arguments
~~~~~~~~~

+-----------------------------------+-----------------------------------+
| ``gobject``                       | Giotto object                     |
+-----------------------------------+-----------------------------------+
| ``spat_unit``                     | spatial unit                      |
+-----------------------------------+-----------------------------------+
| ``feat_type``                     | feature type(s)                   |
+-----------------------------------+-----------------------------------+

Details
~~~~~~~

| The returned data.table has the following columns:

-  sdimx: spatial feature location on the x-axis

-  sdimy: spatial feature location on the y-axis

-  cell_ID: unique cell ID

-  feat: selected feature(s)

-  other columns that are part of the cell metadata

Value
~~~~~

list of data.table(s)
