.. include:: ../../Includes.txt

.. _decisions:

=========================
Decisions, Best Practices
=========================

.. important::

   The information on this page is in no way official. It reflects my opinions.
   Note that I am not an experienced documentation writer. I have read some
   resources, but most of what I came up here is based on looking at TYPO3
   documentation, thinking about what works for me and comparing it to other
   documentation.

For the TYPO3 documentation, a large amount of documentation already exists. 

I think, basic structure and best practices should be defined and a common
goal developed. This can
be an abstract vision which must then be put into practice by defining "best
practices" and "how to do things".


Documentation Manifesto
=======================

Inspired by "Zen of Python" and "Agile Manifesto", this is what I have come up
with so far.



* **Publish when ready** - no to unfinished documentation
* **Quality over quantity** - if you cannot maintain it, take it down
* **Respect your reader** - yes, the documentation is for the reader
* **Respect your contributor** - give him clear instructions, respect his time,
  value her work
* **Test it** - and collect feedback
* **Think about new people too** - not just the experienced TYPO3 users
* **New replaces old** -  Every time you add something new - take down or merge something old!
* **Actions speak louder than words** - If you find documentation important for
  TYPO3, then do something about improving it! Or at least point out the problems!


Main Goal
=========

Make it easier to learn to use, develop for, integrate with, administrate, edit for TYPO3.


Open Questions and Answers
==========================

When finding best practices, these are some of the questions that should be
answered and decided on. Some of these already exist as issues in GitHub.

You can also see my answers and solutions for these open questions,
but currently they only reflect my opinion and are in no way official.

General
-------

Publish Early or Publish When Ready?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question:
   Should we publish early or publish only when "ready"?
   Publish means the texts are available on docs.typo3.org
   and crawlable by search engines. "When ready" means the
   documentation is at least in most parts correct and
   up-to-date (meaning it has been fully reviewed before a new
   branch is published).

My answer:
   I think we should publish only when ready, meaning all
   documentation is up-to-date and correct (a few minor
   errors may still exist, of course). But should not publish
   a new branch that has not been touched for years.

Is this realistic?
    Currently, not. There are not enough people
    to do this, as there are not enough people working on the
    documentation in general. But I think, this should be the goal.
    The damage of people finding incorrect, not up-to-date documentation
    with "to be written" and spelling mistakes cannot be undone
    easily. If they have the impression that the documentation is
    not good, not correct, this will last and they may even turn
    away from TYPO3 because of it (we have heard of accounts of
    this happening).

Implementation
    We have a /typo3cms/draft url on which we can render that
    is not crawled by search enginges. Draft pages should
    additionally contain a message at the top of the page.



“Book” Structure or “One Online Page Structure”
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question:
   Guides, Tutorials etc. are often structured into several
   pages and chapters. You usually have to read entire book.
   Documentation projects of other open source projects
   often have all relevant information
   on one page to solve a single task. Which method should we
   prefer in the future?

My Answer:
   I think people read online material differently. They often google
   for one thing. They want to solve one task. In general, I think the
   information we supply, is too long. And it is not structured in a
   way you can jump right in on any page. I would prefer the "one online
   page structure" within a guide, for example a guide contains a list
   of mini howtos, every howto on one page. The manual :ref:`h2document:start`
   and :ref:`t3contrib:start` already follow this approach. But a good
   part of the information can probably still be drastically reduced and
   shortened.

Example:
   * symfony: Review patch / issues: https://symfony.com/doc/current/contributing/community/reviews.html


Create Documentation Bottom-Up or Top-Down
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question:
   Should we create documentation bottom-up: create individual manuals,
   keep adding more chapters, pages. Or should we create it top-down:
   look at the big picture, decide on information architecture **first**.

Answer:
   We already have a lot of information. So it's not a question where to
   start. But, before we proceed, we should decide about the structure.
   And to do that, we should get feedback from the community and look at
   other documentation projects.


"We Have x" Approach Versus a "I Want to Do x" Approach
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question:
   "We have x" approach describes what TYPO3 has. It is written from the
   perspective of TYPO3. For example describing an API or describing the
   backend in "Getting Started Tutorial". "I want to do x" looks from the
   perspective of the user. He or she wants to solve a task. And fast. This would
   best be served by a mini one-page Howto Guides (e.g. ideally one page
   per task, as already described above).

My Answer:
   I think it often depends on the material. If you have an API, you rather
   show what you have ("we have x") approach. But then you also need examples
   of how to do things. I think, in general, "TYPO3 Explained" follows the
   "we have x" approach. Even if some chapters are explained well and some
   chapters can be used to solve a task, the general structure is so, that
   you are lost, unless you already know at least the basics of how to do
   things. "TYPO3 Explained" jumps right into the specifics of one small
   detail. What is missing, is the part that walks you through the beginning.
   Example: I want to create a content object. Where do I start? I want to
   learn how to configure TYPO3 as an integrator. Where do I start?

The question is which approach to use where? And what does the reader need?
The documentation is not primarily for showcasing how great TYPO3 is. It
should be for helping people to use it.


Long Background Story or Short Info for How to Get Things Done?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question:
   Should we go into the history at all if not necessary? Should we explain
   how it works?

