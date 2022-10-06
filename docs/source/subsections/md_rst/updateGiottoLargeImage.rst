======================
updateGiottoLargeImage
======================

:Date: 2022-10-06

Description
===========

Updates the boundaries of a giotto ``largeImage`` object attached to a
``giotto`` object if both ``gobject`` and ``largeImage_name`` params are
given. Alternatively can directly accept and return as ``largeImage``

Usage
=====

.. code:: r

   updateGiottoLargeImage(
     gobject = NULL,
     largeImage_name = NULL,
     giottoLargeImage = NULL,
     xmax_adj = 0,
     xmin_adj = 0,
     ymax_adj = 0,
     ymin_adj = 0,
     x_shift = 0,
     y_shift = 0,
     scale_factor = NULL,
     scale_x = 1,
     scale_y = 1,
     order = c("first_adj", "first_scale"),
     xmin_set = NULL,
     xmax_set = NULL,
     ymin_set = NULL,
     ymax_set = NULL,
     return_gobject = TRUE,
     verbose = TRUE
   )

Arguments
=========

+-------------------------------+--------------------------------------+
| Argument                      | Description                          |
+===============================+======================================+
| ``gobject``                   | ``giotto`` object containing giotto  |
|                               | ``largeImage`` object                |
+-------------------------------+--------------------------------------+
| ``largeImage_name``           | name of giotto ``largeImage`` object |
+-------------------------------+--------------------------------------+
| ``giottoLargeImage``          | ``largeImage`` object to directly    |
|                               | update                               |
+-------------------------------+--------------------------------------+
| ``xmax_adj, x                 | adjust image boundaries by           |
| min_adj, ymax_adj, ymin_adj`` | increasing maximum and decreasing    |
|                               | minimum bounds respectively of xy    |
|                               | bounds                               |
+-------------------------------+--------------------------------------+
| ``x_shift, y_shift``          | shift entire image along xy axes     |
+-------------------------------+--------------------------------------+
| ``scale_factor``              | set ``scale_x`` and ``scale_y``      |
|                               | params at the same time              |
+-------------------------------+--------------------------------------+
| ``scale_x, scale_y``          | independently scale x or y axis      |
|                               | image mapping from coordinate origin |
+-------------------------------+--------------------------------------+
| ``order``                     | order of operations between fine     |
|                               | adjustments (adjustment and shift    |
|                               | parameters) and scaling              |
+-------------------------------+--------------------------------------+
| ``xmin_set, x                 | directly set xy image boundaries.    |
| max_set, ymin_set, ymax_set`` | Overrides minmax values as spatial   |
|                               | anchor.                              |
+-------------------------------+--------------------------------------+
| ``return_gobject``            | return a ``giotto`` object if        |
|                               | ``TRUE`` , a giotto ``largeImage``   |
|                               | object if ``FALSE``                  |
+-------------------------------+--------------------------------------+
| ``verbose``                   | be verbose                           |
+-------------------------------+--------------------------------------+

Value
=====

a ``giotto`` object or an updated giotto ``largeImage`` object if
``return_gobject = FALSE``
