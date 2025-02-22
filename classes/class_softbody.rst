.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the SoftBody.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_SoftBody:

SoftBody
========

**Inherits:** :ref:`MeshInstance<class_MeshInstance>` **<** :ref:`GeometryInstance<class_GeometryInstance>` **<** :ref:`VisualInstance<class_VisualInstance>` **<** :ref:`Spatial<class_Spatial>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

A soft mesh physics body.

Properties
----------

+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`float<class_float>`       | :ref:`areaAngular_stiffness<class_SoftBody_property_areaAngular_stiffness>`         | 0.5          |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`int<class_int>`           | :ref:`collision_layer<class_SoftBody_property_collision_layer>`                     | 1            |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`int<class_int>`           | :ref:`collision_mask<class_SoftBody_property_collision_mask>`                       | 1            |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`float<class_float>`       | :ref:`damping_coefficient<class_SoftBody_property_damping_coefficient>`             | 0.01         |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`float<class_float>`       | :ref:`drag_coefficient<class_SoftBody_property_drag_coefficient>`                   | 0.0          |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`float<class_float>`       | :ref:`linear_stiffness<class_SoftBody_property_linear_stiffness>`                   | 0.5          |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`NodePath<class_NodePath>` | :ref:`parent_collision_ignore<class_SoftBody_property_parent_collision_ignore>`     | NodePath("") |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`float<class_float>`       | :ref:`pose_matching_coefficient<class_SoftBody_property_pose_matching_coefficient>` | 0.0          |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`float<class_float>`       | :ref:`pressure_coefficient<class_SoftBody_property_pressure_coefficient>`           | 0.0          |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`int<class_int>`           | :ref:`simulation_precision<class_SoftBody_property_simulation_precision>`           | 5            |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`float<class_float>`       | :ref:`total_mass<class_SoftBody_property_total_mass>`                               | 1.0          |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+
| :ref:`float<class_float>`       | :ref:`volume_stiffness<class_SoftBody_property_volume_stiffness>`                   | 0.5          |
+---------------------------------+-------------------------------------------------------------------------------------+--------------+

Methods
-------

+---------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`add_collision_exception_with<class_SoftBody_method_add_collision_exception_with>` **(** :ref:`Node<class_Node>` body **)**                   |
+---------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Array<class_Array>` | :ref:`get_collision_exceptions<class_SoftBody_method_get_collision_exceptions>` **(** **)**                                                        |
+---------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`   | :ref:`get_collision_layer_bit<class_SoftBody_method_get_collision_layer_bit>` **(** :ref:`int<class_int>` bit **)** const                          |
+---------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`   | :ref:`get_collision_mask_bit<class_SoftBody_method_get_collision_mask_bit>` **(** :ref:`int<class_int>` bit **)** const                            |
+---------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`   | :ref:`is_ray_pickable<class_SoftBody_method_is_ray_pickable>` **(** **)** const                                                                    |
+---------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`remove_collision_exception_with<class_SoftBody_method_remove_collision_exception_with>` **(** :ref:`Node<class_Node>` body **)**             |
+---------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`set_collision_layer_bit<class_SoftBody_method_set_collision_layer_bit>` **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)** |
+---------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`set_collision_mask_bit<class_SoftBody_method_set_collision_mask_bit>` **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)**   |
+---------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`set_ray_pickable<class_SoftBody_method_set_ray_pickable>` **(** :ref:`bool<class_bool>` ray_pickable **)**                                   |
+---------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+

Description
-----------

A deformable physics body. Used to create elastic or deformable objects such as cloth, rubber, or other flexible materials.

Property Descriptions
---------------------

.. _class_SoftBody_property_areaAngular_stiffness:

- :ref:`float<class_float>` **areaAngular_stiffness**

+-----------+----------------------------------+
| *Default* | 0.5                              |
+-----------+----------------------------------+
| *Setter*  | set_areaAngular_stiffness(value) |
+-----------+----------------------------------+
| *Getter*  | get_areaAngular_stiffness()      |
+-----------+----------------------------------+

.. _class_SoftBody_property_collision_layer:

- :ref:`int<class_int>` **collision_layer**

+-----------+----------------------------+
| *Default* | 1                          |
+-----------+----------------------------+
| *Setter*  | set_collision_layer(value) |
+-----------+----------------------------+
| *Getter*  | get_collision_layer()      |
+-----------+----------------------------+

The physics layers this area is in.

Collidable objects can exist in any of 32 different layers. These layers work like a tagging system, and are not visual. A collidable can use these layers to select with which objects it can collide, using the collision_mask property.

A contact is detected if object A is in any of the layers that object B scans, or object B is in any layer scanned by object A.

.. _class_SoftBody_property_collision_mask:

- :ref:`int<class_int>` **collision_mask**

+-----------+---------------------------+
| *Default* | 1                         |
+-----------+---------------------------+
| *Setter*  | set_collision_mask(value) |
+-----------+---------------------------+
| *Getter*  | get_collision_mask()      |
+-----------+---------------------------+

The physics layers this area scans for collisions.

.. _class_SoftBody_property_damping_coefficient:

- :ref:`float<class_float>` **damping_coefficient**

+-----------+--------------------------------+
| *Default* | 0.01                           |
+-----------+--------------------------------+
| *Setter*  | set_damping_coefficient(value) |
+-----------+--------------------------------+
| *Getter*  | get_damping_coefficient()      |
+-----------+--------------------------------+

.. _class_SoftBody_property_drag_coefficient:

- :ref:`float<class_float>` **drag_coefficient**

+-----------+-----------------------------+
| *Default* | 0.0                         |
+-----------+-----------------------------+
| *Setter*  | set_drag_coefficient(value) |
+-----------+-----------------------------+
| *Getter*  | get_drag_coefficient()      |
+-----------+-----------------------------+

.. _class_SoftBody_property_linear_stiffness:

- :ref:`float<class_float>` **linear_stiffness**

+-----------+-----------------------------+
| *Default* | 0.5                         |
+-----------+-----------------------------+
| *Setter*  | set_linear_stiffness(value) |
+-----------+-----------------------------+
| *Getter*  | get_linear_stiffness()      |
+-----------+-----------------------------+

.. _class_SoftBody_property_parent_collision_ignore:

- :ref:`NodePath<class_NodePath>` **parent_collision_ignore**

+-----------+------------------------------------+
| *Default* | NodePath("")                       |
+-----------+------------------------------------+
| *Setter*  | set_parent_collision_ignore(value) |
+-----------+------------------------------------+
| *Getter*  | get_parent_collision_ignore()      |
+-----------+------------------------------------+

.. _class_SoftBody_property_pose_matching_coefficient:

- :ref:`float<class_float>` **pose_matching_coefficient**

+-----------+--------------------------------------+
| *Default* | 0.0                                  |
+-----------+--------------------------------------+
| *Setter*  | set_pose_matching_coefficient(value) |
+-----------+--------------------------------------+
| *Getter*  | get_pose_matching_coefficient()      |
+-----------+--------------------------------------+

.. _class_SoftBody_property_pressure_coefficient:

- :ref:`float<class_float>` **pressure_coefficient**

+-----------+---------------------------------+
| *Default* | 0.0                             |
+-----------+---------------------------------+
| *Setter*  | set_pressure_coefficient(value) |
+-----------+---------------------------------+
| *Getter*  | get_pressure_coefficient()      |
+-----------+---------------------------------+

.. _class_SoftBody_property_simulation_precision:

- :ref:`int<class_int>` **simulation_precision**

+-----------+---------------------------------+
| *Default* | 5                               |
+-----------+---------------------------------+
| *Setter*  | set_simulation_precision(value) |
+-----------+---------------------------------+
| *Getter*  | get_simulation_precision()      |
+-----------+---------------------------------+

Increasing this value will improve the resulting simulation, but can affect performance. Use with care.

.. _class_SoftBody_property_total_mass:

- :ref:`float<class_float>` **total_mass**

+-----------+-----------------------+
| *Default* | 1.0                   |
+-----------+-----------------------+
| *Setter*  | set_total_mass(value) |
+-----------+-----------------------+
| *Getter*  | get_total_mass()      |
+-----------+-----------------------+

.. _class_SoftBody_property_volume_stiffness:

- :ref:`float<class_float>` **volume_stiffness**

+-----------+-----------------------------+
| *Default* | 0.5                         |
+-----------+-----------------------------+
| *Setter*  | set_volume_stiffness(value) |
+-----------+-----------------------------+
| *Getter*  | get_volume_stiffness()      |
+-----------+-----------------------------+

Method Descriptions
-------------------

.. _class_SoftBody_method_add_collision_exception_with:

- void **add_collision_exception_with** **(** :ref:`Node<class_Node>` body **)**

Adds a body to the list of bodies that this body can't collide with.

.. _class_SoftBody_method_get_collision_exceptions:

- :ref:`Array<class_Array>` **get_collision_exceptions** **(** **)**

Returns an array of nodes that were added as collision exceptions for this body.

.. _class_SoftBody_method_get_collision_layer_bit:

- :ref:`bool<class_bool>` **get_collision_layer_bit** **(** :ref:`int<class_int>` bit **)** const

Returns an individual bit on the collision mask.

.. _class_SoftBody_method_get_collision_mask_bit:

- :ref:`bool<class_bool>` **get_collision_mask_bit** **(** :ref:`int<class_int>` bit **)** const

Returns an individual bit on the collision mask.

.. _class_SoftBody_method_is_ray_pickable:

- :ref:`bool<class_bool>` **is_ray_pickable** **(** **)** const

.. _class_SoftBody_method_remove_collision_exception_with:

- void **remove_collision_exception_with** **(** :ref:`Node<class_Node>` body **)**

Removes a body from the list of bodies that this body can't collide with.

.. _class_SoftBody_method_set_collision_layer_bit:

- void **set_collision_layer_bit** **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)**

Sets individual bits on the layer mask. Use this if you only need to change one layer's value.

.. _class_SoftBody_method_set_collision_mask_bit:

- void **set_collision_mask_bit** **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)**

Sets individual bits on the collision mask. Use this if you only need to change one layer's value.

.. _class_SoftBody_method_set_ray_pickable:

- void **set_ray_pickable** **(** :ref:`bool<class_bool>` ray_pickable **)**

