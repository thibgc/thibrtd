=================
Inline Formatting
=================

.. contents:: :local:

Italic
======

Source:

.. code-block:: rst

   This is normal. *This is italic.* This is normal again.

Result:

This is normal. *This is italic.* This is normal again.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#emphasis

Bold
====

Source:

.. code-block:: rst

   This is normal. **This is bold.** This is normal again.

Result:

This is normal. **This is bold.** This is normal again.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#strong-emphasis

Literals
========

Source:

.. code-block:: rst

   This is normal. ``This is literal.`` This is normal again.

Result:

This is normal. ``This is literal.`` This is normal again.

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#inline-literals

Rubric
======

A ``rubric`` is rendered as an interstitial heading but does not become part of the structural hierarchy of the document.

Source:

.. code-block:: rst

   This is a paragraph.

   .. rubric:: This is a rubric

   This is another paragraph.

Result:

This is a paragraph.

.. rubric:: This is a rubric

This is another paragraph.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/directives.html#rubric

