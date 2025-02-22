.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Timer.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Timer:

Timer
=====

**Inherits:** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

A countdown timer.

Properties
----------

+------------------------------------------------------+--------------------------------------------------------+-------+
| :ref:`bool<class_bool>`                              | :ref:`autostart<class_Timer_property_autostart>`       | false |
+------------------------------------------------------+--------------------------------------------------------+-------+
| :ref:`bool<class_bool>`                              | :ref:`one_shot<class_Timer_property_one_shot>`         | false |
+------------------------------------------------------+--------------------------------------------------------+-------+
| :ref:`bool<class_bool>`                              | :ref:`paused<class_Timer_property_paused>`             |       |
+------------------------------------------------------+--------------------------------------------------------+-------+
| :ref:`TimerProcessMode<enum_Timer_TimerProcessMode>` | :ref:`process_mode<class_Timer_property_process_mode>` | 1     |
+------------------------------------------------------+--------------------------------------------------------+-------+
| :ref:`float<class_float>`                            | :ref:`time_left<class_Timer_property_time_left>`       |       |
+------------------------------------------------------+--------------------------------------------------------+-------+
| :ref:`float<class_float>`                            | :ref:`wait_time<class_Timer_property_wait_time>`       | 1.0   |
+------------------------------------------------------+--------------------------------------------------------+-------+

Methods
-------

+-------------------------+------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>` | :ref:`is_stopped<class_Timer_method_is_stopped>` **(** **)** const                       |
+-------------------------+------------------------------------------------------------------------------------------+
| void                    | :ref:`start<class_Timer_method_start>` **(** :ref:`float<class_float>` time_sec=-1 **)** |
+-------------------------+------------------------------------------------------------------------------------------+
| void                    | :ref:`stop<class_Timer_method_stop>` **(** **)**                                         |
+-------------------------+------------------------------------------------------------------------------------------+

Signals
-------

.. _class_Timer_signal_timeout:

- **timeout** **(** **)**

Emitted when the timer reaches 0.

Enumerations
------------

.. _enum_Timer_TimerProcessMode:

.. _class_Timer_constant_TIMER_PROCESS_PHYSICS:

.. _class_Timer_constant_TIMER_PROCESS_IDLE:

enum **TimerProcessMode**:

- **TIMER_PROCESS_PHYSICS** = **0** --- Update the timer during the physics step at each frame (fixed framerate processing).

- **TIMER_PROCESS_IDLE** = **1** --- Update the timer during the idle time at each frame.

Description
-----------

Counts down a specified interval and emits a signal on reaching 0. Can be set to repeat or "one-shot" mode.

Property Descriptions
---------------------

.. _class_Timer_property_autostart:

- :ref:`bool<class_bool>` **autostart**

+-----------+----------------------+
| *Default* | false                |
+-----------+----------------------+
| *Setter*  | set_autostart(value) |
+-----------+----------------------+
| *Getter*  | has_autostart()      |
+-----------+----------------------+

If ``true``, the timer will automatically start when entering the scene tree.

.. _class_Timer_property_one_shot:

- :ref:`bool<class_bool>` **one_shot**

+-----------+---------------------+
| *Default* | false               |
+-----------+---------------------+
| *Setter*  | set_one_shot(value) |
+-----------+---------------------+
| *Getter*  | is_one_shot()       |
+-----------+---------------------+

If ``true``, the timer will stop when reaching 0. If ``false``, it will restart.

.. _class_Timer_property_paused:

- :ref:`bool<class_bool>` **paused**

+----------+-------------------+
| *Setter* | set_paused(value) |
+----------+-------------------+
| *Getter* | is_paused()       |
+----------+-------------------+

If ``true``, the timer is paused and will not process until it is unpaused again, even if :ref:`start<class_Timer_method_start>` is called.

.. _class_Timer_property_process_mode:

- :ref:`TimerProcessMode<enum_Timer_TimerProcessMode>` **process_mode**

+-----------+-------------------------------+
| *Default* | 1                             |
+-----------+-------------------------------+
| *Setter*  | set_timer_process_mode(value) |
+-----------+-------------------------------+
| *Getter*  | get_timer_process_mode()      |
+-----------+-------------------------------+

Processing mode. See :ref:`TimerProcessMode<enum_Timer_TimerProcessMode>`.

.. _class_Timer_property_time_left:

- :ref:`float<class_float>` **time_left**

+----------+-----------------+
| *Getter* | get_time_left() |
+----------+-----------------+

The timer's remaining time in seconds. Returns 0 if the timer is inactive.

**Note:** You cannot set this value. To change the timer's remaining time, use :ref:`wait_time<class_Timer_property_wait_time>`.

.. _class_Timer_property_wait_time:

- :ref:`float<class_float>` **wait_time**

+-----------+----------------------+
| *Default* | 1.0                  |
+-----------+----------------------+
| *Setter*  | set_wait_time(value) |
+-----------+----------------------+
| *Getter*  | get_wait_time()      |
+-----------+----------------------+

Wait time in seconds.

Method Descriptions
-------------------

.. _class_Timer_method_is_stopped:

- :ref:`bool<class_bool>` **is_stopped** **(** **)** const

Returns ``true`` if the timer is stopped.

.. _class_Timer_method_start:

- void **start** **(** :ref:`float<class_float>` time_sec=-1 **)**

Starts the timer. Sets ``wait_time`` to ``time_sec`` if ``time_sec > 0``. This also resets the remaining time to ``wait_time``.

**Note:** this method will not resume a paused timer. See :ref:`paused<class_Timer_property_paused>`.

.. _class_Timer_method_stop:

- void **stop** **(** **)**

Stops the timer.

