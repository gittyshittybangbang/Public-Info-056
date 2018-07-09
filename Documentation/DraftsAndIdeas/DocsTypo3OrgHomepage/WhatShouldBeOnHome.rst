.. include:: ../../Includes.txt
.. highlight:: rst

.. _references:

=========================================
Concept: What should be on the Homepages?
=========================================

Common best practices
=====================

* A lot more on the start page, you don't have to click in any submenu, you can
  access the most basic stuff from one page
* A "Getting Started" section
* A section "Architecure Concepts" (not in start manual, somewhere else, e.g. Core API)

  * see `Angular: Architecture overview <https://angular.io/guide/architecture>`__

* A section "Developer Documentation"

  * see `Drupal:Developer documentation <https://www.drupal.org/docs/develop>`__


Possible Structure: Concept 1
=============================

* **Getting started:** one page with information (and links) for

  * link to Getting started Tutorial
  * Setting up TYPO3 (link to Installation & Upgrade Guide)
  * some more links and information for getting started

* **Editor** documentation: all links on one page

  * Getting started tutorial
  * Tutorial for editors
  * `Security Guide: Link to section for editors <https://docs.typo3.org/typo3cms/SecurityGuide/GuidelinesEditors/Index.html>`__

* **Integrator** documentation: all links on one page!

  * TypoScript reference
  * TSconfig reference
  * rte_ckeditor Docs
  * `Security Guide: Link to section for integrators: <https://docs.typo3.org/typo3cms/SecurityGuide/GuidelinesIntegrators/Index.html>`__

* **Developer** documentation: all links on one page!

  * Tutorials and Guides for Developers
  * References for Developers (contains all references currently in references section)
  * Cheat Sheets
  * Snippets

* **SysAd** documentation: info for hosting / system administration

  * currently does not exists, create a guide?
  * could contain updated stuff from the wiki

    * performance optimization
    * tuning MySQL server
    * setting up a caching proxy with Varnish
    * setting up a load balancing system
    * Caching with the caching framework, e.g. Redis, ...
    * Troubleshooting
    * Configuring Webserver, e.g. Apache, Nginx ...

* **Documentation** documentation
* **Translation** documentation
* **Extensions:** System extensions and search box for TER extensions on one page
* **How to get help** (link to https://typo3.org/help)
* **How to contribute** (link to contribution guide)
* **How to use the TYPO3 documentation**

  * Information about the general structure
  * Information about version selector
  * Information about how to use search
  * Information about how to give feedback (link to feedback section)

* **Feedback** : where to give feedback on the docs


What is omitted / moved:

* All cheat sheets are developer sheet cheats, so the list is moved to
  Developer section
* Snippets are moved to Developer section
* References is moved to Developer section, some references will also
  be listed in integrator section


Possible Structure: Concept 1 - pros and cons
=============================================

to be clarified
===============

* should there be a general getting started section or a getting started
  section in each area for editors, integrators etc.?

pro
===

* specific sections for developers, integrators etc. they find everything in one place

con
===

* some docs are not specific to dev / integrators / editors, etc. what to do here?
  Possible solution could be to link directly to the respective section for editors,
  etc.
  Currently this is:

  * Frontend Localization Guide: most of it relevant for integrators, some for editors
  * Security guide: has specific section for editors, integrators etc.
  * Tell me something about X


How do other documentation projects do it
==========================================

What do other docs have on their docs start page?

Symfony
--------

What is worthy of imitation?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* a lot more on one page, you don't have to click in any submenu, you can
  access everything from one page

General observations
~~~~~~~~~~~~~~~~~~~~


Content structure
~~~~~~~~~~~~~~~~~

Links on docs start page (we're not listing everything here):

* What is Symfony?
* Getting started + Subchapters
* New features
* Announcements
* Guides and Tutorials
* Training
* Certification
* Best practices
* Contribution
* PDF Download

https://symfony.com/doc/current/index.html



Laravel
-------


What is worthy of imitation?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* section "Architecture Concepts"
* section "Getting started"


General observations
~~~~~~~~~~~~~~~~~~~~

* documenation is structured by reading level (e.g. basics, digging deeper etc.)

Content structure
~~~~~~~~~~~~~~~~~

Links on docs start page (we're not listing everything here):

* Getting started
* Architecture Concepts
* The Basics
*


https://laravel.com/docs/5.6


Wordpress
---------

What is worthy of imitation?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* has a small table of contents on the start page (of a specific guide in this example,
  see `Plugin API <https://codex.wordpress.org/Plugin_API>`__
  Advantages:

  * You don't have an entire Sitemap on one page like we often do, which is overwhelming
    because it contains far too much information.
  * you don't waste space with only a few sentences on one page, as we often do


Drupal
------

What is worthy of imitation?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Section `"Developer documentation" <https://www.drupal.org/docs/develop>`__
* Section `"Troubleshooting <https://www.drupal.org/troubleshooting>`__
* On the `Code Snippets <https://www.drupal.org/documentation/customization/snippets>`__
  pages, at least some of them are categorized, e.g. PHP snippets, SQL snippets

Not good
--------

* Seperate "Developer documenation" and "Developer Guides"


Angular
-------

What is worthy of imitation?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* `Architecture overview <https://angular.io/guide/architecture>`__ walks you through the
  basic concepts