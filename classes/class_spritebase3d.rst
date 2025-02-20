:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/SpriteBase3D.xml.

.. _class_SpriteBase3D:

SpriteBase3D
============

**Inherits:** :ref:`GeometryInstance3D<class_GeometryInstance3D>` **<** :ref:`VisualInstance3D<class_VisualInstance3D>` **<** :ref:`Node3D<class_Node3D>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`AnimatedSprite3D<class_AnimatedSprite3D>`, :ref:`Sprite3D<class_Sprite3D>`

2D sprite node in 3D environment.

Description
-----------

A node that displays 2D texture information in a 3D environment. See also :ref:`Sprite3D<class_Sprite3D>` where many other properties are defined.

Properties
----------

+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`AlphaCutMode<enum_SpriteBase3D_AlphaCutMode>`     | :ref:`alpha_cut<class_SpriteBase3D_property_alpha_cut>`             | ``0``                 |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| Vector3.Axis                                            | :ref:`axis<class_SpriteBase3D_property_axis>`                       | ``2``                 |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`BillboardMode<enum_BaseMaterial3D_BillboardMode>` | :ref:`billboard<class_SpriteBase3D_property_billboard>`             | ``0``                 |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`bool<class_bool>`                                 | :ref:`centered<class_SpriteBase3D_property_centered>`               | ``true``              |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`bool<class_bool>`                                 | :ref:`double_sided<class_SpriteBase3D_property_double_sided>`       | ``true``              |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`bool<class_bool>`                                 | :ref:`fixed_size<class_SpriteBase3D_property_fixed_size>`           | ``false``             |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`bool<class_bool>`                                 | :ref:`flip_h<class_SpriteBase3D_property_flip_h>`                   | ``false``             |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`bool<class_bool>`                                 | :ref:`flip_v<class_SpriteBase3D_property_flip_v>`                   | ``false``             |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`Color<class_Color>`                               | :ref:`modulate<class_SpriteBase3D_property_modulate>`               | ``Color(1, 1, 1, 1)`` |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`bool<class_bool>`                                 | :ref:`no_depth_test<class_SpriteBase3D_property_no_depth_test>`     | ``false``             |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`Vector2<class_Vector2>`                           | :ref:`offset<class_SpriteBase3D_property_offset>`                   | ``Vector2(0, 0)``     |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`float<class_float>`                               | :ref:`pixel_size<class_SpriteBase3D_property_pixel_size>`           | ``0.01``              |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`int<class_int>`                                   | :ref:`render_priority<class_SpriteBase3D_property_render_priority>` | ``0``                 |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`bool<class_bool>`                                 | :ref:`shaded<class_SpriteBase3D_property_shaded>`                   | ``false``             |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`TextureFilter<enum_BaseMaterial3D_TextureFilter>` | :ref:`texture_filter<class_SpriteBase3D_property_texture_filter>`   | ``3``                 |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+
| :ref:`bool<class_bool>`                                 | :ref:`transparent<class_SpriteBase3D_property_transparent>`         | ``true``              |
+---------------------------------------------------------+---------------------------------------------------------------------+-----------------------+

Methods
-------

+-----------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`TriangleMesh<class_TriangleMesh>` | :ref:`generate_triangle_mesh<class_SpriteBase3D_method_generate_triangle_mesh>` **(** **)** |const|                                                           |
+-----------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                 | :ref:`get_draw_flag<class_SpriteBase3D_method_get_draw_flag>` **(** :ref:`DrawFlags<enum_SpriteBase3D_DrawFlags>` flag **)** |const|                          |
+-----------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Rect2<class_Rect2>`               | :ref:`get_item_rect<class_SpriteBase3D_method_get_item_rect>` **(** **)** |const|                                                                             |
+-----------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                    | :ref:`set_draw_flag<class_SpriteBase3D_method_set_draw_flag>` **(** :ref:`DrawFlags<enum_SpriteBase3D_DrawFlags>` flag, :ref:`bool<class_bool>` enabled **)** |
+-----------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------+

Enumerations
------------

.. _enum_SpriteBase3D_DrawFlags:

.. _class_SpriteBase3D_constant_FLAG_TRANSPARENT:

.. _class_SpriteBase3D_constant_FLAG_SHADED:

