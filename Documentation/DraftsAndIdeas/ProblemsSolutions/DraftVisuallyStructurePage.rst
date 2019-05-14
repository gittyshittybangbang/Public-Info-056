.. include:: ../Includes.txt

.. _solutions-visually-structure-pages:

===================================================
Solutions for Visually Structuring Things on a Page
===================================================


Related: `Project: Improve readability of TYPO3 documentation <https://github.com/orgs/TYPO3-Documentation/projects/4>`__

* **Problem 1: Not enough visible structure on page.** Especially if there are several
  steps to perform and images, notes and hints are on the page, it it difficult
  to see at first glance where one step ends and the next one begins.

  More than one of the following solutions could be applied:

   * Solution 1: Use one of the methods with numbering and background color,
     e.g. :ref:`visually-structure-example-bignums` (see :ref:`h2document:big-nums`)
   * Solution 2: Use the normal section headers in a consistent way, e.g. ref:`visually-structure-example-sections`
   * Solution 3: Do not use too many `.. _tip::` or `.. _hint::`.
   * Solution 4: Use a box-shadow for images, possibly add margin around image
   * Solution 5: Do not use huge images in general

* **Problem 2: Images containing text do not stand out enough from plain text**

   * Solution 1: Always use `box-shadow` for images.
   * Solution 2: Better to solve this in the `theme <https://github.com/TYPO3-Documentation/t3SphinxThemeRtd>`__:
     always add drop-shadow and add additional padding around images,
     see `issue <https://github.com/TYPO3-Documentation/t3SphinxThemeRtd/issues/104>`__

* **Problem 3: On wide screens, width of area for text is too wide.**
  This makes it hard to read. Example: `A journey through the blog example
  <https://docs.typo3.org/typo3cms/ExtbaseFluidBook/3-BlogExample/1-first-orientation.html>`__

   * Solution 1: This should be solved in theme, see `existing issue <https://github.com/TYPO3-Documentation/t3SphinxThemeRtd/issues/83>`__


