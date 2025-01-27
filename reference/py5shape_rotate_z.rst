.. title: Py5Shape.rotate_z()
.. slug: py5shape_rotate_z
.. date: 2021-05-01 20:51:42 UTC+00:00
.. tags:
.. category:
.. link:
.. description: py5 Py5Shape.rotate_z() documentation
.. type: text

Rotates the shape around the z-axis the amount specified by the ``angle`` parameter.

Examples
========

.. raw:: html

    <div class="example-table">

.. raw:: html

    <div class="example-row"><div class="example-cell-image">

.. raw:: html

    </div><div class="example-cell-code">

.. code:: python
    :number-lines:

    def settings():
        py5.size(100, 100, py5.P3D)


    def setup():
        global s
        s = py5.load_shape("bot.svg")


    def draw():
        py5.background(204)
        py5.scale(0.2)
        py5.shape(s, py5.width//2, py5.height//2)


    def mouse_pressed():
        # rotate the shape around the z-axis each time the mouse is pressed
        s.rotate_z(0.1)

.. raw:: html

    </div></div>

.. raw:: html

    </div>

Description
===========

Rotates the shape around the z-axis the amount specified by the ``angle`` parameter. Angles should be specified in radians (values from 0 to ``TWO_PI``) or converted from degrees to radians with the :doc:`radians` method.

Shapes are always rotated around the upper-left corner of their bounding box. Positive numbers rotate objects in a clockwise direction. Subsequent calls to the method accumulates the effect. For example, calling ``rotate_z(HALF_PI)`` and then ``rotate_z(HALF_PI)`` is the same as ``rotate_z(PI)``. This transformation is applied directly to the shape, it's not refreshed each time ``draw()`` is run. 

This method requires a 3D renderer. You need to use ``P3D`` as a third parameter for the :doc:`size` function as shown in the example.

Underlying Java method: `PShape.rotateZ <https://processing.org/reference/PShape_rotateZ_.html>`_

Syntax
======

.. code:: python

    rotate_z(angle: float, /) -> None

Parameters
==========

* **angle**: `float` - angle of rotation specified in radians


Updated on May 01, 2021 20:51:42pm UTC

