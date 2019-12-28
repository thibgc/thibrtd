=====
Links
=====

.. contents:: :local:

External Links
==============

External links can be **bare**, **direct** (```TTT <URL>`_``) or **indirect** (defined by ``.. _TTT: URL`` and referenced by ```TTT`_``).

Source:

.. code-block:: rst

   *  Bare link: http://www.example.com/

   *  Link with direct reference: Link with `direct reference <http://www.example.com/direct>`_.

   *  Link with indirect reference: Link with `indirect reference`_

   .. _indirect reference: http://www.example.com/indirect

Result:

*  Bare link: http://www.example.com/

*  Link with direct reference (```TTT <URL>`_``): Link with `direct reference <http://www.example.com/direct>`_.

*  Link with indirect reference (``.. _TTT: URL`` and ```TTT`_``): Link with `indirect reference`_

.. _indirect reference: http://www.example.com/indirect

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#hyperlink-targets
*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#hyperlink-references
*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#hyperlinks

Internal Links
==============

Section headings are named by preceding them with ``.. LLL:``, and referenced with ``:ref:`LLL``` (note: no trailing underscore).

Source:

.. code-block:: rst

   For more information, see :ref:`fakesection`.

   .. _fakesection:

   Fake Section
   ------------

   This is a fake section.

Result:

For more information, see :ref:`fakesection`.

.. _fakesection:

Fake Section
------------

This is a fake section.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#hyperlink-targets
*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#inline-internal-targets
*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/roles.html#ref-role

Footnotes
=========

Footnotes are defined with ``.. [#LLL]`` and referenced with ``[#LLL]_`` (compare both with the lack of ``#`` in citations).

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
*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#footnote-references
*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#footnotes

Citations
=========

LaTeX-style, single-keyword citations are defined with ``.. [LLL]`` and referenced with ``[LLL]_`` (compare both with the ``#`` in footnotes).

Source:

.. code-block:: rst

   LaTeX-style citations are supported [RFC2119]_ .

   .. rubric:: Citations

   .. [RFC2119]

      Body of ``RFC2119`` citation: https://tools.ietf.org/rfc/rfc2119.txt

      If the body fits on one line, can be on the same line as ``..``.

Result:

LaTeX-style citations are supported [RFC2119]_ .

.. rubric:: Citations

.. [RFC2119]

   Body of ``RFC2119`` citation: https://tools.ietf.org/rfc/rfc2119.txt

   If the body fits on one line, can be on the same line as ``..``.

.. tip::

   Standard reStructuredText citations are per-file, but Sphinx makes citations global.

   In local PDF output, citations are grouped together into a *Bibliography* appendix. In HTML output, citations are rendered wherever they are defined. This makes the toy example above impractical as a single source for both HTML and PDF.

   References:

   *  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#citations

References:

*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#citations
*  https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#citation-references
*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#citations

