.. include:: ../../Includes.txt

.. important::
This chapter was written from scratch. Please review carefully.

current status: Very rough draft. Still needs more work!

====================================
Draft: Setting up and using Phpstorm
====================================

General Setup
=============

* Settings: Languages & Frameworks: PHP
   * PHP Language Level
   * CLI

Coding Guidelines
-----------------

* PSR-2
* use Code: Reformat Code (if necessary)

Link to coding guidelines

Recommended Plugins
====================

* DynamicReturnTypePlugin
* Php Inspections (EA Extended)
* TYPO3 CMS Plugin ?
* TYPO3 XLIFF Utility ?
* TypoScript Plugin ?

Writing Tests
=============

* Settings: Languages & Frameworks: PHP: Test Frameworks (or "PHPUnit")
   * Use composer autoloader
   * Path to script: vendor/autoload.php
   * Test runner: Defaut configuration file: vendor/typo3/testing-framework/Resources/Core/Build/UnitTests.xml
   * Test Runner: Default bootstrap file: vendor/typo3/testing-framework/Resource/Core/Build/UnitTestsBootstrap.php


See:

* https://wiki.typo3.org/Development/PHPStorm_Settings