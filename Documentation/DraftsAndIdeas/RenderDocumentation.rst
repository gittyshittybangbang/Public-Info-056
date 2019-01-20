.. include:: ../Includes.txt
.. highlight:: bash

.. _rendering-docs-quickstart:


.. important::

   This section is currently under construction.


About this page: This is an alternative approach to the documentation on
`t3docs/docker-render-documentation
<https://github.com/t3docs/docker-render-documentation/blob/master/README.rst>`__

The difference is it addresses all three platforms (MacOS, Linux, Windows),
only lists the commands
absolutely needed and addresses the question of how to open the generated docs.

Additionally it adds an alternative workflow using docker-compose which was
originally proposed in `issue #14
<https://github.com/t3docs/docker-render-documentation/issues/14>`__

A solution using PowerShell was used, slightly modified, see `issue #13
<https://github.com/t3docs/docker-render-documentation/issues/13>`__

The various methods should ideally be stripped down to one best practice.

Once the documentation here has matured, we can think about merging it with:
`t3docs/docker-render-documentation
<https://github.com/t3docs/docker-render-documentation/blob/master/README.rst>`__


==========================================
DRAFT: Rendering Documentation with Docker
==========================================

We offer a Docker image for rendering the documentation on your local computer. Using
our Docker image you do not have to install the required packages (e.g. sphinx) on your
computer.



Render on Linux
===============

Run these commands in a terminal in the parent directory of the Documentation
directory every time you wish to render:

.. code-block:: bash
   :linenos:

   docker pull t3docs/render-documentation
   source <(docker run --rm t3docs/render-documentation show-shell-commands)
   dockrun_t3rdf makehtml
   xdg-open "Documentation-GENERATED-temp/Result/project/0.0.0/Index.html"

Explantations, the numbers correspond to the line numbers in code snippet:

#. **docker pull**
   You can run this every time before docker run, but it is not necessary
   unless you want to make sure the docker image gets updated.
   The next run will usually be faster because
   it will only pull (download) the Docker image again if a newer one is
   available.
#. **Prepare dockrun_t3rdf:**
   This will not only run the Docker container, it
   will make the command `dockrun_t3rdf` available in your current terminal.
   You must do this again for every new terminal you open.
   This command may take a while.
#. **Render the documentation:** This will automatically find the documentation
   in the :file:`Documentation`
   subfolder. It will create a directory :file:`Documentation-GENERATED-temp`
   and write the results there.
#. **View the documentation:**
   You can now view the rendered documentation in your browser.
   Look at the hints that are shown in the terminal.
   If you structured the documentation correctly, :file:`Index.rst` is
   always on the top level directory under the directory :file:`Documentation`.
   The renderer will create the file :file:`Index.html` from that. The path
   is always the same.
   If xdg-open does not work for you, create a URL you can open::

      echo "file://"$(pwd)/"Documentation-GENERATED-temp/Result/project/0.0.0/Index.html"


When you make additional changes, you can run step 3 again and reload page
in browser.

.. tip::

   Press reload (e.g. :kbd:`ctrl + r`) in your browser to view the changes.

Render on MacOS
===============

Run the same commands as for Linux but replace xdg-open with open:

.. code-block:: bash
   :linenos:

   docker pull t3docs/render-documentation
   source <(docker run --rm t3docs/render-documentation show-shell-commands)
   dockrun_t3rdf makehtml
   open "Documentation-GENERATED-temp/Result/project/0.0.0/Index.html"

If open does not work for you, create a URL you can open in browser::

   echo "file://"$(pwd)/"Documentation-GENERATED-temp/Result/project/0.0.0/Index.html"

You may also want to try :ref:`render-with-docker-compose` for an
alternative workflow.

Render on Windows
=================

**Recommended:** Try :ref:`render-with-docker-compose`.

With Powershell
----------------

You can directly run the following commands or create a script, for example t3docmake.ps1,
containing::

   docker run --rm -v "$($PWD):/PROJECT/:ro" -v "$($PWD)\Documentation-GENERATED-temp\:/RESULT/" t3docs/render-documentation makehtml;
   start "$PWD/Documentation-GENERATED-temp/Result/project/0.0.0/Index.html"

Then execute the script, e.g.::

   ../t3docmake.ps1
   


.. todo:
.. https://www.borncity.com/blog/2010/02/24/powershell-skripte-lassen-sich-nicht-ausfhren/
.. https://blogs.msdn.microsoft.com/powershell/2011/06/03/invoke-expression-considered-harmful/


.. _render-with-docker-compose:

Render With Docker Compose
==========================


The commands previously described may not work on your system. Additionally,
you may find that once you have set it up, working with Docker Compose
will simplify the workflow.

Prerequisites:

* Additionally to Docker, you will need to install Docker Compose. On Mac
  or Windows this will most likely already be the case, see `Install Docker Compose
  <https://docs.docker.com/compose/install/>`__: *On desktop systems like Docker
  Desktop for Mac and Windows, Docker Compose is included as part of those desktop installs.*

#. Create a docker-compose.yml file. This will usually be the same for all
   documentation projects.

   .. code-block:: yaml
      :lineno:

         version: '2'
         services:
            t3docmake:
               image: t3docs/render-documentation:latest
               volumes:
               - ./:/PROJECT:ro
               - ./Documentation-GENERATED-temp:/RESULT
               command: makehtml

#. Run docker-compose

   If docker-compose.yml exists::

      docker-compose up

   If yaml file is named differently::

      docker-compose -f <path> up


Additional Information
======================

* `Docker Compose Version <https://docs.docker.com/compose/compose-file/>`__
* `StackOverflow: Difference Between docker-compose up and docker-compose run <https://stackoverflow.com/questions/33066528/should-i-use-docker-compose-up-or-run>`__



