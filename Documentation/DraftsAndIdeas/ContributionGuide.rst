
.. include:: ../Includes.txt


========================
TYPO3 Contribution Guide
========================

Todos
=====

Additional things to add to :ref:`TYPO3 Core Contribution Guide <t3contrib:start>`

* Add video from Mathias: `How to fix a bug in the core <https://www.youtube.com/watch?v=gN8BVSBlgfU>`__
* Add section about debugging, add video from Susi 
* Move "Overview of contribution workflow" to beginning
* Add section "prerequisites" with links to mandatory additional info: core api, coding guidelines
* Add section howto startup TYPO3 website
* Hints for finding place in core for source files to change (see video?)
* Hints for testing your stuff
* Section ":ref:`Why a pre-commit hook <why-pre-commit-hook>`" : it's not a pre-commit hook, it's a commit-msg hook.
* Add a prominent warning / note on the information about [SECURITY] commits to contact the security team first in 
  :ref:`Topic description <t3contrib:Commit-Message-Format>` like: 

.. important::
      In case you found a security issues, always get in contact with the Security Team first! Do not post information about the security leak in a public place (like the TYPO3 source code).

* Add a cheat sheet with basic commands (or put in  "Cheat Sheets" section?)
* Possibly provide a brief overview in the beginning what to read for what purpose:
  * testers only
  * bug reporting
  
Optional
========

* More information for people only testing patches and not developing. There is a note on homestead in the gerrit section, 
  but people not developing probably need more information.
* Add examples for Phpstorm in :ref:`Setting up your IDE for CGL"  

Open questions
===============

* There is no information about bug-reporting. Should this be in this guide, is it handled somewhere else?  
  
  
