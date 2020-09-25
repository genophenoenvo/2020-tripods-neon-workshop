.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_

**TRIPODS - HDR Workshop**
==========================

**Times: 09:00 - 14:00 MST, UTC-7**

**Dates: Monday 9th, Tuesday 10th November 2020**

**Ready to join the workshop? Follow these steps:**

**Step 1: Create CyVerse Account (free)** |CyVerse User Portal|

Please use your institutional email address, and if you don't have an |ORCID ID| - sign up for one of those too, they're super important and valuable!

**Step 2: Sign up for Workshop** |Workshop Enrollment| 

**Step 3: Review this website -- all of our training materials will be posted or linked from here**

..
    #### Comment: Use short, imperative titles e.g. Upload and share data, uploading and
    sharing data ####

Goals
-----


**1. Educate one another and engagement between TRIPODS and HDR scientists**

**2. Ensure that we are conducting open science**

**3. Use CyVerse architecture for reproducibile research**

**4. Frame questions for an Institute**

..
    #### Comment: Avoid covering upstream and downstream steps that are not explicitly and
    necessarily part of the tutorial - write or link to separate quick
    starts/tutorials for those parts ####

----

Tutorial Maintainer(s)
------------------------

Who to contact if this guide needs fixing. You can also email
`tswetnam@cyverse.org <tswetnam@cyverse.org>`_

.. list-table::
    :header-rows: 1

    * - Maintainer
      - Institution
      - GitHub Username
    * - Tyson Lee Swetnam
      - CyVerse / University of Arizona
      - tyson-swetnam
    * - Ryan Bartleme
      - CyVerse / University of Arizona
      - rbartleme
----

.. toctree::
	:maxdepth: 2

	Home <self>
  Agenda <agenda.rst>
  Discovery Environment <step1.rst>
  Your Workspace <step2.rst>
  Version Control with GitHub <step5.rst>
  NEON Shiny App <step3.rst>
  Manage your cloud data <step4.rst>
  
..
	#### Comment:This tutorial can have multiple pages. The table of contents assumes
	you have an additional page called 'Step One' with content located in 'step1.rst'
	Edit these titles and filenames as needed ####


Prerequisites
-------------

Downloads, access, and services
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

*In order to complete this tutorial you will need access to the following services/software*

..
	#### comment: delete any row not needed in this table ####

.. list-table::
    :header-rows: 1

    * - Prerequisite
      - Preparation/Notes
      - Link/Download
    * - CyVerse account
      - You will need a CyVerse account to complete this exercise
      - |CyVerse User Portal|
    * - Cyberduck
      - Standalone software for upload/download to Data Store
      - |Download Cyberduck|

Platform(s)
~~~~~~~~~~~

*We will use the following CyVerse platform(s):*

 ..
   #### comment: delete any row not needed in this table ####

.. list-table::
    :header-rows: 1

    * - Platform
      - Interface
      - Link
      - Platform Tour
    * - Data Store
      - GUI/Command line
      - |Data Store|
      - |Data Store Guide|
    * - Discovery Environment
      - Web/Point-and-click
      - |Discovery Environment|
      - |Discovery Environment Guide|
    
Application(s) used
~~~~~~~~~~~~~~~~~~~
..
	#### Comment: these tables are examples, delete whatever is unnecessary ####

**Discovery Environment App(s):**

.. list-table::
    :header-rows: 1

    * - App name
      - Version
      - Description
      - Quick Launch
      - GitHub repositories
    * - Workspace 
      - ``latest``
      - All the Things Geospatial
      -	|workspace-geospatial-latest|_
      - |CyVerse Workspace GitHub|
    * - RStudio 
      - ``3.6.3``
      - Rocker Project RStudio with geospatial applications pre-installed
      - |rstudio-geospatial-3.6.3|_
      - |CyVerse R Studio GitHub|
    * - JupyterLab 
      - ``2.2.5``
      - Jupyter Lab Data Science Notebook with Geospatial applications pre-installed
      - |jupyterlab-geospatial|_
      - |CyVerse JupyterLab GitHub|

Input and example data
~~~~~~~~~~~~~~~~~~~~~~

*In order to complete this tutorial you will need to have the following inputs prepared*

