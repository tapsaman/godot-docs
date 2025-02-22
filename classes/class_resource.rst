.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Resource.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Resource:

Resource
========

**Inherits:** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`Animation<class_Animation>`, :ref:`AnimationNode<class_AnimationNode>`, :ref:`AnimationNodeStateMachinePlayback<class_AnimationNodeStateMachinePlayback>`, :ref:`AnimationNodeStateMachineTransition<class_AnimationNodeStateMachineTransition>`, :ref:`AudioBusLayout<class_AudioBusLayout>`, :ref:`AudioEffect<class_AudioEffect>`, :ref:`AudioStream<class_AudioStream>`, :ref:`BakedLightmapData<class_BakedLightmapData>`, :ref:`BitMap<class_BitMap>`, :ref:`ButtonGroup<class_ButtonGroup>`, :ref:`CubeMap<class_CubeMap>`, :ref:`Curve<class_Curve>`, :ref:`Curve2D<class_Curve2D>`, :ref:`Curve3D<class_Curve3D>`, :ref:`DynamicFontData<class_DynamicFontData>`, :ref:`EditorSettings<class_EditorSettings>`, :ref:`EditorSpatialGizmoPlugin<class_EditorSpatialGizmoPlugin>`, :ref:`Environment<class_Environment>`, :ref:`Font<class_Font>`, :ref:`GDNativeLibrary<class_GDNativeLibrary>`, :ref:`GIProbeData<class_GIProbeData>`, :ref:`Gradient<class_Gradient>`, :ref:`Image<class_Image>`, :ref:`InputEvent<class_InputEvent>`, :ref:`Material<class_Material>`, :ref:`Mesh<class_Mesh>`, :ref:`MeshLibrary<class_MeshLibrary>`, :ref:`MultiMesh<class_MultiMesh>`, :ref:`NavigationMesh<class_NavigationMesh>`, :ref:`NavigationPolygon<class_NavigationPolygon>`, :ref:`OccluderPolygon2D<class_OccluderPolygon2D>`, :ref:`OpenSimplexNoise<class_OpenSimplexNoise>`, :ref:`PackedDataContainer<class_PackedDataContainer>`, :ref:`PackedScene<class_PackedScene>`, :ref:`PhysicsMaterial<class_PhysicsMaterial>`, :ref:`PolygonPathFinder<class_PolygonPathFinder>`, :ref:`Script<class_Script>`, :ref:`Shader<class_Shader>`, :ref:`Shape<class_Shape>`, :ref:`Shape2D<class_Shape2D>`, :ref:`ShortCut<class_ShortCut>`, :ref:`Sky<class_Sky>`, :ref:`SpriteFrames<class_SpriteFrames>`, :ref:`StyleBox<class_StyleBox>`, :ref:`TextFile<class_TextFile>`, :ref:`Texture<class_Texture>`, :ref:`TextureLayered<class_TextureLayered>`, :ref:`Theme<class_Theme>`, :ref:`TileSet<class_TileSet>`, :ref:`Translation<class_Translation>`, :ref:`VideoStream<class_VideoStream>`, :ref:`VisualScriptNode<class_VisualScriptNode>`, :ref:`VisualShaderNode<class_VisualShaderNode>`, :ref:`World<class_World>`, :ref:`World2D<class_World2D>`

**Category:** Core

Brief Description
-----------------

Base class for all resources.

Properties
----------

+-----------------------------+---------------------------------------------------------------------------------+-------+
| :ref:`bool<class_bool>`     | :ref:`resource_local_to_scene<class_Resource_property_resource_local_to_scene>` | false |
+-----------------------------+---------------------------------------------------------------------------------+-------+
| :ref:`String<class_String>` | :ref:`resource_name<class_Resource_property_resource_name>`                     | ""    |
+-----------------------------+---------------------------------------------------------------------------------+-------+
| :ref:`String<class_String>` | :ref:`resource_path<class_Resource_property_resource_path>`                     | ""    |
+-----------------------------+---------------------------------------------------------------------------------+-------+

Methods
-------

+---------------------------------+----------------------------------------------------------------------------------------------------------------+
| void                            | :ref:`_setup_local_to_scene<class_Resource_method__setup_local_to_scene>` **(** **)** virtual                  |
+---------------------------------+----------------------------------------------------------------------------------------------------------------+
| :ref:`Resource<class_Resource>` | :ref:`duplicate<class_Resource_method_duplicate>` **(** :ref:`bool<class_bool>` subresources=false **)** const |
+---------------------------------+----------------------------------------------------------------------------------------------------------------+
| :ref:`Node<class_Node>`         | :ref:`get_local_scene<class_Resource_method_get_local_scene>` **(** **)** const                                |
+---------------------------------+----------------------------------------------------------------------------------------------------------------+
| :ref:`RID<class_RID>`           | :ref:`get_rid<class_Resource_method_get_rid>` **(** **)** const                                                |
+---------------------------------+----------------------------------------------------------------------------------------------------------------+
| void                            | :ref:`setup_local_to_scene<class_Resource_method_setup_local_to_scene>` **(** **)**                            |
+---------------------------------+----------------------------------------------------------------------------------------------------------------+
| void                            | :ref:`take_over_path<class_Resource_method_take_over_path>` **(** :ref:`String<class_String>` path **)**       |
+---------------------------------+----------------------------------------------------------------------------------------------------------------+

