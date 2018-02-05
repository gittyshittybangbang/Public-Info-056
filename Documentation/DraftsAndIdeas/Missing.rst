
.. include:: ../Includes.txt

============================
Things missing in TYPO3 docs
============================


This is an unordered, unprioritized list of things missing from the documentation,
things that are difficult to understand, ambigous or possibly not made clear enough. 

Of course, this is very opiniated. Understanding basic concepts always depends on 
experience, background and a number of other things.

We are basing this on the basic assumption that TYPO3 should not be extremely hard
to learn if you already have some technical background in progamming and it should
be possible to get a good understanding of the basic architecture by reading the 
material on docs.typo3.org (mostly Core API) and possibly a book about extension 
programming.

You can setup and use TYPO3, you can even program extensions without really 
understanding how it works, but in my experience, without a good understanding how
something works under the hood, you eventually run into a brick wall when trying to
do things, that go beyond basic recipes. That goes for TYPO3, that goes for git and
probably just about anything else.

The focus here is on general concepts, not on details. 
 
 
 
 TCE
 ===
 
 "The TYPO3 Core Engine is the class that handles all *data* writing to database 
 tables configured in $TCA. In addition the class handles commands such as copy, 
 move, delete." (see :ref:`TCE <t3coreapi:tce-introduction>)
 
 * Which class?
 
 
 FormEngine
 ===========
 
 "FormEngine renders records, usually in the backend." (see :ref:`FormEngine <t3coreapi:FormEngine-Introduction>`)
 
 * Too fuzzy
 
 Suggestion: "FormEngine renders forms for editing records, usually in the backend." 
 
 Fluid
 =====
 
 see `issue on github <https://github.com/TYPO3-Documentation/TYPO3CMS-Guide-Extbase/issues/92>`__
