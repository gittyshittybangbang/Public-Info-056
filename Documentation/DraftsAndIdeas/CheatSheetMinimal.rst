.. this is used to create the .odt / .pdf cheat sheet

.. include:: ../Includes.txt
.. highlight:: php

.. _rest-cheat sheet:
=========================
reST & Sphinx Cheat Sheet
=========================

This is a Header Level 1
========================

This is a Header Level 2
------------------------

Links
=====

* `external link <https://typo3.org>`__,
* :ref:`Cross reference to section in this manual <intersphinx>`,
* :ref:`intersphinx`,
* :ref:`Cross reference to section in OTHER manual <t3tsref:start>`,
* :ref:`t3tsref:start`


.. t3-field-list-table::
 :header-rows: 1

 - :Anchor:
   :ThisManual:   Link to this manual
   :OtherManual:  Other manual

 - :Anchor:       **Explicit anchor**
   :ThisManual:   1) :ref:`Cross Reference <intersphinx>`
   :OtherManual:  2) :ref:`TSref <t3tsref:start>`

 - :Anchor:       **Automatic anchor**
   :ThisManual:   3) :ref:`intersphinx`
   :OtherManual:  4) :ref:`t3tsref:start`


This is a bullet list:

* list item 1
* list item 2

More text.

.. code-block:: php

   $a = 'one';

::

   $a = 'two';

Another example::

   $a = 'three';


#. :php:`$result = $a + 23;` (PHP snippet)
#. :typoscript:`lib.hello.value = Hello World!` (TypoScript snippets)
#. :file:`/etc/passwd` (file)
#. :kbd:`ctrl` + :kbd:`s` (keyboard strokes)


.. image:: ../images/a4.jpg
   :class: with-shadow


Normal text, **bold text** and *italic text*.


.. youtube:: wNxO-aXY5Yw
