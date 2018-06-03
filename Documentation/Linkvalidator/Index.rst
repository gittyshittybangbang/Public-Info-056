.. With the following include we import some definition. We do this in each and every file.
   so we can change the definition at a single place. Use the relative path to the Includes.txt file,
   which may look as well like ../../../Includes.txt for a deeply nested source file.

.. include:: ../Includes.txt


.. Usually we define 'php' as default highlight language in Includes.txt.
   With the following 'highlight' directive we switch to reStructuredText as default highlight language.

.. highlight:: rst


.. The following, first section (= headline) is the 'Document Title'.


=============
Linkvalidator
=============

What does it do?
================

* Provides Backend module for checking for broken links, displaying a list of broken links and fixing links
* Provides Scheduler task for checking links
* Configuration via TSconfig: `Configuration docs <https://docs.typo3.org/typo3cms/extensions/linkvalidator/Configuration/Index.html>`__ `Default TSconfig <https://github.com/TYPO3/TYPO3.CMS/blob/master/typo3/sysext/linkvalidator/Configuration/TsConfig/Page/pagetsconfig.tsconfig>`__
* Several link types are supported (Page links, external links, ...), provides **hooks** for adding other linktypes

Basic information and links
===========================

* Core extension: typo3/sysext/linkvalidator
* `Official Linkvalidator documentation <https://docs.typo3.org/typo3cms/extensions/linkvalidator/Index.html>`__
* Slack channel `#linkvalidator-rewrite <https://typo3.slack.com/messages/CAEND116H>`__
* TYPO3 forge isue: `Epic #85006 <https://forge.typo3.org/issues/85006>`__
* WIP github `linkvalidator branch basic-rewrite-sybille <https://github.com/wmdbMattes/linkvalidator/tree/basic-rewrite-sybille>`__

Current status
==============

* some bugs and patches pending
* Usability for editors should be improved

Current plan
============

* Fix bugs for TYPO3 v9 + TYPO3 v8
* Add Tests
* Rewrite with Fluid (reuse current functionality) for TYPO3 9 only
* 