.. _class_SpriteBase3D_constant_FLAG_DOUBLE_SIDED:

.. _class_SpriteBase3D_constant_FLAG_DISABLE_DEPTH_TEST:

.. _class_SpriteBase3D_constant_FLAG_FIXED_SIZE:

.. _class_SpriteBase3D_constant_FLAG_MAX:

enum **DrawFlags**:

- **FLAG_TRANSPARENT** = **0** --- If set, the texture's transparency and the opacity are used to make those parts of the sprite invisible.

- **FLAG_SHADED** = **1** --- If set, lights in the environment affect the sprite.

- **FLAG_DOUBLE_SIDED** = **2** --- If set, texture can be seen from the back as well. If not, the texture is invisible when looking at it from behind.

- **FLAG_DISABLE_DEPTH_TEST** = **3** --- Disables the depth test, so this object is drawn on top of all others. However, objects drawn after it in the draw order may cover it.

- **FLAG_FIXED_SIZE** = **4** --- Label is scaled by depth so that it always appears the same size on screen.

- **FLAG_MAX** = **5** --- Represents the size of the :ref:`DrawFlags<enum_SpriteBase3D_DrawFlags>` enum.

----

.. _enum_SpriteBase3D_AlphaCutMode:

.. _class_SpriteBase3D_constant_ALPHA_CUT_DISABLED:

.. _class_SpriteBase3D_constant_ALPHA_CUT_DISCARD:

.. _class_SpriteBase3D_constant_ALPHA_CUT_OPAQUE_PREPASS:

enum **AlphaCutMode**:

- **ALPHA_CUT_DISABLED** = **0** --- This mode performs standard alpha blending. It can display translucent areas, but transparency sorting issues may be visible when multiple transparent materials are overlapping.

- **ALPHA_CUT_DISCARD** = **1** --- This mode only allows fully transparent or fully opaque pixels. Harsh edges will be visible unless some form of screen-space antialiasing is enabled (see :ref:`ProjectSettings.rendering/anti_aliasing/quality/screen_space_aa<class_ProjectSettings_property_rendering/anti_aliasing/quality/screen_space_aa>`). On the bright side, this mode doesn't suffer from transparency sorting issues when multiple transparent materials are overlapping. This mode is also known as *alpha testing* or *1-bit transparency*.

- **ALPHA_CUT_OPAQUE_PREPASS** = **2** --- This mode draws fully opaque pixels in the depth prepass. This is slower than :ref:`ALPHA_CUT_DISABLED<class_SpriteBase3D_constant_ALPHA_CUT_DISABLED>` or :ref:`ALPHA_CUT_DISCARD<class_SpriteBase3D_constant_ALPHA_CUT_DISCARD>`, but it allows displaying translucent areas and smooth edges while using proper sorting.

Property Descriptions
---------------------

.. _class_SpriteBase3D_property_alpha_cut:

- :ref:`AlphaCutMode<enum_SpriteBase3D_AlphaCutMode>` **alpha_cut**

+-----------+---------------------------+
| *Default* | ``0``                     |
+-----------+---------------------------+
| *Setter*  | set_alpha_cut_mode(value) |
+-----------+---------------------------+
| *Getter*  | get_alpha_cut_mode()      |
+-----------+---------------------------+

The alpha cutting mode to use for the sprite. See :ref:`AlphaCutMode<enum_SpriteBase3D_AlphaCutMode>` for possible values.

----

.. _class_SpriteBase3D_property_axis:

- Vector3.Axis **axis**

+-----------+-----------------+
| *Default* | ``2``           |
+-----------+-----------------+
| *Setter*  | set_axis(value) |
+-----------+-----------------+
| *Getter*  | get_axis()      |
+-----------+-----------------+

The direction in which the front of the texture faces.

----

.. _class_SpriteBase3D_property_billboard:

- :ref:`BillboardMode<enum_BaseMaterial3D_BillboardMode>` **billboard**

+-----------+---------------------------+
| *Default* | ``0``                     |
+-----------+---------------------------+
| *Setter*  | set_billboard_mode(value) |
+-----------+---------------------------+
| *Getter*  | get_billboard_mode()      |
+-----------+---------------------------+

