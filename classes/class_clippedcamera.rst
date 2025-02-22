.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the ClippedCamera.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_ClippedCamera:

ClippedCamera
=============

**Inherits:** :ref:`Camera<class_Camera>` **<** :ref:`Spatial<class_Spatial>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------



Properties
----------

+----------------------------------------------------+--------------------------------------------------------------------+-------+
| :ref:`bool<class_bool>`                            | :ref:`clip_to_areas<class_ClippedCamera_property_clip_to_areas>`   | false |
+----------------------------------------------------+--------------------------------------------------------------------+-------+
| :ref:`bool<class_bool>`                            | :ref:`clip_to_bodies<class_ClippedCamera_property_clip_to_bodies>` | true  |
+----------------------------------------------------+--------------------------------------------------------------------+-------+
| :ref:`int<class_int>`                              | :ref:`collision_mask<class_ClippedCamera_property_collision_mask>` | 1     |
+----------------------------------------------------+--------------------------------------------------------------------+-------+
| :ref:`float<class_float>`                          | :ref:`margin<class_ClippedCamera_property_margin>`                 | 0.0   |
+----------------------------------------------------+--------------------------------------------------------------------+-------+
| :ref:`ProcessMode<enum_ClippedCamera_ProcessMode>` | :ref:`process_mode<class_ClippedCamera_property_process_mode>`     | 0     |
+----------------------------------------------------+--------------------------------------------------------------------+-------+

Methods
-------

+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`add_exception<class_ClippedCamera_method_add_exception>` **(** :ref:`Object<class_Object>` node **)**                                           |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`add_exception_rid<class_ClippedCamera_method_add_exception_rid>` **(** :ref:`RID<class_RID>` rid **)**                                          |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`clear_exceptions<class_ClippedCamera_method_clear_exceptions>` **(** **)**                                                                      |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`get_clip_offset<class_ClippedCamera_method_get_clip_offset>` **(** **)** const                                                                  |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`   | :ref:`get_collision_mask_bit<class_ClippedCamera_method_get_collision_mask_bit>` **(** :ref:`int<class_int>` bit **)** const                          |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`remove_exception<class_ClippedCamera_method_remove_exception>` **(** :ref:`Object<class_Object>` node **)**                                     |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`remove_exception_rid<class_ClippedCamera_method_remove_exception_rid>` **(** :ref:`RID<class_RID>` rid **)**                                    |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`set_collision_mask_bit<class_ClippedCamera_method_set_collision_mask_bit>` **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)** |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+

Enumerations
------------

.. _enum_ClippedCamera_ProcessMode:

.. _class_ClippedCamera_constant_CLIP_PROCESS_PHYSICS:

.. _class_ClippedCamera_constant_CLIP_PROCESS_IDLE:

enum **ProcessMode**:

- **CLIP_PROCESS_PHYSICS** = **0**

- **CLIP_PROCESS_IDLE** = **1**

Property Descriptions
---------------------

.. _class_ClippedCamera_property_clip_to_areas:

- :ref:`bool<class_bool>` **clip_to_areas**

+-----------+----------------------------+
| *Default* | false                      |
+-----------+----------------------------+
| *Setter*  | set_clip_to_areas(value)   |
+-----------+----------------------------+
| *Getter*  | is_clip_to_areas_enabled() |
+-----------+----------------------------+

.. _class_ClippedCamera_property_clip_to_bodies:

- :ref:`bool<class_bool>` **clip_to_bodies**

+-----------+-----------------------------+
| *Default* | true                        |
+-----------+-----------------------------+
| *Setter*  | set_clip_to_bodies(value)   |
+-----------+-----------------------------+
| *Getter*  | is_clip_to_bodies_enabled() |
+-----------+-----------------------------+

.. _class_ClippedCamera_property_collision_mask:

- :ref:`int<class_int>` **collision_mask**

+-----------+---------------------------+
| *Default* | 1                         |
+-----------+---------------------------+
| *Setter*  | set_collision_mask(value) |
+-----------+---------------------------+
| *Getter*  | get_collision_mask()      |
+-----------+---------------------------+

.. _class_ClippedCamera_property_margin:

- :ref:`float<class_float>` **margin**

+-----------+-------------------+
| *Default* | 0.0               |
+-----------+-------------------+
| *Setter*  | set_margin(value) |
+-----------+-------------------+
| *Getter*  | get_margin()      |
+-----------+-------------------+

.. _class_ClippedCamera_property_process_mode:

- :ref:`ProcessMode<enum_ClippedCamera_ProcessMode>` **process_mode**

+-----------+-------------------------+
| *Default* | 0                       |
+-----------+-------------------------+
| *Setter*  | set_process_mode(value) |
+-----------+-------------------------+
| *Getter*  | get_process_mode()      |
+-----------+-------------------------+

Method Descriptions
-------------------

.. _class_ClippedCamera_method_add_exception:

- void **add_exception** **(** :ref:`Object<class_Object>` node **)**

.. _class_ClippedCamera_method_add_exception_rid:

- void **add_exception_rid** **(** :ref:`RID<class_RID>` rid **)**

.. _class_ClippedCamera_method_clear_exceptions:

- void **clear_exceptions** **(** **)**

.. _class_ClippedCamera_method_get_clip_offset:

- :ref:`float<class_float>` **get_clip_offset** **(** **)** const

.. _class_ClippedCamera_method_get_collision_mask_bit:

- :ref:`bool<class_bool>` **get_collision_mask_bit** **(** :ref:`int<class_int>` bit **)** const

.. _class_ClippedCamera_method_remove_exception:

- void **remove_exception** **(** :ref:`Object<class_Object>` node **)**

.. _class_ClippedCamera_method_remove_exception_rid:

- void **remove_exception_rid** **(** :ref:`RID<class_RID>` rid **)**

.. _class_ClippedCamera_method_set_collision_mask_bit:

- void **set_collision_mask_bit** **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)**

