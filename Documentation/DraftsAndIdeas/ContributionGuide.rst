
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
   * testing
   * bug reporting
   * coding    
* Add some handy links to useful views in the section on forger  
* Possibly add more information on the section :ref:`<redmine-index>`
   * Status: 
      * who sets to Accepted (core team?)
      * I guess, the rest is obvious
 * Possibly split up "Fixing a bug A-Z" into "Reporting a bug" and "Fixing a bug" 
 * Add formatting information and examples for Redmine in :ref:`<bugfix-index>`
    * how to format links
 * Hints for how to describe a problem in an understandable way. 
    * should "steps to reproduce" be in there?
    * Example: https://testlio.com/blog/the-ideal-bug-report/
      * Environment
      * Steps to reproduce
      * Expected result
      * Actual result
      * Possibly screenshot (if it helps to grasp the problem quickly)
 * Personally, I would add another request: after submitting bug reports or patches, monitor your e-mail notifications
   and respond quickly. 
  
  
Optional
========

* More information for people only testing patches and not developing. There is a note on homestead in the gerrit section, 
  but people not developing probably need more information.
* Add examples for Phpstorm in :ref:`Setting up your IDE for CGL"  

Open questions
===============


  
  
