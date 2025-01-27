.. title: Py5Shape.set_specular()
.. slug: py5shape_set_specular
.. date: 2021-05-01 20:51:42 UTC+00:00
.. tags:
.. category:
.. link:
.. description: py5 Py5Shape.set_specular() documentation
.. type: text

Sets the specular color of a ``Py5Shape`` object's material, which sets the color of highlight.

Examples
========

.. raw:: html

    <div class="example-table">

.. raw:: html

    <div class="example-row"><div class="example-cell-image">

.. image:: /images/reference/Py5Shape_set_specular_0.png
    :alt: example picture for set_specular()

.. raw:: html

    </div><div class="example-cell-code">

.. code:: python
    :number-lines:

    def settings():
        py5.size(100, 100, py5.P3D)


    def setup():
        py5.background(0)
        py5.light_specular(255, 255, 255)
        py5.directional_light(204, 204, 204, 0, 0, -1)
        py5.no_stroke()
        s = py5.create_shape(py5.SPHERE, 20)

        s.set_specular(py5.color(255, 255, 255))
        py5.shape(s, 50, 25)
        s.set_specular(py5.color(204, 102, 0))
        py5.shape(s, 50, 75)

.. raw:: html

    </div></div>

.. raw:: html

    </div>

Description
===========

Sets the specular color of a ``Py5Shape`` object's material, which sets the color of highlight. This is part of the material properties of a ``Py5Shape`` object.

The ``specular`` parameter can be applied to the entire ``Py5Shape`` object or to a single vertex.

This method can only be used for a complete ``Py5Shape`` object, and never within a :doc:`py5shape_begin_shape` and :doc:`py5shape_end_shape` pair.

Underlying Java method: PShape.setSpecular

Syntax
======

.. code:: python

    set_specular(index: int, specular: int, /) -> None
    set_specular(specular: int, /) -> None

Parameters
==========

* **index**: `int` - vertex index
* **specular**: `int` - any color value


Updated on May 01, 2021 20:51:42pm UTC

