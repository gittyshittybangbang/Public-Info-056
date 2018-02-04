.. With the following include we import some definition. We do this in each and every file.
   so we can change the definition at a single place. Use the relative path to the Includes.txt file,
   which may look as well like ../../../Includes.txt for a deeply nested source file.

.. include:: Includes.txt


.. Usually we define 'php' as default highlight language in Includes.txt.
   With the following 'highlight' directive we switch to reStructuredText as default highlight language.

.. highlight:: rst


.. The following, first section (= headline) is the 'Document Title'.

================
Sphinx for TYPO3
================

Resources for documenting TYPO3:

* `demo docs <https://docs.typo3.org/typo3cms/drafts/github/TYPO3-Documentation/t3SphinxThemeRtdDemoDocs/Index.html>`__
* `TYPO3 Worx: Guide to TYPO3 documentation, part 3 <https://typo3worx.eu/2017/02/guide-to-typo3-documentation-part-3-contribute/>`__


.. toctree::
   :hidden:

   
   MartinsIntro
   Overview
   Hyperlinks
   reStructuredText
