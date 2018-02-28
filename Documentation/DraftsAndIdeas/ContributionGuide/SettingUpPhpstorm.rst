.. include:: ../../Includes.txt


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


Recommended Plugins
====================

* DynamicReturnTypePlugin
* Php Inspections (EA Extended)

Writing Tests
=============

* Settings: Languages & Frameworks: PHP: Test Frameworks (or "PHPUnit")
   * Use composer autoloader
   * Path to script: vendor/autoload.php
   * Test runner: Defaut configuration file: vendor/typo3/testing-framework/Resources/Core/Build/UnitTests.xml
   * Test Runner: Default bootstrap file: vendor/typo3/testing-framework/Resource/Core/Build/UnitTestsBootstrap.php
