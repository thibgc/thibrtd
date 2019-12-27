=====
Links
=====

.. contents:: :local:

Hyperlinks
==========

Source:

.. code-block:: rst

   This is a bare link: http://www.example.com/

   This is a link with `link text <http://www.example.com/linktext>`_.

   Rather than repeatedly linking to the same URL with the same link text, you can define the mapping from the link text to the URL like this:

   .. _defined link text: http://www.example.com/definedlink

   and make multiple references to it by link text alone: one reference to the `defined link text`_, another reference to the `defined link text`_.

   The same directive without a URL simply names its location in the current document:

   .. _internal link text:

   You can then reference it by the `internal link text`_.

Result:

This is a bare link: http://www.example.com/

This is a link with `link text <http://www.example.com/linktext>`_.

Rather than repeatedly linking to the same URL with the same link text, you can define the mapping from the link text to the URL like this:

.. _defined link text: http://www.example.com/definedlink

and make multiple references to it by link text alone: one reference to the `defined link text`_, another reference to the `defined link text`_.

The same directive without a URL simply names its location in the current document:

.. _internal link text:

You can then reference it by the `internal link text`_.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#hyperlink-targets
*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#hyperlinks

Footnotes
=========

Source:

.. code-block:: rst

   This is a reference to a footnote labeled f1 [#f1]_ . This is also a reference to f1 [#f1]_ .

   .. rubric:: Footnotes

   .. [#f1]

      Body of footnote f1.

      If the body fits on one line, can be on the same line as ``..``.

Result:

This is a reference to a footnote labeled f1 [#f1]_ . This is also a reference to f1 [#f1]_ .

.. rubric:: Footnotes

.. [#f1]

   Body of footnote f1.

   If the body fits on one line, can be on the same line as ``..``.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#footnotes
*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#footnotes

Citations
=========

Source:

Result:

LaTeX-style single-keyword citations are supported [RFC2119]_ .

.. rubric:: Citations

.. [RFC2119]

   Body of ``RFC2119`` citation: https://tools.ietf.org/rfc/rfc2119.txt

   If the body fits on one line, can be on the same line as ``..``.

.. tip::

   Standard reStructuredText citations are per-file, but Sphinx makes citations global.

   References:

   *  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#citations

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#citations
*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#citations

