:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/EditorFileDialog.xml.

.. _class_EditorFileDialog:

EditorFileDialog
================

**Inherits:** :ref:`ConfirmationDialog<class_ConfirmationDialog>` **<** :ref:`AcceptDialog<class_AcceptDialog>` **<** :ref:`Window<class_Window>` **<** :ref:`Viewport<class_Viewport>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

A modified version of :ref:`FileDialog<class_FileDialog>` used by the editor.

.. rst-class:: classref-introduction-group

Description
-----------

**EditorFileDialog** is an enhanced version of :ref:`FileDialog<class_FileDialog>` available only to editor plugins. Additional features include list of favorited/recent files and the ability to see files as thumbnails grid instead of list.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`Access<enum_EditorFileDialog_Access>`           | :ref:`access<class_EditorFileDialog_property_access>`                                       | ``0``                                                                                    |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>`                           | :ref:`current_dir<class_EditorFileDialog_property_current_dir>`                             |                                                                                          |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>`                           | :ref:`current_file<class_EditorFileDialog_property_current_file>`                           |                                                                                          |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>`                           | :ref:`current_path<class_EditorFileDialog_property_current_path>`                           |                                                                                          |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                               | dialog_hide_on_ok                                                                           | ``false`` (overrides :ref:`AcceptDialog<class_AcceptDialog_property_dialog_hide_on_ok>`) |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                               | :ref:`disable_overwrite_warning<class_EditorFileDialog_property_disable_overwrite_warning>` | ``false``                                                                                |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>` | :ref:`display_mode<class_EditorFileDialog_property_display_mode>`                           | ``0``                                                                                    |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`FileMode<enum_EditorFileDialog_FileMode>`       | :ref:`file_mode<class_EditorFileDialog_property_file_mode>`                                 | ``4``                                                                                    |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`PackedStringArray<class_PackedStringArray>`     | :ref:`filters<class_EditorFileDialog_property_filters>`                                     | ``PackedStringArray()``                                                                  |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                               | :ref:`show_hidden_files<class_EditorFileDialog_property_show_hidden_files>`                 | ``false``                                                                                |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>`                           | title                                                                                       | ``"Save a File"`` (overrides :ref:`Window<class_Window_property_title>`)                 |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +-------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                      | :ref:`add_filter<class_EditorFileDialog_method_add_filter>` **(** :ref:`String<class_String>` filter, :ref:`String<class_String>` description="" **)** |
   +-------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                      | :ref:`clear_filters<class_EditorFileDialog_method_clear_filters>` **(** **)**                                                                          |
   +-------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LineEdit<class_LineEdit>`           | :ref:`get_line_edit<class_EditorFileDialog_method_get_line_edit>` **(** **)**                                                                          |
   +-------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`VBoxContainer<class_VBoxContainer>` | :ref:`get_vbox<class_EditorFileDialog_method_get_vbox>` **(** **)**                                                                                    |
   +-------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                      | :ref:`invalidate<class_EditorFileDialog_method_invalidate>` **(** **)**                                                                                |
   +-------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Signals
-------

.. _class_EditorFileDialog_signal_dir_selected:

.. rst-class:: classref-signal

**dir_selected** **(** :ref:`String<class_String>` dir **)**

Emitted when a directory is selected.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_signal_file_selected:

.. rst-class:: classref-signal

**file_selected** **(** :ref:`String<class_String>` path **)**

Emitted when a file is selected.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_signal_files_selected:

.. rst-class:: classref-signal

**files_selected** **(** :ref:`PackedStringArray<class_PackedStringArray>` paths **)**

Emitted when multiple files are selected.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Enumerations
------------

.. _enum_EditorFileDialog_FileMode:

.. rst-class:: classref-enumeration

enum **FileMode**:

.. _class_EditorFileDialog_constant_FILE_MODE_OPEN_FILE:

.. rst-class:: classref-enumeration-constant

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **FILE_MODE_OPEN_FILE** = ``0``

The **EditorFileDialog** can select only one file. Accepting the window will open the file.

.. _class_EditorFileDialog_constant_FILE_MODE_OPEN_FILES:

.. rst-class:: classref-enumeration-constant

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **FILE_MODE_OPEN_FILES** = ``1``

The **EditorFileDialog** can select multiple files. Accepting the window will open all files.

.. _class_EditorFileDialog_constant_FILE_MODE_OPEN_DIR:

.. rst-class:: classref-enumeration-constant

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **FILE_MODE_OPEN_DIR** = ``2``

The **EditorFileDialog** can select only one directory. Accepting the window will open the directory.

.. _class_EditorFileDialog_constant_FILE_MODE_OPEN_ANY:

.. rst-class:: classref-enumeration-constant

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **FILE_MODE_OPEN_ANY** = ``3``

The **EditorFileDialog** can select a file or directory. Accepting the window will open it.

.. _class_EditorFileDialog_constant_FILE_MODE_SAVE_FILE:

.. rst-class:: classref-enumeration-constant

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **FILE_MODE_SAVE_FILE** = ``4``

The **EditorFileDialog** can select only one file. Accepting the window will save the file.

.. rst-class:: classref-item-separator

----

.. _enum_EditorFileDialog_Access:

.. rst-class:: classref-enumeration

enum **Access**:

.. _class_EditorFileDialog_constant_ACCESS_RESOURCES:

.. rst-class:: classref-enumeration-constant

:ref:`Access<enum_EditorFileDialog_Access>` **ACCESS_RESOURCES** = ``0``

The **EditorFileDialog** can only view ``res://`` directory contents.

.. _class_EditorFileDialog_constant_ACCESS_USERDATA:

.. rst-class:: classref-enumeration-constant

:ref:`Access<enum_EditorFileDialog_Access>` **ACCESS_USERDATA** = ``1``

The **EditorFileDialog** can only view ``user://`` directory contents.

.. _class_EditorFileDialog_constant_ACCESS_FILESYSTEM:

.. rst-class:: classref-enumeration-constant

:ref:`Access<enum_EditorFileDialog_Access>` **ACCESS_FILESYSTEM** = ``2``

The **EditorFileDialog** can view the entire local file system.

.. rst-class:: classref-item-separator

----

.. _enum_EditorFileDialog_DisplayMode:

.. rst-class:: classref-enumeration

enum **DisplayMode**:

.. _class_EditorFileDialog_constant_DISPLAY_THUMBNAILS:

.. rst-class:: classref-enumeration-constant

:ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>` **DISPLAY_THUMBNAILS** = ``0``

