.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Input.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Input:

Input
=====

**Inherits:** :ref:`Object<class_Object>`

**Inherited By:** :ref:`InputDefault<class_InputDefault>`

**Category:** Core

Brief Description
-----------------

A Singleton that deals with inputs.

Methods
-------

+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`action_press<class_Input_method_action_press>` **(** :ref:`String<class_String>` action, :ref:`float<class_float>` strength=1.0 **)**                                                                                             |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`action_release<class_Input_method_action_release>` **(** :ref:`String<class_String>` action **)**                                                                                                                                 |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`add_joy_mapping<class_Input_method_add_joy_mapping>` **(** :ref:`String<class_String>` mapping, :ref:`bool<class_bool>` update_existing=false **)**                                                                               |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>`              | :ref:`get_accelerometer<class_Input_method_get_accelerometer>` **(** **)** const                                                                                                                                                        |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                  | :ref:`get_action_strength<class_Input_method_get_action_strength>` **(** :ref:`String<class_String>` action **)** const                                                                                                                 |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Array<class_Array>`                  | :ref:`get_connected_joypads<class_Input_method_get_connected_joypads>` **(** **)**                                                                                                                                                      |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`CursorShape<enum_Input_CursorShape>` | :ref:`get_current_cursor_shape<class_Input_method_get_current_cursor_shape>` **(** **)** const                                                                                                                                          |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>`              | :ref:`get_gravity<class_Input_method_get_gravity>` **(** **)** const                                                                                                                                                                    |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>`              | :ref:`get_gyroscope<class_Input_method_get_gyroscope>` **(** **)** const                                                                                                                                                                |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                  | :ref:`get_joy_axis<class_Input_method_get_joy_axis>` **(** :ref:`int<class_int>` device, :ref:`int<class_int>` axis **)** const                                                                                                         |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                      | :ref:`get_joy_axis_index_from_string<class_Input_method_get_joy_axis_index_from_string>` **(** :ref:`String<class_String>` axis **)**                                                                                                   |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`                | :ref:`get_joy_axis_string<class_Input_method_get_joy_axis_string>` **(** :ref:`int<class_int>` axis_index **)**                                                                                                                         |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                      | :ref:`get_joy_button_index_from_string<class_Input_method_get_joy_button_index_from_string>` **(** :ref:`String<class_String>` button **)**                                                                                             |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`                | :ref:`get_joy_button_string<class_Input_method_get_joy_button_string>` **(** :ref:`int<class_int>` button_index **)**                                                                                                                   |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`                | :ref:`get_joy_guid<class_Input_method_get_joy_guid>` **(** :ref:`int<class_int>` device **)** const                                                                                                                                     |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`                | :ref:`get_joy_name<class_Input_method_get_joy_name>` **(** :ref:`int<class_int>` device **)**                                                                                                                                           |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                  | :ref:`get_joy_vibration_duration<class_Input_method_get_joy_vibration_duration>` **(** :ref:`int<class_int>` device **)**                                                                                                               |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`              | :ref:`get_joy_vibration_strength<class_Input_method_get_joy_vibration_strength>` **(** :ref:`int<class_int>` device **)**                                                                                                               |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`              | :ref:`get_last_mouse_speed<class_Input_method_get_last_mouse_speed>` **(** **)** const                                                                                                                                                  |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>`              | :ref:`get_magnetometer<class_Input_method_get_magnetometer>` **(** **)** const                                                                                                                                                          |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                      | :ref:`get_mouse_button_mask<class_Input_method_get_mouse_button_mask>` **(** **)** const                                                                                                                                                |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`MouseMode<enum_Input_MouseMode>`     | :ref:`get_mouse_mode<class_Input_method_get_mouse_mode>` **(** **)** const                                                                                                                                                              |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                    | :ref:`is_action_just_pressed<class_Input_method_is_action_just_pressed>` **(** :ref:`String<class_String>` action **)** const                                                                                                           |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                    | :ref:`is_action_just_released<class_Input_method_is_action_just_released>` **(** :ref:`String<class_String>` action **)** const                                                                                                         |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                    | :ref:`is_action_pressed<class_Input_method_is_action_pressed>` **(** :ref:`String<class_String>` action **)** const                                                                                                                     |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                    | :ref:`is_joy_button_pressed<class_Input_method_is_joy_button_pressed>` **(** :ref:`int<class_int>` device, :ref:`int<class_int>` button **)** const                                                                                     |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                    | :ref:`is_joy_known<class_Input_method_is_joy_known>` **(** :ref:`int<class_int>` device **)**                                                                                                                                           |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                    | :ref:`is_key_pressed<class_Input_method_is_key_pressed>` **(** :ref:`int<class_int>` scancode **)** const                                                                                                                               |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                    | :ref:`is_mouse_button_pressed<class_Input_method_is_mouse_button_pressed>` **(** :ref:`int<class_int>` button **)** const                                                                                                               |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`joy_connection_changed<class_Input_method_joy_connection_changed>` **(** :ref:`int<class_int>` device, :ref:`bool<class_bool>` connected, :ref:`String<class_String>` name, :ref:`String<class_String>` guid **)**                |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`parse_input_event<class_Input_method_parse_input_event>` **(** :ref:`InputEvent<class_InputEvent>` event **)**                                                                                                                    |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`remove_joy_mapping<class_Input_method_remove_joy_mapping>` **(** :ref:`String<class_String>` guid **)**                                                                                                                           |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`set_custom_mouse_cursor<class_Input_method_set_custom_mouse_cursor>` **(** :ref:`Resource<class_Resource>` image, :ref:`CursorShape<enum_Input_CursorShape>` shape=0, :ref:`Vector2<class_Vector2>` hotspot=Vector2( 0, 0 ) **)** |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`set_default_cursor_shape<class_Input_method_set_default_cursor_shape>` **(** :ref:`CursorShape<enum_Input_CursorShape>` shape=0 **)**                                                                                             |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`set_mouse_mode<class_Input_method_set_mouse_mode>` **(** :ref:`MouseMode<enum_Input_MouseMode>` mode **)**                                                                                                                        |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`set_use_accumulated_input<class_Input_method_set_use_accumulated_input>` **(** :ref:`bool<class_bool>` enable **)**                                                                                                               |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`start_joy_vibration<class_Input_method_start_joy_vibration>` **(** :ref:`int<class_int>` device, :ref:`float<class_float>` weak_magnitude, :ref:`float<class_float>` strong_magnitude, :ref:`float<class_float>` duration=0 **)** |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`stop_joy_vibration<class_Input_method_stop_joy_vibration>` **(** :ref:`int<class_int>` device **)**                                                                                                                               |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`warp_mouse_position<class_Input_method_warp_mouse_position>` **(** :ref:`Vector2<class_Vector2>` to **)**                                                                                                                         |
+--------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Signals
-------

.. _class_Input_signal_joy_connection_changed:

- **joy_connection_changed** **(** :ref:`int<class_int>` device, :ref:`bool<class_bool>` connected **)**

Emitted when a joypad device has been connected or disconnected.

Enumerations
------------

.. _enum_Input_MouseMode:

.. _class_Input_constant_MOUSE_MODE_VISIBLE:

.. _class_Input_constant_MOUSE_MODE_HIDDEN:

.. _class_Input_constant_MOUSE_MODE_CAPTURED:

.. _class_Input_constant_MOUSE_MODE_CONFINED:

enum **MouseMode**:

- **MOUSE_MODE_VISIBLE** = **0** --- Makes the mouse cursor visible if it is hidden.

- **MOUSE_MODE_HIDDEN** = **1** --- Makes the mouse cursor hidden if it is visible.

- **MOUSE_MODE_CAPTURED** = **2** --- Captures the mouse. The mouse will be hidden and unable to leave the game window, but it will still register movement and mouse button presses.

- **MOUSE_MODE_CONFINED** = **3** --- Makes the mouse cursor visible but confines it to the game window.

.. _enum_Input_CursorShape:

.. _class_Input_constant_CURSOR_ARROW:

.. _class_Input_constant_CURSOR_IBEAM:

.. _class_Input_constant_CURSOR_POINTING_HAND:

.. _class_Input_constant_CURSOR_CROSS:

.. _class_Input_constant_CURSOR_WAIT:

.. _class_Input_constant_CURSOR_BUSY:

.. _class_Input_constant_CURSOR_DRAG:

.. _class_Input_constant_CURSOR_CAN_DROP:

.. _class_Input_constant_CURSOR_FORBIDDEN:

.. _class_Input_constant_CURSOR_VSIZE:

.. _class_Input_constant_CURSOR_HSIZE:

.. _class_Input_constant_CURSOR_BDIAGSIZE:

.. _class_Input_constant_CURSOR_FDIAGSIZE:

.. _class_Input_constant_CURSOR_MOVE:

.. _class_Input_constant_CURSOR_VSPLIT:

.. _class_Input_constant_CURSOR_HSPLIT:

.. _class_Input_constant_CURSOR_HELP:

enum **CursorShape**:

- **CURSOR_ARROW** = **0** --- Arrow cursor. Standard, default pointing cursor.

- **CURSOR_IBEAM** = **1** --- I-beam cursor. Usually used to show where the text cursor will appear when the mouse is clicked.

- **CURSOR_POINTING_HAND** = **2** --- Pointing hand cursor. Usually used to indicate the pointer is over a link or other interactable item.

- **CURSOR_CROSS** = **3** --- Cross cursor. Typically appears over regions in which a drawing operation can be performed or for selections.

- **CURSOR_WAIT** = **4** --- Wait cursor. Indicates that the application is busy performing an operation. This cursor shape denotes that the application is still usable during the operation.

- **CURSOR_BUSY** = **5** --- Busy cursor. Indicates that the application is busy performing an operation. This cursor shape denotes that the application isn't usable during the operation (e.g. something is blocking its main thread).

- **CURSOR_DRAG** = **6** --- Drag cursor. Usually displayed when dragging something.

- **CURSOR_CAN_DROP** = **7** --- Can drop cursor. Usually displayed when dragging something to indicate that it can be dropped at the current position.

- **CURSOR_FORBIDDEN** = **8** --- Forbidden cursor. Indicates that the current action is forbidden (for example, when dragging something) or that the control at a position is disabled.

- **CURSOR_VSIZE** = **9** --- Vertical resize mouse cursor. A double-headed vertical arrow. It tells the user they can resize the window or the panel vertically.

- **CURSOR_HSIZE** = **10** --- Horizontal resize mouse cursor. A double-headed horizontal arrow. It tells the user they can resize the window or the panel horizontally.

- **CURSOR_BDIAGSIZE** = **11** --- Window resize mouse cursor. The cursor is a double-headed arrow that goes from the bottom left to the top right. It tells the user they can resize the window or the panel both horizontally and vertically.

- **CURSOR_FDIAGSIZE** = **12** --- Window resize mouse cursor. The cursor is a double-headed arrow that goes from the top left to the bottom right, the opposite of :ref:`CURSOR_BDIAGSIZE<class_Input_constant_CURSOR_BDIAGSIZE>`. It tells the user they can resize the window or the panel both horizontally and vertically.

- **CURSOR_MOVE** = **13** --- Move cursor. Indicates that something can be moved.

- **CURSOR_VSPLIT** = **14** --- Vertical split mouse cursor. On Windows, it's the same as :ref:`CURSOR_VSIZE<class_Input_constant_CURSOR_VSIZE>`.

- **CURSOR_HSPLIT** = **15** --- Horizontal split mouse cursor. On Windows, it's the same as :ref:`CURSOR_HSIZE<class_Input_constant_CURSOR_HSIZE>`.

- **CURSOR_HELP** = **16** --- Help cursor. Usually a question mark.

Description
-----------

A Singleton that deals with inputs. This includes key presses, mouse buttons and movement, joypads, and input actions. Actions and their events can be set in the **Input Map** tab in the **Project > Project Settings**, or with the :ref:`InputMap<class_InputMap>` class.

Tutorials
---------

- :doc:`../tutorials/inputs/index`

Method Descriptions
-------------------

.. _class_Input_method_action_press:

- void **action_press** **(** :ref:`String<class_String>` action, :ref:`float<class_float>` strength=1.0 **)**

This will simulate pressing the specified action.

The strength can be used for non-boolean actions, it's ranged between 0 and 1 representing the intensity of the given action.

.. _class_Input_method_action_release:

- void **action_release** **(** :ref:`String<class_String>` action **)**

If the specified action is already pressed, this will release it.

.. _class_Input_method_add_joy_mapping:

- void **add_joy_mapping** **(** :ref:`String<class_String>` mapping, :ref:`bool<class_bool>` update_existing=false **)**

Adds a new mapping entry (in SDL2 format) to the mapping database. Optionally update already connected devices.

.. _class_Input_method_get_accelerometer:

- :ref:`Vector3<class_Vector3>` **get_accelerometer** **(** **)** const

If the device has an accelerometer, this will return the acceleration. Otherwise, it returns an empty :ref:`Vector3<class_Vector3>`.

Note this method returns an empty :ref:`Vector3<class_Vector3>` when running from the editor even when your device has an accelerometer. You must export your project to a supported device to read values from the accelerometer.

.. _class_Input_method_get_action_strength:

- :ref:`float<class_float>` **get_action_strength** **(** :ref:`String<class_String>` action **)** const

Returns a value between 0 and 1 representing the intensity of the given action. In a joypad, for example, the further away the axis (analog sticks or L2, R2 triggers) is from the dead zone, the closer the value will be to 1. If the action is mapped to a control that has no axis as the keyboard, the value returned will be 0 or 1.

.. _class_Input_method_get_connected_joypads:

- :ref:`Array<class_Array>` **get_connected_joypads** **(** **)**

Returns an :ref:`Array<class_Array>` containing the device IDs of all currently connected joypads.

.. _class_Input_method_get_current_cursor_shape:

- :ref:`CursorShape<enum_Input_CursorShape>` **get_current_cursor_shape** **(** **)** const

.. _class_Input_method_get_gravity:

- :ref:`Vector3<class_Vector3>` **get_gravity** **(** **)** const

If the device has an accelerometer, this will return the gravity. Otherwise, it returns an empty :ref:`Vector3<class_Vector3>`.

.. _class_Input_method_get_gyroscope:

- :ref:`Vector3<class_Vector3>` **get_gyroscope** **(** **)** const

If the device has a gyroscope, this will return the rate of rotation in rad/s around a device's X, Y, and Z axes. Otherwise, it returns an empty :ref:`Vector3<class_Vector3>`.

.. _class_Input_method_get_joy_axis:

- :ref:`float<class_float>` **get_joy_axis** **(** :ref:`int<class_int>` device, :ref:`int<class_int>` axis **)** const

Returns the current value of the joypad axis at given index (see :ref:`JoystickList<enum_@GlobalScope_JoystickList>`).

.. _class_Input_method_get_joy_axis_index_from_string:

- :ref:`int<class_int>` **get_joy_axis_index_from_string** **(** :ref:`String<class_String>` axis **)**

Returns the index of the provided axis name.

.. _class_Input_method_get_joy_axis_string:

- :ref:`String<class_String>` **get_joy_axis_string** **(** :ref:`int<class_int>` axis_index **)**

Receives a :ref:`JoystickList<enum_@GlobalScope_JoystickList>` axis and returns its equivalent name as a string.

.. _class_Input_method_get_joy_button_index_from_string:

- :ref:`int<class_int>` **get_joy_button_index_from_string** **(** :ref:`String<class_String>` button **)**

Returns the index of the provided button name.

.. _class_Input_method_get_joy_button_string:

- :ref:`String<class_String>` **get_joy_button_string** **(** :ref:`int<class_int>` button_index **)**

Receives a gamepad button from :ref:`JoystickList<enum_@GlobalScope_JoystickList>` and returns its equivalent name as a string.

.. _class_Input_method_get_joy_guid:

- :ref:`String<class_String>` **get_joy_guid** **(** :ref:`int<class_int>` device **)** const

Returns a SDL2-compatible device GUID on platforms that use gamepad remapping. Returns ``"Default Gamepad"`` otherwise.

.. _class_Input_method_get_joy_name:

- :ref:`String<class_String>` **get_joy_name** **(** :ref:`int<class_int>` device **)**

Returns the name of the joypad at the specified device index.

.. _class_Input_method_get_joy_vibration_duration:

- :ref:`float<class_float>` **get_joy_vibration_duration** **(** :ref:`int<class_int>` device **)**

Returns the duration of the current vibration effect in seconds.

.. _class_Input_method_get_joy_vibration_strength:

- :ref:`Vector2<class_Vector2>` **get_joy_vibration_strength** **(** :ref:`int<class_int>` device **)**

Returns the strength of the joypad vibration: x is the strength of the weak motor, and y is the strength of the strong motor.

.. _class_Input_method_get_last_mouse_speed:

- :ref:`Vector2<class_Vector2>` **get_last_mouse_speed** **(** **)** const

Returns the mouse speed for the last time the cursor was moved, and this until the next frame where the mouse moves. This means that even if the mouse is not moving, this function will still return the value of the last motion.

.. _class_Input_method_get_magnetometer:

- :ref:`Vector3<class_Vector3>` **get_magnetometer** **(** **)** const

If the device has a magnetometer, this will return the magnetic field strength in micro-Tesla for all axes.

.. _class_Input_method_get_mouse_button_mask:

- :ref:`int<class_int>` **get_mouse_button_mask** **(** **)** const

Returns mouse buttons as a bitmask. If multiple mouse buttons are pressed at the same time, the bits are added together.

.. _class_Input_method_get_mouse_mode:

- :ref:`MouseMode<enum_Input_MouseMode>` **get_mouse_mode** **(** **)** const

Returns the mouse mode. See the constants for more information.

.. _class_Input_method_is_action_just_pressed:

- :ref:`bool<class_bool>` **is_action_just_pressed** **(** :ref:`String<class_String>` action **)** const

Returns ``true`` when the user starts pressing the action event, meaning it's ``true`` only on the frame that the user pressed down the button.

This is useful for code that needs to run only once when an action is pressed, instead of every frame while it's pressed.

.. _class_Input_method_is_action_just_released:

- :ref:`bool<class_bool>` **is_action_just_released** **(** :ref:`String<class_String>` action **)** const

Returns ``true`` when the user stops pressing the action event, meaning it's ``true`` only on the frame that the user released the button.

.. _class_Input_method_is_action_pressed:

- :ref:`bool<class_bool>` **is_action_pressed** **(** :ref:`String<class_String>` action **)** const

Returns ``true`` if you are pressing the action event.

.. _class_Input_method_is_joy_button_pressed:

- :ref:`bool<class_bool>` **is_joy_button_pressed** **(** :ref:`int<class_int>` device, :ref:`int<class_int>` button **)** const

Returns ``true`` if you are pressing the joypad button (see :ref:`JoystickList<enum_@GlobalScope_JoystickList>`).

.. _class_Input_method_is_joy_known:

- :ref:`bool<class_bool>` **is_joy_known** **(** :ref:`int<class_int>` device **)**

Returns ``true`` if the system knows the specified device. This means that it sets all button and axis indices exactly as defined in :ref:`JoystickList<enum_@GlobalScope_JoystickList>`. Unknown joypads are not expected to match these constants, but you can still retrieve events from them.

.. _class_Input_method_is_key_pressed:

- :ref:`bool<class_bool>` **is_key_pressed** **(** :ref:`int<class_int>` scancode **)** const

Returns ``true`` if you are pressing the key. You can pass a :ref:`KeyList<enum_@GlobalScope_KeyList>` constant.

.. _class_Input_method_is_mouse_button_pressed:

- :ref:`bool<class_bool>` **is_mouse_button_pressed** **(** :ref:`int<class_int>` button **)** const

Returns ``true`` if you are pressing the mouse button specified with :ref:`ButtonList<enum_@GlobalScope_ButtonList>`.

.. _class_Input_method_joy_connection_changed:

- void **joy_connection_changed** **(** :ref:`int<class_int>` device, :ref:`bool<class_bool>` connected, :ref:`String<class_String>` name, :ref:`String<class_String>` guid **)**

.. _class_Input_method_parse_input_event:

- void **parse_input_event** **(** :ref:`InputEvent<class_InputEvent>` event **)**

Feeds an :ref:`InputEvent<class_InputEvent>` to the game. Can be used to artificially trigger input events from code.

.. _class_Input_method_remove_joy_mapping:

- void **remove_joy_mapping** **(** :ref:`String<class_String>` guid **)**

Removes all mappings from the internal database that match the given GUID.

.. _class_Input_method_set_custom_mouse_cursor:

- void **set_custom_mouse_cursor** **(** :ref:`Resource<class_Resource>` image, :ref:`CursorShape<enum_Input_CursorShape>` shape=0, :ref:`Vector2<class_Vector2>` hotspot=Vector2( 0, 0 ) **)**

Sets a custom mouse cursor image, which is only visible inside the game window. The hotspot can also be specified. Passing ``null`` to the image parameter resets to the system cursor. See enum ``CURSOR_*`` for the list of shapes.

``image``'s size must be lower than 256×256.

``hotspot`` must be within ``image``'s size.

.. _class_Input_method_set_default_cursor_shape:

- void **set_default_cursor_shape** **(** :ref:`CursorShape<enum_Input_CursorShape>` shape=0 **)**

Sets the default cursor shape to be used in the viewport instead of :ref:`CURSOR_ARROW<class_Input_constant_CURSOR_ARROW>`.

**Note:** If you want to change the default cursor shape for :ref:`Control<class_Control>`'s nodes, use :ref:`Control.mouse_default_cursor_shape<class_Control_property_mouse_default_cursor_shape>` instead.

.. _class_Input_method_set_mouse_mode:

- void **set_mouse_mode** **(** :ref:`MouseMode<enum_Input_MouseMode>` mode **)**

Sets the mouse mode. See the constants for more information.

.. _class_Input_method_set_use_accumulated_input:

- void **set_use_accumulated_input** **(** :ref:`bool<class_bool>` enable **)**

Whether to accumulate similar input events sent by the operating system. Enabled by default.

.. _class_Input_method_start_joy_vibration:

- void **start_joy_vibration** **(** :ref:`int<class_int>` device, :ref:`float<class_float>` weak_magnitude, :ref:`float<class_float>` strong_magnitude, :ref:`float<class_float>` duration=0 **)**

Starts to vibrate the joypad. Joypads usually come with two rumble motors, a strong and a weak one. ``weak_magnitude`` is the strength of the weak motor (between 0 and 1) and ``strong_magnitude`` is the strength of the strong motor (between 0 and 1). ``duration`` is the duration of the effect in seconds (a duration of 0 will try to play the vibration indefinitely).

**Note:** Not every hardware is compatible with long effect durations; it is recommended to restart an effect if it has to be played for more than a few seconds.

.. _class_Input_method_stop_joy_vibration:

- void **stop_joy_vibration** **(** :ref:`int<class_int>` device **)**

Stops the vibration of the joypad.

.. _class_Input_method_warp_mouse_position:

- void **warp_mouse_position** **(** :ref:`Vector2<class_Vector2>` to **)**

Sets the mouse position to the specified vector.

