.. With the following include we import some definition. We do this in each and every file.
   so we can change the definition at a single place. Use the relative path to the Includes.txt file,
   which may look as well like ../../../Includes.txt for a deeply nested source file.

.. include:: ../Includes.txt


.. Usually we define 'php' as default highlight language in Includes.txt.
   With the following 'highlight' directive we switch to reStructuredText as default highlight language.

.. highlight:: rst


.. The following, first section (= headline) is the 'Document Title'.


========================================
Drafts and Ideas for TYPO3 documentation
========================================

.. toctree::
   :hidden:
   :glob:


   GeneralThings/Index
   DocsTypo3OrgHomepage/Index
   *

