======
Images
======

.. contents:: :local:

Image
=====

The ``image`` directive accepts the optional parameters ``:alt:``, ``:height:``, ``:width:``, ``:scale:``, ``:align:`` and ``:target:`` (see `definition <https://docutils.sourceforge.io/docs/ref/rst/directives.html#images>`_).

Source:

.. code-block:: rst

   .. image:: /images/test-image.png
      :alt: HTML alt text
      :width: 100px

Result:

.. image:: /images/test-image.png
   :alt: HTML alt text
   :width: 100px

References:

*  https://docutils.sourceforge.io/docs/ref/rst/directives.html#images
*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#images

Figure
======

The ``figure`` directive accepts an image file path as its direct argument; the first paragraph of its body is rendered as the caption and the remainder of its body as the "legend" (arbitrary body elements). It supports the same options as the ``image`` directive, plus ``:figwidth:``.

Source:

.. code-block:: rst

   .. figure:: /images/test-image.png
      :alt: HTML alt text

      This is the caption.

      This is the legend, paragraph 1.

      This is the legend, paragraph 2.

Result:

.. figure:: /images/test-image.png
   :alt: HTML alt text

   This is the caption.

   This is the legend, paragraph 1.

   This is the legend, paragraph 2.

In HTML, the rendering is above.

In PDF, the rendering is on a page of its own.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/directives.html#figure


