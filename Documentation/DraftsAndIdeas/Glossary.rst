
.. include:: ../Includes.txt

.. Suggestions:
   1. Keep text here short and link to relevant sections in manual.
   
.. Todo
   1. Check: When we talk about TYPO3 core, do we mean the entire TYPO3
   source or just the "core" sysext in the source?

=====================
DRAFT: TYPO3 Glossary
=====================

Overview of basic terms, acronyms and hashtags used throughout the TYPO3 documentation
and TYPO3 community.

.. hint::

   This is a first draft. The idea is: When people are new to TYPO3, 
   they might get confused by the terminology. This should serve as
   a handy reference. The explanations should be kept short and link 
   to the places in the documentation where the respective concept 
   is explained in more detail.
  

   
.. _backend:

Backend 	
=======

TYPO3 provides a view for editing and administrating the TYPO3 
installation. In order to interact with the backend, you need to 
login as a backend user.

See

* :ref:`Backend and Frontend <t3start:backend-and-frontend>` 
  (Getting started tutorial)
* :ref:`Backend interface <t3inside:backend-modules-structure>` 
  (Inside TYPO3)

.. _backend_module:

(Backend) module	
================

In the backend of a TYPO3 installation, the left panel shows a 
module menu which lists all available (backend) modules. Backend 
modules are only available in the backend. 

Backend modules are provided by :ref:`extensions`, as are
:ref:`Plugin` (displayed in the Frontend).

See

* :ref:`Backend Modules <t3inside:backend-modules-structure>` 
  (Inside TYPO3)
* :ref:`Extension Architecture <t3coreapi:extension-architecture-introduction>` 
  (Core API)

.. _cache:

Cache
=====

TYPO3 optimizes performance by using a sophisticated caching system. This is highly configurable, e.g. the page cache can be stored in the Database or for example in Redis. 

See

* :ref:`Caching Framework <t3coreapi:caching>`
* `Stackoverflow: What are the different kind of caches? <https://stackoverflow.com/questions/27320922/typo3-what-are-the-different-kind-of-caches>`__


.. _ckeditor:

CKEditor
========

`CKEditor <https://en.wikipedia.org/wiki/CKEditor>`__ itself is not specific to TYPO3, the extension rte_ckeditor is. 

CKEditor is a Rich Text Editor (:ref:`RTE <t3coreapi:rte>`) that can be used to edit fields in TYPO3 using Wysiwyg elements like lists, bold text etc. The corresponding extension (rte_ckeditor) is included in the core but it must be activated.  

Ckeditor is configured with Yaml files.

See

* TYPO3 Worx: `The new CKeditor in TYPO3 : A configuration tutorial <https://typo3worx.eu/2017/02/configure-ckeditor-in-typo3/>`__


.. _composer:

Composer
========

Composer is not specific to TYPO3.


Composer is a tool for dependency management in PHP. It can be used
to setup / manage a TYPO3 installation including the required 
extensions (and their dependencies). Currently, there is more than 
one way to setup a TYPO3 installation. It can be done with composer 
or without. The new (and recommended) way is to use composer

See

* `Composer <https://getcomposer.org/>`_
* `How to install TYPO3 using composer 
  <https://typo3.com/blog/how-to-install-typo3-using-composer-in-less-than-5-minutes/>`__ 
  

.. _content-element:

Content element
===============

.. see StackOverflow: https://stackoverflow.com/questions/42644930/typo3-difference-between-plugin-and-custom-content-element


.. _core:

Core
====

.. attention:: 
   Fixme: Check this!

TYPO3 Core can mean one of two things:

#. The entire TYPO3 CMS 

   #. Entire TYPO3 CMS codebase (source code )
   #. TYPO3 core functionality (meaning the functionality, that the TYPO3 CMS supplies)

#. ext:core Since (almost) everything is an
  extension in TYPO3, core functionality is bundled inside the extension 
  "core".

   #. TYPO3 basic code provided by ext:core. 
   #. TYPO3 basic functionality provided by ext:core. 



Most of the time "TYPO3 core" refers to the first and second definition, as in TYPO3 core development. 

.. _css_styled_content:

css_styled_content
==================

Outdated, see :ref:`fluid_styled_content`.

.. _datahandler:

DataHandler
===========

Formerly known as TCEmain. 

DataHandler provides an API for modifying (creating, modifying, copying, 
deleting) TYPO3 database records.

See

* :ref:`DataHandler basics (Core API) <t3coreapi:tce-database-basics>`

.. _doctrine_dbal:

Doctrine DBAL
=============

Doctrine is not specific to TYPO3.

Doctrine DBAL (database abstraction & access layer) is an abstraction layer 
for accessing various databases. It is used in TYPO3 since TYPO3 8.

See

* :ref:`Database overview (Core API) <t3coreapi:Database_Introduction>`

.. _Extbase:

Extbase
=======