The billboard mode to use for the sprite. See :ref:`BillboardMode<enum_BaseMaterial3D_BillboardMode>` for possible values.

----

.. _class_SpriteBase3D_property_centered:

- :ref:`bool<class_bool>` **centered**

+-----------+---------------------+
| *Default* | ``true``            |
+-----------+---------------------+
| *Setter*  | set_centered(value) |
+-----------+---------------------+
| *Getter*  | is_centered()       |
+-----------+---------------------+

If ``true``, texture will be centered.

----

.. _class_SpriteBase3D_property_double_sided:

- :ref:`bool<class_bool>` **double_sided**

+-----------+----------------------+
| *Default* | ``true``             |
+-----------+----------------------+
| *Setter*  | set_draw_flag(value) |
+-----------+----------------------+
| *Getter*  | get_draw_flag()      |
+-----------+----------------------+

If ``true``, texture can be seen from the back as well, if ``false``, it is invisible when looking at it from behind.

----

.. _class_SpriteBase3D_property_fixed_size:

- :ref:`bool<class_bool>` **fixed_size**

+-----------+----------------------+
| *Default* | ``false``            |
+-----------+----------------------+
| *Setter*  | set_draw_flag(value) |
+-----------+----------------------+
| *Getter*  | get_draw_flag()      |
+-----------+----------------------+

If ``true``, the label is rendered at the same size regardless of distance.

----

.. _class_SpriteBase3D_property_flip_h:

- :ref:`bool<class_bool>` **flip_h**

+-----------+-------------------+
| *Default* | ``false``         |
+-----------+-------------------+
| *Setter*  | set_flip_h(value) |
+-----------+-------------------+
| *Getter*  | is_flipped_h()    |
+-----------+-------------------+

If ``true``, texture is flipped horizontally.

----

.. _class_SpriteBase3D_property_flip_v:

- :ref:`bool<class_bool>` **flip_v**

+-----------+-------------------+
| *Default* | ``false``         |
+-----------+-------------------+
| *Setter*  | set_flip_v(value) |
+-----------+-------------------+
| *Getter*  | is_flipped_v()    |
+-----------+-------------------+

If ``true``, texture is flipped vertically.

----

.. _class_SpriteBase3D_property_modulate:

- :ref:`Color<class_Color>` **modulate**

+-----------+-----------------------+
| *Default* | ``Color(1, 1, 1, 1)`` |
+-----------+-----------------------+
| *Setter*  | set_modulate(value)   |
+-----------+-----------------------+
| *Getter*  | get_modulate()        |
+-----------+-----------------------+

A color value used to *multiply* the texture's colors. Can be used for mood-coloring or to simulate the color of light.

\ **Note:** If a :ref:`GeometryInstance3D.material_override<class_GeometryInstance3D_property_material_override>` is defined on the ``SpriteBase3D``, the material override must be configured to take vertex colors into account for albedo. Otherwise, the color defined in :ref:`modulate<class_SpriteBase3D_property_modulate>` will be ignored. For a :ref:`BaseMaterial3D<class_BaseMaterial3D>`, :ref:`BaseMaterial3D.vertex_color_use_as_albedo<class_BaseMaterial3D_property_vertex_color_use_as_albedo>` must be ``true``. For a :ref:`ShaderMaterial<class_ShaderMaterial>`, ``ALBEDO *= COLOR.rgb;`` must be inserted in the shader's ``fragment()`` function.

----

.. _class_SpriteBase3D_property_no_depth_test:

- :ref:`bool<class_bool>` **no_depth_test**

+-----------+----------------------+
| *Default* | ``false``            |
+-----------+----------------------+
| *Setter*  | set_draw_flag(value) |
+-----------+----------------------+
| *Getter*  | get_draw_flag()      |
+-----------+----------------------+

If ``true``, depth testing is disabled and the object will be drawn in render order.

----

.. _class_SpriteBase3D_property_offset:

- :ref:`Vector2<class_Vector2>` **offset**

+-----------+-------------------+
| *Default* | ``Vector2(0, 0)`` |
+-----------+-------------------+
| *Setter*  | set_offset(value) |
+-----------+-------------------+
| *Getter*  | get_offset()      |
+-----------+-------------------+