The **EditorFileDialog** displays resources as thumbnails.

.. _class_EditorFileDialog_constant_DISPLAY_LIST:

.. rst-class:: classref-enumeration-constant

:ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>` **DISPLAY_LIST** = ``1``

The **EditorFileDialog** displays resources as a list of filenames.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_EditorFileDialog_property_access:

.. rst-class:: classref-property

:ref:`Access<enum_EditorFileDialog_Access>` **access** = ``0``

.. rst-class:: classref-property-setget

- void **set_access** **(** :ref:`Access<enum_EditorFileDialog_Access>` value **)**
- :ref:`Access<enum_EditorFileDialog_Access>` **get_access** **(** **)**

The location from which the user may select a file, including ``res://``, ``user://``, and the local file system.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_current_dir:

.. rst-class:: classref-property

:ref:`String<class_String>` **current_dir**

.. rst-class:: classref-property-setget

- void **set_current_dir** **(** :ref:`String<class_String>` value **)**
- :ref:`String<class_String>` **get_current_dir** **(** **)**

The currently occupied directory.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_current_file:

.. rst-class:: classref-property

:ref:`String<class_String>` **current_file**

.. rst-class:: classref-property-setget

- void **set_current_file** **(** :ref:`String<class_String>` value **)**
- :ref:`String<class_String>` **get_current_file** **(** **)**

The currently selected file.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_current_path:

.. rst-class:: classref-property

:ref:`String<class_String>` **current_path**

.. rst-class:: classref-property-setget

- void **set_current_path** **(** :ref:`String<class_String>` value **)**
- :ref:`String<class_String>` **get_current_path** **(** **)**

The file system path in the address bar.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_disable_overwrite_warning:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **disable_overwrite_warning** = ``false``

.. rst-class:: classref-property-setget

- void **set_disable_overwrite_warning** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_overwrite_warning_disabled** **(** **)**

If ``true``, the **EditorFileDialog** will not warn the user before overwriting files.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_display_mode:

.. rst-class:: classref-property

:ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>` **display_mode** = ``0``