.. The following sentence was copied verbatim from the manual. See the provided link. Feel free to modify and improve. 

Extbase is a framework for TYPO3 extension development. It is included inside the TYPO3 source code.

See

* :ref:`Introduction (TYPO3 Extbase guide) <t3extguide:start>`


.. _extension_builder:

Extension Builder
=================

Extension_builder is an additional extension that is not included with the TYPO3 CMS. It can be used to design extensions and automatically generates code. It includes a database modeler.

See

* `extension_builder <https://docs.typo3.org/typo3cms/extensions/extension_builder/>`__



.. _extensions:

Extensions
==========

Extensions are software components for TYPO3. An extension must 
adhere to some standards in order to be detected and loaded by TYPO3. 

* Extensions may be installed via the :ref:`extension_manager` or via 
  :ref:`composer`.  It is recommended to use the composer method.
* The TYPO3 source code itself consists mostly of extensions.
* The Extension Architecture of TYPO3 makes TYPO3 very extendable and flexible. 
* A large number of Extensions provided by 3rdparties are available 
  via the TYPO3 Extension Repository (:ref:`ter`) or `Packagist
  <https://packagist.org/packages/typo3/>`__ (if you use composer). 
* Extensions are typically developed using the :ref:`extbase` Framework
  and / or the :ref:`fluid` templating engine, but it is possible to
  develop extensions without using Extbase or Fluid. 

See

* :ref:`Extension Architecture 
  <t3coreapi:extension-architecture-introduction>` 
  (Core API)
* `TYPO3 Extension Repository 
  <https://extensions.typo3.org/>`__ 
  (TER)

.. _extension_manager:

Extension Manager
=================

The Extension Manager is accessible in the :ref:`backend` of a TYPO3
Installation. It can be used to configure Extensions, execute update 
scripts of Extensions, import, install, uninstall, update and remove 
Extensions.

If :ref:`composer` is used to setup a TYPO3 installation, all installation 
/ deinstallation of Extensions is done via composer. In this case, it 
is not possible to do this with the Extension Manager.

See

* :ref:`Extension Manager <t3start:extension-manager>` (Getting Started)
* :ref:`Extension Manager <t3coreapi:extension-manager>` (Core API)


.. _fal:

FAL
===

FAL = File Abstraction Layer 

Abstraction Layer in the TYPO3 core for handling files. 

See

* :ref:`FAL Introduction <t3coreapi:fal_introduction>` (Core API)
* :ref:`Using FAL <t3coreapi:using-fal>` (Core API)


.. _flash_messages:

Flash messages
==============

.. _flexform:

Flexform
========

.. This is a first draft for a text. I didn't really find a place in the documentation where flexforms are explained. 

Flexforms are used to configure plugins. A configuration schema is defined in XML. It can contain text fields, lists and other elements. This defines how a plugin is configured in the TYPO3 backend. The configuration is stored into a single field pi_flexform inside the tt_content table. 

.. attention::
   Fixme: add link


.. _Fluid:

Fluid
=====

Fluid is a templating engine used by TYPO3. 

See

* :ref:`Fluid <t3extguide:start>` (Extbase / Fluid guide)

.. attention::
   Fixme: I did not find a really good introductory text for fluid
   in the docs. Maybe add another link later or update the docs?


.. _fluid_styled_content:

fluid_styled_content
====================


.. _form-framework:

Form
====

aka Form Framework, aka EXT:form

