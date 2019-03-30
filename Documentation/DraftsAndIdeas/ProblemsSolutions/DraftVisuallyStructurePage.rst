.. include:: ../Includes.txt

.. _solutions-visually-structure-pages:

=====================================================
Solutations for visually structuring things on a page
=====================================================

Test out and showcase some ideas.

Adresses:

* `PR for contribution guide
  <https://github.com/TYPO3-Documentation/TYPO3CMS-Guide-ContributionWorkflow/issues/77>`__

Related:

* `Project: Improve readability of TYPO3 documentation <https://github.com/orgs/TYPO3-Documentation/projects/4>`__

* **Problem 1: Too much information on page.** Especially if there are several
  steps to perform and images, notes and hints are on the page, it it difficult
  to see at first glance where one step ends and the next one begins.

   * Solution: Use one of the methods with numbering and background color,
     e.g. `rst-class:: bignums` (see :ref:`h2document:big-nums`)
   * Solution: Use the normal section headers in a consistent way
   * Solution: Do not use too many `.. _tip::` or `.. _hint::`. Use sidebar
     instead. Only use tip / hint etc. on top of page?
   * Solution: Use a box-shadow for images, possibly add transparent border inside image
   * Solution: Do not use huge images in general

* **Problem 2: Images containing text do not stand out enough from plain text**

   * Solution: Always use `box-shadow` for images. Preferably, this should be default in theme
   * Solution: This should be solved in the `theme <https://github.com/TYPO3-Documentation/t3SphinxThemeRtd>`__:
     add additional padding around images, see `issue <https://github.com/TYPO3-Documentation/t3SphinxThemeRtd/issues/104>`__

* **Problem 3: On wide screens, width of area for text is too wide.**
  This makes it hard to read. Example: `A journey through the blog example
  <https://docs.typo3.org/typo3cms/ExtbaseFluidBook/3-BlogExample/1-first-orientation.html>`__

   * Solution: This should be solved in theme, see `existing issue <https://github.com/TYPO3-Documentation/t3SphinxThemeRtd/issues/83>`__


Method: 1-2-3 with big numbers
==============================


first found in form extension docs: https://docs.typo3.org/typo3cms/extensions/form/QuickStart/Index.html

.. rst-class:: bignums-xxl

1. pro

   * good division between parts
   * numbering makes it easier to follow

2. con

   * not in menu, so you can't jump to specific section from menu
   * no named anchor so you can't link directly to section

3. conlusion

   **Good method if there are not too many items (up to 5 is ok).
   It is probably a good idea to use this consistently throughout
   the documentation, e.g. for a Quick start section**

Method: subsections
===================

pro:
----

division between subsection
~~~~~~~~~~~~~~~~~~~~~~~~~~~

subsection title in menu so you can click directly
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


you can link directly to section with named anchors
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

con:
----

* no numbering


Methods: Borders for images
===========================


Adresses problem that it is difficult to distinguish images from text.


For demo with images, also see: https://docs.typo3.org/typo3cms/drafts/github/TYPO3-Documentation/t3SphinxThemeRtdDemoDocs/ImagesAndFigures/Index.html


