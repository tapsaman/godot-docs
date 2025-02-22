.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the PinJoint2D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_PinJoint2D:

PinJoint2D
==========

**Inherits:** :ref:`Joint2D<class_Joint2D>` **<** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

Pin Joint for 2D shapes.

Properties
----------

+---------------------------+-----------------------------------------------------+-----+
| :ref:`float<class_float>` | :ref:`softness<class_PinJoint2D_property_softness>` | 0.0 |
+---------------------------+-----------------------------------------------------+-----+

Description
-----------

Pin Joint for 2D rigid bodies. It pins two bodies (rigid or static) together.

Property Descriptions
---------------------

.. _class_PinJoint2D_property_softness:

- :ref:`float<class_float>` **softness**

+-----------+---------------------+
| *Default* | 0.0                 |
+-----------+---------------------+
| *Setter*  | set_softness(value) |
+-----------+---------------------+
| *Getter*  | get_softness()      |
+-----------+---------------------+

The higher this value, the more the bond to the pinned partner can flex.

