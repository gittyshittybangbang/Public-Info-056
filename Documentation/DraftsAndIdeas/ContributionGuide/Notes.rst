
.. include:: ../../Includes.txt


==========================
Contribution Guide (Notes)
==========================

Todos
=====

Additional things to add to :ref:`TYPO3 Core Contribution Guide <t3contrib:start>`

If the information already exists somewhere else, link to it and do not duplicate it!



Things to add
-------------

Getting started
~~~~~~~~~~~~~~~

* Add video from Mathias: `How to fix a bug in the core <https://www.youtube.com/watch?v=gN8BVSBlgfU>`__

Bug reporting
~~~~~~~~~~~~~
 
* What to fill out, what to leave blank
   * Do *not* fill out "Assignee" (to be removed shortly for people without permissions, see
* Add formatting information and examples for Redmine
    * how to format links
    * Inline image: example
    * add link: https://www.redmine.org/projects/redmine/wiki/RedmineTextFormattingTextile
* Bug reporting: Hints for how to describe a problem in an understandable way. 
* Add diagram: issue life cycle


Examples:
* Example for bug report with video (animated gif): https://forge.typo3.org/issues/84089

Developing
~~~~~~~~~~


Writing tests
~~~~~~~~~~~~~

* Link to blog articles: https://typo3.com/blog/testing-typo3s-core-part-i-infrastructure

Some information about the testing framework
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Testing
~~~~~~~

Testing for bug reporting, bug handling and testing reviews.

* Hints for testing your stuff

Debugging
~~~~~~~~~

* Add section about debugging, add video from Susi: https://www.youtube.com/watch?v=VtffB0CG1ok&t=13s


Misc
~~~~
 
* Add some handy links to useful views in the section on forger  
* Add section howto startup TYPO3 website (see "needs help")

Appendix
~~~~~~~~

* Add FAQ
* Add a cheat sheet with basic info / commands
* add link to https://typo3.org/community/code-of-conduct/   (or maybe in section on slack?)


Needs help
----------

* Add section howto startup TYPO3 website, also in an easy way for people just testing, not developing. 
   * There is a note on homestead in the gerrit section, check if this is up to date, provide information
   * php -S 127.0.0.1:12345
   * FIRST_INSTALL: https://docs.typo3.org/typo3cms/InstallationGuide/QuickInstall/TheInstallTool/Index.html
* issue life cycle


Structural changes
------------------

* Move "Overview of contribution workflow" to beginning
* Split up "Fixing a bug A-Z" into "Reporting a bug" and "Fixing a bug" 
* move information on slack to a seperate section (e.g. "Getting help"), currently mentioned here
   * https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/latest/singlehtml/#fixing-a-bug-a-z 
   * and here https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/BugfixingAZ/Index.html)
    
Nitpicky minor things
---------------------

* Section ":ref:`Why a pre-commit hook <why-pre-commit-hook>`" : it's not a pre-commit hook, it's a commit-msg hook.

* Change the info to contact the sectteam in :ref:`Topic description <t3contrib:Commit-Message-Format>` to a really prominent warning like:

.. important::
      In case you found a security issues, always get in contact with the `Security Team <https://typo3.org/teams/security/>`__ first! Do not post information about the security leak in a public place. Once you push a patch, it will be publicly viewable on the review server. Do not do this for security-related things.



Open questions
===============

* Is the question of people writing better (reproducable, intelligible and nicely formated) bug reports considered important here? (Maybe ask in channel ...)
  
Drafts
======

Bug reporting
-------------

* Bug reporting: Hints for how to describe a problem in an understandable way. 
    * should "steps to reproduce" be in there?
       * Environment
       * Steps to reproduce
       * Expected result
       * Actual result
       * Screenshot (if it helps to grasp the problem quickly)
    * formatting templates?  https://gist.github.com/carlo/3402842
    * use general common sense, all information not always required

* Example: https://testlio.com/blog/the-ideal-bug-report/
* Example: https://kb.yoast.com/kb/how-to-write-a-good-bug-report/


FAQ
---

moved ... (see index)
