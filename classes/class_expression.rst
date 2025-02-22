.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Expression.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Expression:

Expression
==========

**Inherits:** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

A class that stores an expression you can execute.

Methods
-------

+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Variant<class_Variant>`         | :ref:`execute<class_Expression_method_execute>` **(** :ref:`Array<class_Array>` inputs=[  ], :ref:`Object<class_Object>` base_instance=null, :ref:`bool<class_bool>` show_error=true **)** |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`           | :ref:`get_error_text<class_Expression_method_get_error_text>` **(** **)** const                                                                                                            |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`               | :ref:`has_execute_failed<class_Expression_method_has_execute_failed>` **(** **)** const                                                                                                    |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Error<enum_@GlobalScope_Error>` | :ref:`parse<class_Expression_method_parse>` **(** :ref:`String<class_String>` expression, :ref:`PoolStringArray<class_PoolStringArray>` input_names=PoolStringArray(  ) **)**              |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Description
-----------

An expression can be made of any arithmetic operation, built-in math function call, method call of a passed instance, or built-in type construction call.

An example expression text using the built-in math functions could be ``sqrt(pow(3,2) + pow(4,2))``.

In the following example we use a :ref:`LineEdit<class_LineEdit>` node to write our expression and show the result.

::

    onready var expression = Expression.new()
    
    func _ready():
        $LineEdit.connect("text_entered", self, "_on_text_entered")
    
    func _on_text_entered(command):
        var error = expression.parse(command, [])
        if error != OK:
            print(expression.get_error_text())
            return
        var result = expression.execute([], null, true)
        if not expression.has_execute_failed():
            $LineEdit.text = str(result)

Method Descriptions
-------------------

.. _class_Expression_method_execute:

- :ref:`Variant<class_Variant>` **execute** **(** :ref:`Array<class_Array>` inputs=[  ], :ref:`Object<class_Object>` base_instance=null, :ref:`bool<class_bool>` show_error=true **)**

Executes the expression that was previously parsed by :ref:`parse<class_Expression_method_parse>` and returns the result. Before you use the returned object, you should check if the method failed by calling :ref:`has_execute_failed<class_Expression_method_has_execute_failed>`.

If you defined input variables in :ref:`parse<class_Expression_method_parse>`, you can specify their values in the inputs array, in the same order.

.. _class_Expression_method_get_error_text:

- :ref:`String<class_String>` **get_error_text** **(** **)** const

Returns the error text if :ref:`parse<class_Expression_method_parse>` has failed.

.. _class_Expression_method_has_execute_failed:

- :ref:`bool<class_bool>` **has_execute_failed** **(** **)** const

Returns ``true`` if :ref:`execute<class_Expression_method_execute>` has failed.

.. _class_Expression_method_parse:

- :ref:`Error<enum_@GlobalScope_Error>` **parse** **(** :ref:`String<class_String>` expression, :ref:`PoolStringArray<class_PoolStringArray>` input_names=PoolStringArray(  ) **)**

Parses the expression and returns an :ref:`Error<enum_@GlobalScope_Error>` code.

You can optionally specify names of variables that may appear in the expression with ``input_names``, so that you can bind them when it gets executed.