..
	#### comment: delete any row not needed in this table ####

.. list-table::
    :header-rows: 1

    * - Input File(s)
      - Format
      - Preparation/Notes
      - Example Data
    * - |NEON API|
      - various
      - Use in browser or R Studio Shiny App
      - |NEON Shiny Browser|

----

**Fix or improve this documentation**

- Search for an answer:
  |CyVerse Learning Center|
- Ask us for help:
  click |Intercom| on the lower right-hand side of the page
- Report an issue or submit a change:
  |Github Repo Link|
- Send feedback: `learning@CyVerse.org <learning@CyVerse.org>`_

.. comment:

   Uncomment the below and fix with this repo's information if citing

   **Citation**

   You may cite this work as:
   [Repository Title]
   [Author(s)]
   [Repository Release Version]
   [DOI: Zenodo DOI link (generated from Github Release/Zenodo)]
----

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`__


.. Comment: Place Images Below This Line
   use :width: to give a desired width for your image
   use :height: to give a desired height for your image
   replace the image name/location and URL if hyperlinked


 .. |Clickable hyperlinked image| image:: ./img/IMAGENAME.png
    :width: 500
    :height: 100
 .. _CyVerse logo: http://learning.cyverse.org/

 .. |Static image| image:: ./img/IMAGENAME.png
    :width: 25
    :height: 25



.. Comment: Place URLS Below This Line

   # Use this example to ensure that links open in new tabs, avoiding
   # forcing users to leave the document, and making it easy to update links
   # In a single place in this document

   .. |Substitution| raw:: html # Place this anywhere in the text you want a hyperlink

      <a href="REPLACE_THIS_WITH_URL" target="blank">Replace_with_text</a>

.. |Workshop Enrollment|  raw:: html

   <a href="https://user.cyverse.org/workshops/56/overview" target="blank">Workshop Enrollment</a>

.. |ORCID ID| raw:: html

   <a href="https://orcid.org/" target="blank">ORCID ID</a>

.. |workspace-geospatial-latest| image:: https://de.cyverse.org/Powered-By-CyVerse-blue.svg
.. _workspace-geospatial-latest: https://de.cyverse.org/de/?type=quick-launch&quick-launch-id=66f5a2d6-04c3-4346-8804-fab350e2f9b8&app-id=55f4f8b0-f552-11ea-80fa-008cfa5ae621

.. |CyVerse Workspace GitHub|  raw:: html
 
   <a href=" " target="blank">CyVerse Workspace GitHub</a>
  
.. |rstudio-geospatial-3.6.3| image:: https://de.cyverse.org/Powered-By-CyVerse-blue.svg
.. _rstudio-geospatial-3.6.3: https://de.cyverse.org/de/?type=quick-launch&quick-launch-id=e7383172-dafd-42a2-b539-a67a9b65425e&app-id=6943b4f2-b663-11ea-92c5-008cfa5ae621

.. |CyVerse R Studio GitHub|  raw:: html

   <a href="https://github.com/cyverse-vice/rstudio-geospatial" target="blank">CyVerse RStudio GitHub</a>
   
  
.. |CyVerse JupyterLab GitHub|  raw:: html

   <a href=" " target="blank">CyVerse JupyterLab GitHub</a>

.. |jupyterlab-geospatial| image:: https://de.cyverse.org/Powered-By-CyVerse-blue.svg
.. _jupyterlab-geospatial: https://de.cyverse.org/de/?type=quick-launch&quick-launch-id=63afd24c-9acc-4a8c-85ef-58b634a2ebc2&app-id=c940912c-fcea-11ea-b07f-008cfa5ae621

.. |NEON API|  raw:: html

   <a href="https://data.neonscience.org/data-products/explore" target="blank">NEON API</a>

.. |NEON Shiny Browser|  raw:: html

   <a href="https://github.com/cyverse-gis/neon-shiny-browser" target="blank">NEON Shiny Browser</a>

.. |Download Cyberduck|  raw:: html

   <a href="https://cyberduck.io/" target="blank">Download Cyberduck</a>

.. |Github Repo Link|  raw:: html

   <a href="https://github.com/genophenoenvo/2020-tripods-neon-workshop" target="blank">Github Repo Link</a>