My Answer:
   I am very much in favor of understanding how things work. I am not a fan
   of just supplying snippets you can simply copy-paste. **But** I think the
   information should be structured in a way, you can easily find the step-by
   step information. You should not have to always plow through the entire
   history of how things developed *first*. It's good to have it, but make
   it easy for the reader. Providing a quick start is often a good idea,
   see `ext:form <https://docs.typo3.org/typo3cms/extensions/form/QuickStart/Index.html>`__
   Some of the chapters in the Extbase / Fluid book and even in TYPO3 Explained
   are just way to long. And a quick start or quick reference is missing.


What Should Be Documented on docs.typo3.org and What Elsewhere?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question:
   Some documentation is in books, videos and blogs. What should be documented
   on docs.typo3.org, what in blogs and what in books?

My Answer:
   This is not an easy question. And of course we can't really tell people what
   to blog about or what to write books about. But one thing I noticed is, it is
   not that documentation does not get written. People write **a lot**: on blogs,
   in books, on StackOverflow, on Slack. *If* a lot of the time people put in
   writing on StackOverflow, in blogs on Slack would be put into the documentation,
   we would not have such a problem on docs.typo3.org. So this is not an answer,
   this is another question. Why do people document things on blogs and not on
   docs.typo3.org? Why do they write great answers on StackOverflow, but rarely
   make the changes on docs.typo3.org? Why is the quality of the blogs and of
   StackOverflow often much higher than on docs.typo3.org?

   Let's ask these questions and be honest about it.

   We could draw the conclusion, ok, not everything must be documented on docs.typo3.org,
   it's ok to have the blogs. But they cannot be maintained by the community.
   Beginners don't know where to read. They do not know what to trust. Where to
   start. They often come to docs.typo3.org when they begin. So, no, **the current
   situation is not good.**


Documentation in Extra GitHub Repoitories or in Core?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question:
   Should documentation be kept extra or in TYPO3 core code repository?
   We currently have both: changelog + sysext doc in core, everything
   else separate (see :ref:`h2document:overview-of-types`.
   Currently, even the system extensions do not do it
   consistently, e.g. ext:form and ext:rte_ckeditor in core, ext:seo in
   "TYPO3 Explained".

My Answer:
   There are a number of arguments for keeping documentation in the code
   repo, see for example https://hackernoon.com/write-good-documentation-6caffb9082b4
   one possibility: put tsref, TCA ref, TSconfig ref and TYPO3 Explained in core.
   Would be easier if TYPO3 core uses GitHub as well.

Related:
   * `Issue: Maintain documentation in core? <https://github.com/TYPO3-Documentation/T3DocTeam/issues/72>`__

One-File Approach or Multi-File Approach With Little Content on one Page?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Question:
   It was customary to have an Index.rst for each subchapter and then a toctree
   with various other pages. Some of these pages contain little content.
   The trend already seems to be to put more on one page (see "TYPO3 Explained")

Answer:
   I would avoid having pages with very little content and no context. But,
   putting a lot on one page can make it more overwhelming. So one must
   be careful to structure it well with chapters or even :ref:`h2document:big-nums`.
   In any case, having to page back and forth on pages with 2 sentences is annoying.

Specific Questions
------------------

How Do we Deal With Changelog:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question:
   For features, Changelog is often main source of documentation. This causes
   fragmentation, meaning the documentation is missing in main manual, or it
   just contains a stub and then points to Changelog. How do we deal with this?
   Proceed as before, or change something?

Answer:
   Not decided on this yet. Also see already existing issue:

Related:
   * `Issue: Question: How to deal with Changelog becoming main documentation for some new features?
     <https://github.com/TYPO3-Documentation/TYPO3CMS-Reference-CoreApi/issues/418>`__

What Is Scope of TYPO3 Book?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question:
  What is scope of TYPO3 book and how does it relate to docs.typo3.org?

My answer:
  From what I understand it, the book is in addition to docs.typo3.org. It should
  cover the basics. But I am not sure, if you were to map out a learning path,
  what would you tell people to read? We usually send them to the :ref:`t3start:start`
  first. But, then what?
  My answer would be: We cannot think about the scope of the TYPO3 book unless
  we also think about the scope on docs.typo3.org as a whole and about learning
  paths for integrators, developers, editors and system administrators.

What Is Future of Extbase / Fluid Book?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question:
   These are actually several questions: Should Fluid be separated? Must we document
   Fluid basics at all, as it is already documented on typo3fluid on GitHub?
   What is scope of (to be released) edition 3 of Fluid / Extbase book by
   Michael Schams? Do we need another online book?

My Answer:
   I would try to deduplicate as much as possible. As soon as book comes out,
   if it covers the material well and there is considerable overlap, I would
   at least think about taking down Extbase / Fluid book and replacing it
   with only what is missing, e.g. a set of mini howtos or a reference.

   The same goes for information on `typo3fluid on GitHub
   <https://github.com/TYPO3/Fluid/blob/master/README.md>`__


Contribution
------------

Do We Keep Telling People That Writing Documentation Is Easy?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question:
   Do we want to keep telling people documenting is easy and everyone can do it?
   Or do we want to sell it as a task that requires a number of skills, requires
   some learning but can be very rewarding in the end?

My Answer:
   Short answer: no!

   Long answer: Selling something as easy does not necessarily motivate developers. In fact,
   the "easy" approach devalues it: Everyone can do it, so it's for people who
   are not skilled enough for other things (???). I'm not saying this, but that
   may be the implicit message.

   Additionally, the "easy" approach frustrates people because telling someone
   somethings is easy that is not and where they may struggle makes them feel stupid.
   Put some more glamour into documenting: It's not easy, it requires skills.

   But, do give people resources, documentation, examples, templates to make it
   easier to write good documentation!






