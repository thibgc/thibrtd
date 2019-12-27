======
Asides
======

.. contents:: :local:

Admonitions
===========

Admonitions are side notes offset from the main body of text by a box. Examples include "Warning", "Note" and "Important". The specific admonition directives ``attention``, ``caution``, ``danger``, ``error``, ``hint``, ``important``, ``note``, ``tip``, and ``warning`` are implemented in terms of the generic ``admonition`` directive.

Admonition
----------

Source:

.. code-block:: rst

   .. admonition:: Check This Out!

      This is a generic Admonition. It has the custom title "Check This Out!"

      It can have multiple paragraphs.

Result:

.. admonition:: Check This Out!

   This is a generic Admonition. It has the custom title "Check This Out!"

   It can have multiple paragraphs.

Attention
---------

Source:

.. code-block:: rst

   .. attention::

      This is an Attention admonition.

      It can have multiple paragraphs.

Result:

.. attention::

   This is an Attention admonition.

   It can have multiple paragraphs.

Caution
-------

Source:

.. code-block:: rst

   .. caution::

      This is a Caution admonition.

      It can have multiple paragraphs.

Result:

.. caution::

   This is a Caution admonition.

   It can have multiple paragraphs.

Danger
------

Source:

.. code-block:: rst

   .. danger::

      This is a Danger admonition.

      It can have multiple paragraphs.

Result:

.. danger::

   This is a Danger admonition.

   It can have multiple paragraphs.

Error
-----

Source:

.. code-block:: rst

   .. error::

      This is an Error admonition.

      It can have multiple paragraphs.

Result:

.. error::

   This is an Error admonition.

   It can have multiple paragraphs.

Hint
----

Source:

.. code-block:: rst

   .. hint::

      This is a Hint admonition.

      It can have multiple paragraphs.

Result:

.. hint::

   This is a Hint admonition.

   It can have multiple paragraphs.

Important
---------

Source:

.. code-block:: rst

   .. important::

      This is an Important admonition.

      It can have multiple paragraphs.

Result:

.. important::

   This is an Important admonition.

   It can have multiple paragraphs.

Note
----

Source:

.. code-block:: rst

   .. note::

      This is a Note admonition.

      It can have multiple paragraphs.

Result:

.. note::

   This is a Note admonition.

   It can have multiple paragraphs.

Tip
---

Source:

.. code-block:: rst

   .. tip::

      This is a Tip admonition.

      It can have multiple paragraphs.

Result:

.. tip::

   This is a Tip admonition.

   It can have multiple paragraphs.

Warning
-------

Source:

.. code-block:: rst

   .. warning::

      This is a Warning admonition.

      It can have multiple paragraphs.

Result:

.. warning::

   This is a Warning admonition.

   It can have multiple paragraphs.

Sidebar
=======

.. sidebar:: Sidebar Title

   Subsequent indented lines comprise
   the body of the sidebar, and are
   interpreted as body elements.

Source:

.. code-block:: rst

   .. sidebar:: Sidebar Title

      Subsequent indented lines comprise
      the body of the sidebar, and are
      interpreted as body elements.

Result:

Rendered to the right.

Notes:

*  Tip: for better rendering, you may want to code the sidebar just before what it relates to, rather than just after.
*  The version of Sphinx and Sphinx_rtd_theme we use does not seem to render the ``:subtitle:`` differently.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/directives.html#sidebar

