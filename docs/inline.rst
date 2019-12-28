======
Inline
======

.. contents:: :local:

Italic
======

Preferred: ``*TTT*``

Synonyms: ``:emphasis:`TTT```

Source:

.. code-block:: rst

   This is normal. *This is italic.* This is normal again.

Result:

This is normal. *This is italic.* This is normal again.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#emphasis
*  https://docutils.sourceforge.io/docs/ref/rst/roles.html#emphasis
*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#inline-markup

Bold
====

Preferred: ``**TTT**``

Synonyms: ``:strong:`TTT```

Source:

.. code-block:: rst

   This is normal. **This is bold.** This is normal again.

Result:

This is normal. **This is bold.** This is normal again.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#strong-emphasis
*  https://docutils.sourceforge.io/docs/ref/rst/roles.html#strong
*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#inline-markup

Literal
=======

Preferred: `````TTT`````

Synonyms: ``:literal:`TTT```

Source:

.. code-block:: rst

   This is normal. ``This is literal.`` This is normal again.

Result:

This is normal. ``This is literal.`` This is normal again.

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#inline-literals
*  https://docutils.sourceforge.io/docs/ref/rst/roles.html#literal
*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#inline-markup

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

Superscript
===========

Preferred: ``:sup:``

Synonyms: ``:superscript:``

Source:

.. code-block:: rst

   Plot the parabola y=x\ :sup:`2`\ +1.

Result:

Plot the parabola y=x\ :sup:`2`\ +1.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/roles.html#superscript

Subscript
=========

Preferred: ``:sub:``

Synonyms: ``:subscript:``

Source:

.. code-block:: rst

   Water is H\ :sub:`2`\ O.

Result:

Water is H\ :sub:`2`\ O.

References:

*  http://docutils.sourceforge.net/docs/ref/rst/roles.html#subscript

Semantic Markup
===============

.. note::

   These roles are part of Sphinx.

Result:

*  ``:command:`` for an OS command: Type :command:`rm`

*  ``:file:`` for a path: Edit :file:`/etc/resolv.conf` .

   *  Use curly braces for a variable portion: Installed in :file:`/usr/lib/python2.{x}/site-packages` .

*  ``:guilabel:`` for a GUI label: Click :guilabel:`OK` .

   *  Precede a letter accelerator with an ampersand: Click :guilabel:`&Cancel` .

   *  Use a double ampersand for a literal ampersand: Click :guilabel:`Save && Restart` .

