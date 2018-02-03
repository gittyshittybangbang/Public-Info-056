
.. include:: ../Includes.txt


==============
TYPO3 Glossary
==============

Overview of basic terms used by TYPO3.

.. _backend:

backend 	
=======

TYPO3 provides a view for editing and administrating the TYPO3 installation. In order to interact with the backend, you need to login as a backend user.

See

* :ref:`Backend and Frontend (Getting started tutorial) <t3start:backend-and-frontend>`
* :ref:`Backend interface (Inside TYPO3) <t3inside:backend-modules-structure>`

.. _backend_module:

Backend module	
==============

In the backend of a TYPO3 installation, the left panel shows a module menu which lists all available backend modules. Backend modules are only available in the backend. 

See

* :ref:`Backend Modules (Inside TYPO3) <t3inside:backend-modules-structure>`

.. _cache:

Cache
=====



.. _ckeditor:

Ckeditor
========



.. _composer:

Composer
========

Composer is not specific to TYPO3.

Composer is a tool for dependency management in PHP. It can be used to setup / manage a TYPO3 installation including the required extensions (and their dependencies). Currently, there is more than one way to setup a TYPO3 installation. It can be done with composer or without. The recommended way is to use composer

See

* `Composer <https://getcomposer.org/>`_
* `How to install TYPO3 using composer (TYPO3 Blog) <https://typo3.com/blog/how-to-install-typo3-using-composer-in-less-than-5-minutes/>`__


.. _core:

Core
====

TYPO3 basic code and functionality. Since (almost) everything is an extension in TYPO3, core functionality is bundled inside the extension „core“.

.. _datahandler:

DataHandler
===========

Formerly known as TCEmain. 

DataHandler provides an API for modifying (creating, modifying, copying, deleting) TYPO3 database records.

See

* :ref:`DataHandler basics (Core API) <t3coreapi:tce-database-basics>`

.. _doctrine_dbal:

Doctrine DBAL
=============

Doctrine is not specific to TYPO3

Doctrine DBAL (database abstraction & access layer) is an abstraction layer for accessing variaous databases. It is used in TYPO3 since TYPO3 8.

See

* :ref:`Database overview (Core API) <t3coreapi:Database_Introduction>`

.. _extbase:

Extbase
=======



.. _extension:

Extension
=========

.. _extension_manager:

Extension Manager
=================

.. _fal:

FAL
===

FAL = File Abstraction Layer (Digitial assets management)

.. _flash_messages:

Flash messages
==============

.. _flexform:

Flexform
========

.. _fluid:

Fluid
=====

.. _frontend:

Frontend
========


.. _formengine:

FormEngine
==========

See

* :ref:`FormEngine (Core API) <t3coreapi:FormEngine-Introduction>`


.. _hook:

Hook
====


.. _install_tool:

Install Tool
============

.. _plugin:

Plugin
======

.. _rte:

RTE
===

.. _scheduler:

Scheduler
=========


.. _signal:

Signal
======

.. _system_log:

System Log
==========

.. _tca:

TCA
===

TCA = Table Configuration Array

.. The following sentence was copied almost verbatim from the tca reference. The rest was added later. See the provided link. Feel free to modify and improve. 

A global array $GLOBALS['TCA']. which extends the definition of database tables beyond what can be done strictly with SQL.

TCA defines / configures properties and relations between database tables and fields. It can be used to
* define which tables / fields are editable in the TYPO3 backend
* configure what is displayed in the backend
* define relations between tables
* configure validators for database fields 

See

* :ref:`Introduction (TCA Reference) <t3tca:introduction>`

.. _tce:

TCE
===

TCE = TYPO3 core engine

The TYPO3 Core Engine handles all data writing to database tables as configured in TCA. 

See

* :ref:`Typo3 Core Engine (Core API) <t3coreapi:tce-introduction>`

.. _tcemain:

TCEmain
=======

Deprecated term, see Datahandler_.