Signals
-------

.. _class_Resource_signal_changed:

- **changed** **(** **)**

Emitted whenever the resource changes.

Description
-----------

Resource is the base class for all Godot-specific resource types, serving primarily as data containers. They are reference counted and freed when no longer in use. They are also cached once loaded from disk, so that any further attempts to load a resource from a given path will return the same reference (all this in contrast to a :ref:`Node<class_Node>`, which is not reference counted and can be instanced from disk as many times as desired). Resources can be saved externally on disk or bundled into another object, such as a :ref:`Node<class_Node>` or another resource.

Tutorials
---------

- :doc:`../getting_started/step_by_step/resources`

Property Descriptions
---------------------

.. _class_Resource_property_resource_local_to_scene:

- :ref:`bool<class_bool>` **resource_local_to_scene**

+-----------+---------------------------+
| *Default* | false                     |
+-----------+---------------------------+
| *Setter*  | set_local_to_scene(value) |
+-----------+---------------------------+
| *Getter*  | is_local_to_scene()       |
+-----------+---------------------------+

If ``true``, the resource will be made unique in each instance of its local scene. It can thus be modified in a scene instance without impacting other instances of that same scene.

.. _class_Resource_property_resource_name:

- :ref:`String<class_String>` **resource_name**

+-----------+-----------------+
| *Default* | ""              |
+-----------+-----------------+
| *Setter*  | set_name(value) |
+-----------+-----------------+
| *Getter*  | get_name()      |
+-----------+-----------------+

The name of the resource. This is an optional identifier.

.. _class_Resource_property_resource_path:

- :ref:`String<class_String>` **resource_path**

+-----------+-----------------+
| *Default* | ""              |
+-----------+-----------------+
| *Setter*  | set_path(value) |
+-----------+-----------------+
| *Getter*  | get_path()      |
+-----------+-----------------+

The path to the resource. In case it has its own file, it will return its filepath. If it's tied to the scene, it will return the scene's path, followed by the resource's index.

Method Descriptions
-------------------

.. _class_Resource_method__setup_local_to_scene:

- void **_setup_local_to_scene** **(** **)** virtual

Virtual function which can be overridden to customize the behavior value of :ref:`setup_local_to_scene<class_Resource_method_setup_local_to_scene>`.

.. _class_Resource_method_duplicate:

- :ref:`Resource<class_Resource>` **duplicate** **(** :ref:`bool<class_bool>` subresources=false **)** const

Duplicates the resource, returning a new resource. By default, sub-resources are shared between resource copies for efficiency, this can be changed by passing ``true`` to the ``subresources`` argument.

.. _class_Resource_method_get_local_scene:

- :ref:`Node<class_Node>` **get_local_scene** **(** **)** const

If :ref:`resource_local_to_scene<class_Resource_property_resource_local_to_scene>` is enabled and the resource was loaded from a :ref:`PackedScene<class_PackedScene>` instantiation, returns the local scene where this resource's unique copy is in use. Otherwise, returns ``null``.

.. _class_Resource_method_get_rid:

- :ref:`RID<class_RID>` **get_rid** **(** **)** const

Returns the RID of the resource (or an empty RID). Many resources (such as :ref:`Texture<class_Texture>`, :ref:`Mesh<class_Mesh>`, etc) are high-level abstractions of resources stored in a server, so this function will return the original RID.

.. _class_Resource_method_setup_local_to_scene:

- void **setup_local_to_scene** **(** **)**

This method is called when a resource with :ref:`resource_local_to_scene<class_Resource_property_resource_local_to_scene>` enabled is loaded from a :ref:`PackedScene<class_PackedScene>` instantiation. Its behavior can be customized by overriding :ref:`_setup_local_to_scene<class_Resource_method__setup_local_to_scene>` from script.

For most resources, this method performs no base logic. :ref:`ViewportTexture<class_ViewportTexture>` performs custom logic to properly set the proxy texture and flags in the local viewport.

.. _class_Resource_method_take_over_path:

- void **take_over_path** **(** :ref:`String<class_String>` path **)**

Sets the path of the resource, potentially overriding an existing cache entry for this path. This differs from setting :ref:`resource_path<class_Resource_property_resource_path>`, as the latter would error out if another resource was already cached for the given path.