The texture's drawing offset.

----

.. _class_SpriteBase3D_property_pixel_size:

- :ref:`float<class_float>` **pixel_size**

+-----------+-----------------------+
| *Default* | ``0.01``              |
+-----------+-----------------------+
| *Setter*  | set_pixel_size(value) |
+-----------+-----------------------+
| *Getter*  | get_pixel_size()      |
+-----------+-----------------------+

The size of one pixel's width on the sprite to scale it in 3D.

----

.. _class_SpriteBase3D_property_render_priority:

- :ref:`int<class_int>` **render_priority**

+-----------+----------------------------+
| *Default* | ``0``                      |
+-----------+----------------------------+
| *Setter*  | set_render_priority(value) |
+-----------+----------------------------+
| *Getter*  | get_render_priority()      |
+-----------+----------------------------+

Sets the render priority for the sprite. Higher priority objects will be sorted in front of lower priority objects.

\ **Note:** This only applies if :ref:`alpha_cut<class_SpriteBase3D_property_alpha_cut>` is set to :ref:`ALPHA_CUT_DISABLED<class_SpriteBase3D_constant_ALPHA_CUT_DISABLED>` (default value).

\ **Note:** This only applies to sorting of transparent objects. This will not impact how transparent objects are sorted relative to opaque objects. This is because opaque objects are not sorted, while transparent objects are sorted from back to front (subject to priority).

----

.. _class_SpriteBase3D_property_shaded:

- :ref:`bool<class_bool>` **shaded**

+-----------+----------------------+
| *Default* | ``false``            |
+-----------+----------------------+
| *Setter*  | set_draw_flag(value) |
+-----------+----------------------+
| *Getter*  | get_draw_flag()      |
+-----------+----------------------+

If ``true``, the :ref:`Light3D<class_Light3D>` in the :ref:`Environment<class_Environment>` has effects on the sprite.

----

.. _class_SpriteBase3D_property_texture_filter:

- :ref:`TextureFilter<enum_BaseMaterial3D_TextureFilter>` **texture_filter**

+-----------+---------------------------+
| *Default* | ``3``                     |
+-----------+---------------------------+
| *Setter*  | set_texture_filter(value) |
+-----------+---------------------------+
| *Getter*  | get_texture_filter()      |
+-----------+---------------------------+

Filter flags for the texture. See :ref:`TextureFilter<enum_BaseMaterial3D_TextureFilter>` for options.

----

.. _class_SpriteBase3D_property_transparent:

- :ref:`bool<class_bool>` **transparent**

+-----------+----------------------+
| *Default* | ``true``             |
+-----------+----------------------+
| *Setter*  | set_draw_flag(value) |
+-----------+----------------------+
| *Getter*  | get_draw_flag()      |
+-----------+----------------------+

If ``true``, the texture's transparency and the opacity are used to make those parts of the sprite invisible.

Method Descriptions
-------------------

.. _class_SpriteBase3D_method_generate_triangle_mesh:

- :ref:`TriangleMesh<class_TriangleMesh>` **generate_triangle_mesh** **(** **)** |const|

Returns a :ref:`TriangleMesh<class_TriangleMesh>` with the sprite's vertices following its current configuration (such as its :ref:`axis<class_SpriteBase3D_property_axis>` and :ref:`pixel_size<class_SpriteBase3D_property_pixel_size>`).

----

.. _class_SpriteBase3D_method_get_draw_flag:

- :ref:`bool<class_bool>` **get_draw_flag** **(** :ref:`DrawFlags<enum_SpriteBase3D_DrawFlags>` flag **)** |const|

Returns the value of the specified flag.

----

.. _class_SpriteBase3D_method_get_item_rect:

- :ref:`Rect2<class_Rect2>` **get_item_rect** **(** **)** |const|

Returns the rectangle representing this sprite.

----

.. _class_SpriteBase3D_method_set_draw_flag:

- void **set_draw_flag** **(** :ref:`DrawFlags<enum_SpriteBase3D_DrawFlags>` flag, :ref:`bool<class_bool>` enabled **)**

If ``true``, the specified flag will be enabled. See :ref:`DrawFlags<enum_SpriteBase3D_DrawFlags>` for a list of flags.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
