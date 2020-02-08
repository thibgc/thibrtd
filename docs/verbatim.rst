========
Verbatim
========

.. contents:: :local:

----
Code
----

.. tip::

   This directive is part of basic reStructuredText, but has fewer features than its Sphinx counterparts ``code-block`` and ``literalinclude``, which are recommended instead.

   References:

   *  https://stackoverflow.com/questions/34845889/whats-the-difference-between-the-code-and-code-block-directives-in-rest/35174436#35174436

Source:

.. code-block:: rst

   .. code:: java

      public static void main(String[] args) {
        System.out.println("Hello world!");
      }

Result:

.. code:: java

   public static void main(String[] args) {
     System.out.println("Hello world!");
   }

Source:

.. code-block:: rst

   .. code:: java
      :number-lines:

      public static void main(String[] args) {
        System.out.println("Hello world!");
      }

Result:

.. code:: java
   :number-lines:

   public static void main(String[] args) {
     System.out.println("Hello world!");
   }

Source:

.. code-block:: rst

   .. code:: java
      :number-lines: 123

      public static void main(String[] args) {
        System.out.println("Hello world!");
      }

Result:

.. code:: java
   :number-lines: 123

   public static void main(String[] args) {
     System.out.println("Hello world!");
   }

Notes:

*  The language keywords accepted are those accepted by Pygments.

References:

*  https://docutils.sourceforge.io/docs/ref/rst/directives.html#code
*  https://pygments.org/docs/lexers/

----------
Code Block
----------

.. note::

   This directive is part of Sphinx.

.. admonition:: PDF Output

   In HTML output, ``code`` and ``code-block`` look the same, but in PDF output, ``code-block`` is rendered inside a boxed area, with small, ``a2ps``-style line numbers outside the boxed area.

Source:

.. code-block:: rst

   .. code-block:: java

      public static void main(String[] args) {
        System.out.println("Hello world!");
      }

Result:

.. code-block:: java

   public static void main(String[] args) {
     System.out.println("Hello world!");
   }

Source:

.. code-block:: rst

   .. code-block:: java
      :linenos:

      public static void main(String[] args) {
        System.out.println("Hello world!");
      }

Result:

.. code-block:: java
   :linenos:

   public static void main(String[] args) {
     System.out.println("Hello world!");
   }

Source:

.. code-block:: rst

   .. code-block:: java
      :lineno-start: 123

      public static void main(String[] args) {
        System.out.println("Hello world!");
      }

Result:

.. code-block:: java
   :lineno-start: 123

   public static void main(String[] args) {
     System.out.println("Hello world!");
   }

Source:

.. code-block:: rst

   .. code-block:: java
      :emphasize-lines: 2,3

      public static void main(String[] args) {
        // These two lines are highlighted
        System.out.println("Hello world!");
      }

Result:

.. code-block:: java
   :emphasize-lines: 2,3

   public static void main(String[] args) {
     // These two lines are highlighted
     System.out.println("Hello world!");
   }

Source:

.. code-block:: rst

   .. code-block:: java
      :caption: Title of the code block

      public static void main(String[] args) {
        System.out.println("Hello world!");
      }

Result:

.. code-block:: java
   :caption: Title of the code block

   public static void main(String[] args) {
     System.out.println("Hello world!");
   }

Source:

.. code-block:: rst

   .. code-block:: java
      :dedent: 8

                  These lines have source with 11 leading spaces:
                  3 to align with the ``c`` of ``.. code-block``
                  (by convention) and 12 proper ones. But the
                  result is rendered with only 4 leading spaces,
                  after being "de-indented" by 8.

Result:

.. code-block:: none
   :dedent: 8

               These lines have source with 11 leading spaces:
               3 to align with the ``c`` of ``.. code-block``
               (by convention) and 12 proper ones. But the
               result is rendered with only 4 leading spaces,
               after being "de-indented" by 8.

References:

*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#directive-code-block
*  https://pygments.org/docs/lexers/

---------------
Literal Include
---------------

.. note::

   This directive is part of Sphinx.

The ``literalinclude`` directive is similar to ``code-block`` but takes its source from an external file. It has the same basic options, except that ``code-block``'s direct argument is a Pygments language code whereas ``literalinclude``'s is a file path, meaning the Pygments language keyword is specified with the ``:language:`` option instead.

It also accepts these additional options:

*  ``:encoding:``: a file encoding like ``latin-1``.

*  ``:lines:``: the comma-separated list of line numbers (e.g. ``3``) or line number ranges either closed (e.g. ``23-45``) or open (e.g. ``-77`` or ``99-``) controls which lines from the external file are actually included.

*  ``:start-after:`` and ``:end-before:``: these independent options can be used to include only lines of the external file strictly after or strictly before (respectively) the first line containing the string given as an argument.

*  ``:start-at:`` and ``:end-at:``: similar to ``:start-after:`` and ``:end-before:``, but also includes the matched line in the output.

*  ``:prepend:`` and ``:append:``: prepend or append (respectively) the line given as argument to the output.

*  ``:diff:``: this option accepts another file path as argument and displays the unified diff from the ``:diff:`` argument file to the ``literalinclude`` argument file.

References:

*  https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html
*  https://pygments.org/docs/lexers/