.. rst-class:: classref-property-setget

- void **set_display_mode** **(** :ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>` value **)**
- :ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>` **get_display_mode** **(** **)**

The view format in which the **EditorFileDialog** displays resources to the user.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_file_mode:

.. rst-class:: classref-property

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **file_mode** = ``4``

.. rst-class:: classref-property-setget

- void **set_file_mode** **(** :ref:`FileMode<enum_EditorFileDialog_FileMode>` value **)**
- :ref:`FileMode<enum_EditorFileDialog_FileMode>` **get_file_mode** **(** **)**

The dialog's open or save mode, which affects the selection behavior. See :ref:`FileMode<enum_EditorFileDialog_FileMode>`.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_filters:

.. rst-class:: classref-property

:ref:`PackedStringArray<class_PackedStringArray>` **filters** = ``PackedStringArray()``

.. rst-class:: classref-property-setget

- void **set_filters** **(** :ref:`PackedStringArray<class_PackedStringArray>` value **)**
- :ref:`PackedStringArray<class_PackedStringArray>` **get_filters** **(** **)**

The available file type filters. For example, this shows only ``.png`` and ``.gd`` files: ``set_filters(PackedStringArray(["*.png ; PNG Images","*.gd ; GDScript Files"]))``. Multiple file types can also be specified in a single filter. ``"*.png, *.jpg, *.jpeg ; Supported Images"`` will show both PNG and JPEG files when selected.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_show_hidden_files:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **show_hidden_files** = ``false``

.. rst-class:: classref-property-setget

- void **set_show_hidden_files** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_showing_hidden_files** **(** **)**

If ``true``, hidden files and directories will be visible in the **EditorFileDialog**. This property is synchronized with :ref:`EditorSettings.filesystem/file_dialog/show_hidden_files<class_EditorSettings_property_filesystem/file_dialog/show_hidden_files>`.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_EditorFileDialog_method_add_filter:

.. rst-class:: classref-method

void **add_filter** **(** :ref:`String<class_String>` filter, :ref:`String<class_String>` description="" **)**

Adds a comma-delimited file name ``filter`` option to the **EditorFileDialog** with an optional ``description``, which restricts what files can be picked.

A ``filter`` should be of the form ``"filename.extension"``, where filename and extension can be ``*`` to match any string. Filters starting with ``.`` (i.e. empty filenames) are not allowed.

For example, a ``filter`` of ``"*.tscn, *.scn"`` and a ``description`` of ``"Scenes"`` results in filter text "Scenes (\*.tscn, \*.scn)".

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_clear_filters:

.. rst-class:: classref-method

void **clear_filters** **(** **)**

Removes all filters except for "All Files (\*)".

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_get_line_edit:

.. rst-class:: classref-method

:ref:`LineEdit<class_LineEdit>` **get_line_edit** **(** **)**

Returns the LineEdit for the selected file.

\ **Warning:** This is a required internal node, removing and freeing it may cause a crash. If you wish to hide it or any of its children, use their :ref:`CanvasItem.visible<class_CanvasItem_property_visible>` property.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_get_vbox:

.. rst-class:: classref-method

:ref:`VBoxContainer<class_VBoxContainer>` **get_vbox** **(** **)**

Returns the ``VBoxContainer`` used to display the file system.

\ **Warning:** This is a required internal node, removing and freeing it may cause a crash. If you wish to hide it or any of its children, use their :ref:`CanvasItem.visible<class_CanvasItem_property_visible>` property.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_invalidate:

.. rst-class:: classref-method

void **invalidate** **(** **)**

Notify the **EditorFileDialog** that its view of the data is no longer accurate. Updates the view contents on next view update.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
