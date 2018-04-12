
.. With the following include we import some definition. We do this in each and every file.
so we can change the definition at a single place. Use the relative path to the Includes.txt file,
which may look as well like ../../../Includes.txt for a deeply nested source file.

.. include:: ../../Includes.txt


.. Usually we define 'php' as default highlight language in Includes.txt.
With the following 'highlight' directive we switch to reStructuredText as default highlight language.

.. highlight:: bash


.. The following, first section (= headline) is the 'Document Title'.


===============
Rendering Guide
===============

Hier weitere Infos zum lokalen Rendern.

Dies ist mein Pull request:

https://github.com/TYPO3-Documentation/TYPO3CMS-Guide-ContributionWorkflow/pull/43

Dort steht auch, was sich geändert hat. Im Wesentlichen sind einige Kapitel dazugekommen.

Wenn der PR noch nicht gemerged wurde, kann man folgendendermaßen vorgehen, um sich den aktuellen Stand lokal zu rendern
(da es ziemlich mühselig ist, sich die diffs anzusehen).

Wie sonst auch üblich clonen:

::

   git clone https://github.com/sypets/TYPO3CMS-Guide-ContributionWorkflow.git
   cd TYPO3CMS-Guide-ContributionWorkflow
   git checkout one-big-pull-request

Dies kann mit dem docker image von Martin Bless gerendert werden:


   source <(docker run --rm t3docs/render-documentation show-shell-commands)
   dockrun_t3rdf makehtml


s. https://github.com/t3docs/docker-render-documentation


Die gerenderten HTML-Dateien befinden sich dann unter Documentation-GENERATED-temp/typo3cms/drafts/project/0.0.0/ und können mit dem Browser
gesichtet werden.

