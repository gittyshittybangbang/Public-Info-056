.. Tip - just do it:
   don't use TABs (= \t, tabulators)
   replace each TAB by *three blanks* (enable RegExp for Search and Replace in your IDE)
   set TAB width and indentation to THREE in your IDE
   set 'Use blanks instead of TABs' in your IDE


.. With the following include we import some definition. We do this in each and every file.
   so we can change the definition at a single place. Use the relative path to the Includes.txt file,
   which may look as well like ../../../Includes.txt for a deeply nested source file.

.. include:: ../Includes.txt


.. Usually we define 'php' as default highlight language in Includes.txt.
   With the following 'highlight' directive we switch to reStructuredText as default highlight language.

.. highlight:: rst


.. The following, first section (= headline) is the 'Document Title'.


===============
To be clarified
===============

Automatic bolding of bullet items
=================================

* This is not a bullet list but a DT item of a DL
    * This is the DD

..

* this is a bullet list (line 1)

  * this is a bullet sublist
  
* some more text (line 2)


* another bullet list
* this is a bullet sublist
* some more text



**See:**

* `list and bullets <http://openalea.gforge.inria.fr/doc/openalea/doc/_build/html/source/sphinx/rest_syntax.html#list-and-bullets>`__
