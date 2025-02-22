.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the ParallaxBackground.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_ParallaxBackground:

ParallaxBackground
==================

**Inherits:** :ref:`CanvasLayer<class_CanvasLayer>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

A node used to create a parallax scrolling background.

Properties
----------

+-------------------------------+-----------------------------------------------------------------------------------------------+-----------------+
| :ref:`Vector2<class_Vector2>` | :ref:`scroll_base_offset<class_ParallaxBackground_property_scroll_base_offset>`               | Vector2( 0, 0 ) |
+-------------------------------+-----------------------------------------------------------------------------------------------+-----------------+
| :ref:`Vector2<class_Vector2>` | :ref:`scroll_base_scale<class_ParallaxBackground_property_scroll_base_scale>`                 | Vector2( 1, 1 ) |
+-------------------------------+-----------------------------------------------------------------------------------------------+-----------------+
| :ref:`bool<class_bool>`       | :ref:`scroll_ignore_camera_zoom<class_ParallaxBackground_property_scroll_ignore_camera_zoom>` | false           |
+-------------------------------+-----------------------------------------------------------------------------------------------+-----------------+
| :ref:`Vector2<class_Vector2>` | :ref:`scroll_limit_begin<class_ParallaxBackground_property_scroll_limit_begin>`               | Vector2( 0, 0 ) |
+-------------------------------+-----------------------------------------------------------------------------------------------+-----------------+
| :ref:`Vector2<class_Vector2>` | :ref:`scroll_limit_end<class_ParallaxBackground_property_scroll_limit_end>`                   | Vector2( 0, 0 ) |
+-------------------------------+-----------------------------------------------------------------------------------------------+-----------------+
| :ref:`Vector2<class_Vector2>` | :ref:`scroll_offset<class_ParallaxBackground_property_scroll_offset>`                         | Vector2( 0, 0 ) |
+-------------------------------+-----------------------------------------------------------------------------------------------+-----------------+

Description
-----------

A ParallaxBackground uses one or more :ref:`ParallaxLayer<class_ParallaxLayer>` child nodes to create a parallax effect. Each :ref:`ParallaxLayer<class_ParallaxLayer>` can move at a different speed using :ref:`ParallaxLayer.motion_offset<class_ParallaxLayer_property_motion_offset>`. This creates an illusion of depth in a 2D game. If not used with a :ref:`Camera2D<class_Camera2D>`, you must manually calculate the :ref:`scroll_offset<class_ParallaxBackground_property_scroll_offset>`.

Property Descriptions
---------------------

.. _class_ParallaxBackground_property_scroll_base_offset:

- :ref:`Vector2<class_Vector2>` **scroll_base_offset**

+-----------+-------------------------------+
| *Default* | Vector2( 0, 0 )               |
+-----------+-------------------------------+
| *Setter*  | set_scroll_base_offset(value) |
+-----------+-------------------------------+
| *Getter*  | get_scroll_base_offset()      |
+-----------+-------------------------------+

The base position offset for all :ref:`ParallaxLayer<class_ParallaxLayer>` children.

.. _class_ParallaxBackground_property_scroll_base_scale:

- :ref:`Vector2<class_Vector2>` **scroll_base_scale**

+-----------+------------------------------+
| *Default* | Vector2( 1, 1 )              |
+-----------+------------------------------+
| *Setter*  | set_scroll_base_scale(value) |
+-----------+------------------------------+
| *Getter*  | get_scroll_base_scale()      |
+-----------+------------------------------+

The base motion scale for all :ref:`ParallaxLayer<class_ParallaxLayer>` children.

.. _class_ParallaxBackground_property_scroll_ignore_camera_zoom:

- :ref:`bool<class_bool>` **scroll_ignore_camera_zoom**

+-----------+-------------------------------+
| *Default* | false                         |
+-----------+-------------------------------+
| *Setter*  | set_ignore_camera_zoom(value) |
+-----------+-------------------------------+
| *Getter*  | is_ignore_camera_zoom()       |
+-----------+-------------------------------+

If ``true``, elements in :ref:`ParallaxLayer<class_ParallaxLayer>` child aren't affected by the zoom level of the camera.

.. _class_ParallaxBackground_property_scroll_limit_begin:

- :ref:`Vector2<class_Vector2>` **scroll_limit_begin**

+-----------+------------------------+
| *Default* | Vector2( 0, 0 )        |
+-----------+------------------------+
| *Setter*  | set_limit_begin(value) |
+-----------+------------------------+
| *Getter*  | get_limit_begin()      |
+-----------+------------------------+

Top-left limits for scrolling to begin. If the camera is outside of this limit, the background will stop scrolling. Must be lower than :ref:`scroll_limit_end<class_ParallaxBackground_property_scroll_limit_end>` to work.

.. _class_ParallaxBackground_property_scroll_limit_end:

- :ref:`Vector2<class_Vector2>` **scroll_limit_end**

+-----------+----------------------+
| *Default* | Vector2( 0, 0 )      |
+-----------+----------------------+
| *Setter*  | set_limit_end(value) |
+-----------+----------------------+
| *Getter*  | get_limit_end()      |
+-----------+----------------------+

Bottom-right limits for scrolling to end. If the camera is outside of this limit, the background will stop scrolling. Must be higher than :ref:`scroll_limit_begin<class_ParallaxBackground_property_scroll_limit_begin>` to work.

.. _class_ParallaxBackground_property_scroll_offset:

- :ref:`Vector2<class_Vector2>` **scroll_offset**

+-----------+--------------------------+
| *Default* | Vector2( 0, 0 )          |
+-----------+--------------------------+
| *Setter*  | set_scroll_offset(value) |
+-----------+--------------------------+
| *Getter*  | get_scroll_offset()      |
+-----------+--------------------------+

The ParallaxBackground's scroll value. Calculated automatically when using a :ref:`Camera2D<class_Camera2D>`, but can be used to manually manage scrolling when no camera is present.

