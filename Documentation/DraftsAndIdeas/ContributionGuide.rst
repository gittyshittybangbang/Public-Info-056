
.. include:: ../Includes.txt


========================
TYPO3 Contribution Guide
========================

Todos
=====

Additional things to add to :ref:`TYPO3 Core Contribution Guide <t3contrib:start>`

If the information already exists somewhere else, link to it and do not duplicate it!

Things to add
-------------

* Add video from Mathias: `How to fix a bug in the core <https://www.youtube.com/watch?v=gN8BVSBlgfU>`__
* Add section about debugging (link to info and add video from Susi)
* Add links to: core api, coding guidelines
* Add section howto startup TYPO3 website
* Hints for testing your stuff
* More information for people only testing patches and not developing. There is a note on homestead in the gerrit section, 
  but people not developing probably need more information.
* Add hints (only a minor section) with hints for Phpstorm in :ref:`Setting up your IDE for CGL", e.g. "Code:Reformat code"  
* Add a prominent warning / note on the information about [SECURITY] commits to contact the security team first in 
  :ref:`Topic description <t3contrib:Commit-Message-Format>` like: 

.. important::
      In case you found a security issues, always get in contact with the Security Team first! Do not post information about the security leak in a public place (like the TYPO3 source code).

* Add a cheat sheet with basic info / commands (or put in  "Cheat Sheets" section?)
* Add some handy links to useful views in the section on forger  
* Provide a brief overview in the beginning what to read for what purpose:
   * testing
   * bug reporting
   * coding    
* Add formatting information and examples for Redmine in :ref:`<bugfix-index>`
    * how to format links
    * Inline image: example
    * add link: https://www.redmine.org/projects/redmine/wiki/RedmineTextFormattingTextile
* Bug reporting: Hints for how to describe a problem in an understandable way. 
    * should "steps to reproduce" be in there?
    * Example: https://testlio.com/blog/the-ideal-bug-report/
      * Environment
      * Steps to reproduce
      * Expected result
      * Actual result
      * Screenshot (if it helps to grasp the problem quickly)
    * formatting templates?  
* Add a request: after submitting bug reports or patches, monitor your e-mail notifications
   and respond

Structural changes
------------------

* Move "Overview of contribution workflow" to beginning
* Split up "Fixing a bug A-Z" into "Reporting a bug" and "Fixing a bug" 
* Move information on slack to a seperate section (currently mentioned here https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/latest/singlehtml/#fixing-a-bug-a-z and here https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/BugfixingAZ/Index.html)
    * botty : Add a link to botty information: https://wiki.typo3.org/T3Bot  
    * provide very short info on which channel to use for what

Nitpicky minor things
---------------------

* Section ":ref:`Why a pre-commit hook <why-pre-commit-hook>`" : it's not a pre-commit hook, it's a commit-msg hook.




Open questions
===============


  
  
