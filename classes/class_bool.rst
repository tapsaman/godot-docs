.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the bool.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_bool:

bool
====

**Category:** Built-In Types

Brief Description
-----------------

Boolean built-in type.

Methods
-------

+-------------------------+----------------------------------------------------------------------------------+
| :ref:`bool<class_bool>` | :ref:`bool<class_bool_method_bool>` **(** :ref:`int<class_int>` from **)**       |
+-------------------------+----------------------------------------------------------------------------------+
| :ref:`bool<class_bool>` | :ref:`bool<class_bool_method_bool>` **(** :ref:`float<class_float>` from **)**   |
+-------------------------+----------------------------------------------------------------------------------+
| :ref:`bool<class_bool>` | :ref:`bool<class_bool_method_bool>` **(** :ref:`String<class_String>` from **)** |
+-------------------------+----------------------------------------------------------------------------------+

Description
-----------

Boolean built-in type.

Method Descriptions
-------------------

.. _class_bool_method_bool:

- :ref:`bool<class_bool>` **bool** **(** :ref:`int<class_int>` from **)**

Cast an :ref:`int<class_int>` value to a boolean value, this method will return ``true`` if called with an integer value different to 0 and ``false`` in other case.

- :ref:`bool<class_bool>` **bool** **(** :ref:`float<class_float>` from **)**

Cast a :ref:`float<class_float>` value to a boolean value, this method will return ``true`` if called with a floating-point value different to 0 and ``false`` in other case.

- :ref:`bool<class_bool>` **bool** **(** :ref:`String<class_String>` from **)**

Cast a :ref:`String<class_String>` value to a boolean value, this method will return ``true`` if called with a non-empty string and ``false`` in other case. Examples: ``bool("False")`` returns ``true``, ``bool("")`` returns ``false``.

