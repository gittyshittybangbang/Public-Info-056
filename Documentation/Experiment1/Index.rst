.. With the following include we import some definition. We do this in each and every file.
   so we can change the definition at a single place. Use the relative path to the Includes.txt file,
   which may look as well like ../../../Includes.txt for a deeply nested source file.

.. include:: Includes.txt


.. Usually we define 'php' as default highlight language in Includes.txt.
   With the following 'highlight' directive we switch to reStructuredText as default highlight language.

.. highlight:: rst


.. The following, first section (= headline) is the 'Document Title'.

===========
Experiment1
===========

Some **bold** and *italic* Text.


Headers
=======

Subheader 1
-----------

Subheader 2
-----------



Links
=====


Link
----

.. highlight:: rst

::

   Use `Link text <http://example.com/>`__ for inline web links.

Links to other TYPO3 manuals
----------------------------

.. attention::
   Make sure the manuals you are referencing here are listed in Settings.cfg!

.. highlight:: rst



Link to Core API Reference:

::

   :ref:`Core API <t3coreapi:start>`

Examples:

* See :ref:`description of the TS function "parsefunc" <t3tsref:parsefunc>`
* See :ref:`HTMLparser <t3tsref:htmlparser>`
* See :ref:`Core API <t3coreapi:start>`


References:

* `Cross-referencing <http://www.sphinx-doc.org/en/stable/markup/inline.html#ref-role/>`__

Source Code Examples (PHP)
==========================

.. highlight:: php

::

   <?php
   
   namespace Sypets\Supercode\Myclass;
   
   class Myclass 
   {
      function __construct()
      {
         $this->initialize();
      }

use this for syntax highlighting:

.. highlight:: rst

::

   .. highlight:: php

   ::


References:

* `Source Code <http://www.sphinx-doc.org/en/stable/rest.html#source-code/>`__

Tables
======

=====  =======  =======
       Average  Total
=====  =======  =======
Jan    2.7      3.1
Feb    3.4      2.0
=====  =======  =======


References:

* `Tables <http://www.sphinx-doc.org/en/stable/rest.html#tables/>`__

References
==========


* `reStructured Text Primer <http://www.sphinx-doc.org/en/stable/rest.html/>`__
* `Starter Project 001 <https://docs.typo3.org/typo3cms/drafts/github/T3DocumentationStarter/Public-Info-001/StyleGuides/Index.html#/>`__


