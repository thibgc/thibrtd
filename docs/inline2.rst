===================
Other Inline Markup
===================

.. contents:: :local:

--------------------
Interstitial Heading
--------------------

A ``rubric`` is rendered as an interstitial heading but does not become part of the structural hierarchy of the document. Useful for marking the footnotes section at the end of a page.

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

-----------
Superscript
-----------

Preferred: ``:sup:`...```

Synonyms: ``:superscript:`...```

Source:

.. code-block:: rst

   Plot the parabola y = x :sup:`2` + 1.

Result:

Plot the parabola y = x :sup:`2` + 1.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/roles.html#superscript

---------
Subscript
---------

Preferred: ``:sub:`...```

Synonyms: ``:subscript:`...```

Source:

.. code-block:: rst

   Water is H :sub:`2` O.

Result:

Water is H :sub:`2` O.

References:

*  http://docutils.sourceforge.net/docs/ref/rst/roles.html#subscript

---------------
Title Reference
---------------

Used for the title of a book, periodical, etc.

Preferred: ``:title-reference:`...```

Synonyms: ``:title:`...```, ``:t:`...```

Source:

.. code-block:: rst

   :title-reference:`Design Patterns` is a great book.

Result:

:title-reference:`Design Patterns` is a great book.

References:

*  http://docutils.sourceforge.net/docs/ref/rst/roles.html#title-reference

---------------
Semantic Markup
---------------

.. note::

   These roles are part of Sphinx.

Sphinx defines a number of roles for semantic markup.

``:abbr:`AAA (expansion of AAA)```

   Abbreviation and expansion.

   ``:abbr:`FTP (File Transfer Protocol)``` -> :abbr:`FTP (File Transfer Protocol)`

``:command:`...```

   OS-level command.

   ``:command:`rm``` -> :command:`rm`

``:dfn:`...```

   Defining instance of a term.

   ``:dfn:`LOCKSS``` -> :dfn:`LOCKSS`

``:file:`...```

   File or directory name.

   Within the contents, you can use curly braces to indicate a variable part

   ``:file:`/usr/lib/python2.{x}/site-packages``` -> :file:`/usr/lib/python2.{x}/site-packages`

``:guilabel:`...```

   UI labels (button text, field name...)

   Within the contents, an accelerator key can be marked specially by preceding it with an ampersand (two ampersands result in a literal ampersand).

   ``:guilabel:`&Cancel``` -> :guilabel:`&Cancel`

``:kbd:`...```

   Sequence of keystrokes.

   ``:kbd:`Control + Alt + Delete``` -> :kbd:`Control + Alt + Delete`

``:mailheader:`...```

   Mail or HTTP header.

   ``:mailheader:`Content-Type``` -> :mailheader:`Content-Type`

``:manpage:`COMMAND(N)```

   Unix :command:`man` page and section

   ``:manpage:`ls(1)``` -> :manpage:`ls(1)`

``:menuselection:``

   A menu selection sequence, separated by ``-->``.

   Supports ampersand accelerators like ``:guilabel:``.

   ``:menuselection:`Edit --> Copy``` -> :menuselection:`Edit --> Copy`

``:mimetype:``

   Media type, or major or minor portion of a media type.

   ``:mimetype:`text/html``` -> :mimetype:`text/html`

``:program:``

   Executable program.

   ``:program:`configure.sh``` -> :program:`configure.sh`

``:regexp:``

   Regular expression.

   ``:regexp:`^ab*c$``` -> :regexp:`^ab*c$`

``:samp:``

   Piece of sample text.

   Within the contents, you can use curly braces to indicate a variable part, as in ``:file:``. Curly braces are escaped with a backslash.

   ``:samp:`print {variable} + 1``` -> ``:samp:`print {variable} + 1`

Notes:

*  ``:guilabel:`` seems to have bugs. In HTML output, the accelerator key surrounds the affected character with a distinguishable ``<span>`` but seemingly not resulting in a different visual. In PDF output, the double ampersand remains without being escaped to a single ampersand.

References:

*  http://www.sphinx-doc.org/en/master/usage/restructuredtext/roles.html#other-semantic-markup
