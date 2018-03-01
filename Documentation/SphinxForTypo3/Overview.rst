.. With the following include we import some definition. We do this in each and every file.
   so we can change the definition at a single place. Use the relative path to the Includes.txt file,
   which may look as well like ../../../Includes.txt for a deeply nested source file.

.. include:: ../Includes.txt


.. Usually we define 'php' as default highlight language in Includes.txt.
   With the following 'highlight' directive we switch to reStructuredText as default highlight language.

.. highlight:: rst


.. The following, first section (= headline) is the 'Document Title'.

==========================================
Sphinx for TYPO3 Hints: Overview (Sybille)
==========================================


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

1. Look for the shorthand name of the manual in Settings.cfg. Here: t3coreapi
2. Look for the section name of the page / section you want to reference 

If the section name is

::

   .. _parsefunc:
   
you need to use

::

   <t3coreapi:parsefunc>

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


Images
======

Apparently, floating images are not possible? https://stackoverflow.com/questions/16463051/how-to-create-floating-figures-in-restructuredtext-sphinx

But it seems to work ...

.. highlight:: rst

::

   .. image:: _assets/slack.png
   :width: 200px
   :align: left
   :height: 100px
   :alt: Register for TYPO3's Slack Platform


References
==========


* `reStructured Text Primer <http://www.sphinx-doc.org/en/stable/rest.html/>`__
* `Starter Project 001 <https://docs.typo3.org/typo3cms/drafts/github/T3DocumentationStarter/Public-Info-001/StyleGuides/Index.html#/>`__


