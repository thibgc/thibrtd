=====
Lists
=====

.. contents:: :local:

Bullet List
===========

Source:

.. code-block:: rst

   *  This is the first bullet list item.  The blank line above the
      first list item is required; blank lines between list items
      (such as below this paragraph) are optional.

   *  This is the first paragraph in the second item in the list.

      This is the second paragraph in the second item in the list.
      The blank line above this paragraph is required.  The left edge
      of this paragraph lines up with the paragraph above, both
      indented relative to the bullet.

      *  This is a sublist.  The bullet lines up with the left edge of
         the text blocks above.  A sublist is a new list so requires a
         blank line above and below.

   *  This is the third item of the main list.

   This paragraph is not part of the list.

Result:

*  This is the first bullet list item.  The blank line above the
   first list item is required; blank lines between list items
   (such as below this paragraph) are optional.

*  This is the first paragraph in the second item in the list.

   This is the second paragraph in the second item in the list.
   The blank line above this paragraph is required.  The left edge
   of this paragraph lines up with the paragraph above, both
   indented relative to the bullet.

   *  This is a sublist.  The bullet lines up with the left edge of
      the text blocks above.  A sublist is a new list so requires a
      blank line above and below.

*  This is the third item of the main list.

This paragraph is not part of the list.

Notes:

*  Bullet marker can be ``*``, ``-`` or ``+``.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#bullet-lists

Enumerated List
===============

Source:

.. code-block:: rst

   1. Item 1

   2. Item 2

      1. Item 2.1

      2. Item 2.2

   3. Item 3

Result:

1. Item 1

2. Item 2

   1. Item 2.1

   2. Item 2.2

3. Item 3

Notes:

*  Supported enumerators are ``1, 2, 3...``, ``A, B, C...``, ``a, b, c...``, ``I, II, III...``, ``i, ii, iii...``

*  Supported markers are followed by a dot (e.g. ``1.``), followed by a parenthesis (e.g. ``1)``), or surrounded by parentheses (e.g. ``(1)``).

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#enumerated-lists

Definition List
===============

Source:

.. code-block:: rst

   term 1
       Definition 1.

   term 2
       Definition 2, paragraph 1.

       Definition 2, paragraph 2.

Result:

term 1
    Definition 1.

term 2
    Definition 2, paragraph 1.

    Definition 2, paragraph 2.

Notes:

*  Terms can also have *qualifiers* but the rendering does not seem to work with the version of Sphinx and Sphinx_rtd_theme we are using.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#definition-lists

