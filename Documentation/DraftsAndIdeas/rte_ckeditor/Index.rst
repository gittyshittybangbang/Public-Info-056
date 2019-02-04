.. include:: ../../Includes.txt
.. highlight:: rst

===================
DRAFT: rte_ckeditor
===================


* `github issue <https://github.com/TYPO3-Documentation/T3DocTeam/issues/25>`__
* patch: https://review.typo3.org/c/59627/
* draft is here: :ref:`rte_ckeditor`

.. important::

   The draft here is not kept up to date, see latest version is in patch
   https://review.typo3.org/c/59627/ and render locally!


**Quickstart: How to get latest TYPO3 core, apply the patch and render with Docker**

.. rst-class:: bignums

1. Get TYPO3 source

   .. code-block:: bash


      git clone git://git.typo3.org/Packages/TYPO3.CMS.git t3coredev
      cd t3coredev


2. Apply patch

   - Go to https://review.typo3.org/c/59627/
   - Click Download
   - Click "copy" on the right of the line "Cherry Pick"
   - Paste the command to your shell

   see https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/HandlingAPatch/CherryPick.html

3. Render


   .. code-block:: bash

      cd typo3/sysext/rte_ckeditor
      source <(docker run --rm t3docs/render-documentation show-shell-commands)
      dockrun_t3rdf makehtml


   Now, open file Documentation-GENERATED-temp/Result/project/0.0.0/Index.html in Browser

   See https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/AddingDocumentation/Index.html#render-the-changelog

4. Review the patch

   Go to: https://review.typo3.org/c/59627/

   see https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/HandlingAPatch/Review.html



.. toctree::
   :hidden:

   Documentation/Index
