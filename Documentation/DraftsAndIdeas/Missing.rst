
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
 
 
 
TCE
---
 
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

Softref
=======

`Sofref url <https://docs.typo3.org/typo3cms/CoreApiReference/ApiOverview/SoftReferences/Index.html#url>`__

"URL highlights (with a scheme)."

* What does the word "highlight" mean in this context?
* It says "with a scheme", so I would assume softref=url means complete url with a scheme. However, the pages.url TCA uses softref=url, but it does NOT include the scheme. Instead there is an extra field urltype with the scheme.
