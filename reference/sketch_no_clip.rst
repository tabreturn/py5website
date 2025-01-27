.. title: no_clip()
.. slug: no_clip
.. date: 2021-03-03 21:11:14 UTC+00:00
.. tags:
.. category:
.. link:
.. description: py5 no_clip() documentation
.. type: text

Disables the clipping previously started by the :doc:`clip` function.

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
        py5.size(200, 200)


    def setup():
        py5.image_mode(py5.CENTER)


    def draw():
        py5.background(204)
        if py5.is_mouse_pressed:
            py5.clip(py5.mouse_x, py5.mouse_y, 100, 100)
        else:
            py5.no_clip()

        py5.line(0, 0, py5.width, py5.height)
        py5.line(0, py5.height, py5.width, 0)

.. raw:: html

    </div></div>

.. raw:: html

    </div>

Description
===========

Disables the clipping previously started by the :doc:`clip` function.

Underlying Java method: `noClip <https://processing.org/reference/noClip_.html>`_

Syntax
======

.. code:: python

    no_clip() -> None

Updated on March 03, 2021 21:11:14pm UTC