.. todo: clarify : 
.. - formengine
.. _ formhandler
.. _ form
.. - form framework (see #cig-formframework on slack)


.. question: is EXT:form = form framework?



.. _formengine:

FormEngine
==========

FormEngine aka TCEforms

.. attention::
   Find a good introductory text for FormEngine. The Core API docs
   do a good job of explaining how FormEngine, TSFE and DataHandler
   play together, but what exactly is the responsibility of 
   FormEngine is a little fuzzy. This here is a very, very first draft.
   
FormEngine is part of the TYPO3 core. It renders forms in the :ref:`backend`
for editing records. It can be used to edit for example the page title in 
the table pages. The result is then stored in the database. :ref:`tca` is 
used to configure how the various fields can be edited. 

See

* :ref:`FormEngine <t3coreapi:FormEngine-Introduction>` (Core API)





.. _frontend:

Frontend
========



.. _hook:

Hook
====


.. _install_tool:

Install Tool
============

.. _irre:

IRRE
====



.. _mount_point:

Mount Point
===========


.. _page_overlay:


Page Overlay
============



.. _plugins:

Plugins
=======

See

* * :ref:`Extension Architecture <t3coreapi:extension-architecture-introduction>` (Core API)


.. _rte:

RTE
===

.. _scheduler:

Scheduler
=========

The ' TYPO3 scheduler <https://docs.typo3.org/typo3cms/extensions/scheduler/Index.html>' __ 
is an extension inside the core which can be used to automatically and periodically 
start processes inside the TYPO3 context. Extensions can provide :ref:`command controllers <t3extbasebook:extbase_command_controller_about>`
that may be executed via the scheduler. 

.. _signal:

Signal
======



Slot
====


.. _system_log:

System Log
==========

sys_log

.. _t3dd:

t3dd
====

TYPO3 developer days (Event) 

.. _t3uxw:

T3uxw
=====

TYPO3 User Experience Week (Event)


.. _tca:

TCA
===

:ref:`TCA <t3tca:introduction>`  = Table Configuration Array

.. The following sentence was copied almost verbatim from the tca reference. 
.. The rest was added later. See the provided link. Feel free to modify and improve. 

A global array :php:`$GLOBALS['TCA']` which extends the definition of 
database tables beyond what can be done strictly with SQL.


TCA defines / configures properties and relations between database 
tables and fields. It can be used to:

* define which tables / fields are editable in the TYPO3 backend
* configure what is displayed in the backend
* define relations between tables
* configure validators for database fields 



.. _tce:

TCE
===

TCE = TYPO3 core engine

The TYPO3 Core Engine handles all data writing to database tables 
as configured in TCA. 

See

* :ref:`TYPO3 Core Engine <t3coreapi:tce-introduction>` (Core API)

.. _tcemain:

TCEmain
=======

Deprecated term, see :ref:`datahandler`.

.. _tceform:

TCEFORM
=======


.. _template:

Template
========

In the context of TYPO3, template can mean any of these things:

* A :ref:`typoscript` template, which is a set of TypoScript configuration connected 
  to a specific page (and it's subpages)
* A :ref:`fluid` template file defining how a plugin / content element / page is to be 
  rendered
* (not TYPO3 specific) The general process of using a template as a general blueprint for the site layout. The 
  template contains static parts and dynamic parts that will be filled differently for each page


.. _ter:

TER
===

`TYPO3 Extension Repository <https://extensions.typo3.org/>`__

Extensions that are supplied by 3rdparties and that are not shipped with TYPO3 are hosted in the TER. The TER web interface supplies information about each extension (e.g. Link to the documentation, TYPO3 version support).

The TER used to be the central repository for Extensions. Nowaday, it is recommended 
to use :ref:`composer` and the extensions are downloaded from resources like packagist. 

.. _tsconfig:

TSConfig
========

TSconfig can be page TSconfig (specific to a page and it's subpages) 
or user TSconfig (specific to a Backend user or Backend group). 

It is used to configure the TYPO3 backend. 

.. tsfe:

TSFE
====

.. attention::
   I did not find any place in the docs where TSFE is explained ... This text was written from scratch. 

TSFE = TypoScript Frontend

$GLOBALS['TSFE'] is the instantiation of the class TypoScriptFrontendController. It contains information for the currently rendered page in the frontend, e.g. the current language or pid.  

.. attention::
   Fixme: Find better place to link to.

See

* `FormEngine introduction <https://docs.typo3.org/typo3cms/CoreApiReference/ApiOverview/FormEngine/Introduction/Index.html?highlight=typoscriptfrontendcontroller>`__ (Core API)



.. _typo3:


TYPO3
=====

The word TYPO3 has several meanings:

* The word "TYPO3" is a trademark owned by the TYPO3 Association, see `Trademark Usage Policy <https://typo3.org/about/the-trademarks/>`__
* TYPO3 is often used to refer to TYPO3 CMS, though TYPO3 CMS would be the correct term.
* TYPO3 is often used in combination with anything concerning TYPO3 including but not limited to the TYPO3 community and the TYPO3 products.
* The name TYPO3 has the following history: `About the name <https://typo3.org/about/the-brand/about-the-name/>`__


.. _typo3_association:

TYPO3 Association
=================

.. Text taken verbatim from ttps://typo3.org/association/

The `TYPO3 Association <https://typo3.org/association/>`__ is a not-for-profit organisation and was founded in 2004 to provide funds for long-term development goals.


.. _typo3_cms:

TYPO3 CMS
=========

The TYPO3 `Content Management System <https://en.wikipedia.org/wiki/Content_management_system>`__.

.. _typo3_gmbh:

TYPO3 GmbH
===========


.. _typoscript:

TypoScript
==========

"TypoScript is a syntax for defining information in a hierarchical structure using simple ASCII text content." (:ref:`What is TypoScript <t3coreapi:typoscript-syntax-what-is-typoscript>` TypoScript is converted into a PHP array. 

It can be used for configuration and for defining the rendering in the frontend. Some parts of what was previously handled by TypoScript is now being taken over by :ref:`fluid_styled_content` and :ref:`fluid` templates. 

Just a few examples of what can be done with TypoScript:

* language configuration
* define how menus are rendered in the site layout
* configure extensions


.. _user_int:

USER / USER_INT
===============


(Fluid) ViewHelper
==================
