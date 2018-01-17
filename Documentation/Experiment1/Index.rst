
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


Links
=====

::

   Use `Link text <http://example.com/>`_ for inline web links.

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

* `Source Code <http://www.sphinx-doc.org/en/stable/rest.html#source-code/>`_

Tables
======

=====  =====    =======
       Average  Total
=====  =====    =======
Jan    2.7      3.1
Feb    3.4      2.0
=====  =====    =======


References:

* `Tables <http://www.sphinx-doc.org/en/stable/rest.html#tables/>`_

References
==========


#. reStructured Text Primer: http://www.sphinx-doc.org/en/stable/rest.html


