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

Source:

.. code-block:: rst

   *  ``:command:`` for an named executable: Use :command:`rsync` or :command:`scp` .

   *  ``:envvar:`` for an environment variable: Set :envvar:`JAVA_HOME` .

   *  ``:file:`` for a path, with variable portions in curly braces: Edit :file:`/home/{user}/.myconf` .

      *  Use curly braces for a variable portion: Installed in :file:`/usr/lib/python2.{x}/site-packages` .

   *  ``:guilabel:`` for a GUI label, with an ampersand preceding an accelerator key (use double ampersand for a literal ampersand): Click :guilabel:`Cancel` .

   *  ``:kbd:`` for a keystroke sequence: Hit :kbd:`Ctrl+C` .

   *  ``:menuselection:`` for a menu sequence, separated by ``-->``: Select :menuselection:`Edit --> Copy`

   *  ``:mimetype:`` for a MIME type or portion thereof: The :mimetype:`text/plain` MIME type.

   *  ``:program:`` for a typed executable: Type :program:`exit` to log out.

   *  ``:regexp:`` for a regular expression: Use :regexp:`^([^#]*)#?` to ignore comments.

   *  ``:samp:`` for literal text, with variable parts in curly braces (use backslash to escape literal curly braces): Type :samp:`sleep {secs}` .

Result:

*  ``:command:`` for an named executable: Use :command:`rsync` or :command:`scp` .

*  ``:envvar:`` for an environment variable: Set :envvar:`JAVA_HOME` .

*  ``:file:`` for a path, with variable portions in curly braces: Edit :file:`/home/{user}/.myconf` .

   *  Use curly braces for a variable portion: Installed in :file:`/usr/lib/python2.{x}/site-packages` .

*  ``:guilabel:`` for a GUI label, with an ampersand preceding an accelerator key (use double ampersand for a literal ampersand): Click :guilabel:`Cancel` .

*  ``:kbd:`` for a keystroke sequence: Hit :kbd:`Ctrl+C` .

*  ``:menuselection:`` for a menu sequence, separated by ``-->``: Select :menuselection:`Edit --> Copy`

*  ``:mimetype:`` for a MIME type or portion thereof: The :mimetype:`text/plain` MIME type.

*  ``:program:`` for a typed executable: Type :program:`exit` to log out.

*  ``:regexp:`` for a regular expression: Use :regexp:`^([^#]*)#?` to ignore comments.

*  ``:samp:`` for literal text, with variable parts in curly braces (use backslash to escape literal curly braces): Type :samp:`sleep {secs}` .

Notes:

*  ``:guilabel:`` seems to have bugs. In HTML output, the accelerator key surrounds the affected character with a distinguishable ``<span>`` but seemingly not resulting in a different visual. In PDF output, the double ampersand remains without being escaped to a single ampersand.

References:

*  http://www.sphinx-doc.org/en/master/usage/restructuredtext/roles.html#cross-referencing-other-items-of-interest
*  http://www.sphinx-doc.org/en/master/usage/restructuredtext/roles.html#other-semantic-markup

