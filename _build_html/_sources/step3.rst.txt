.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


NEON Shiny App
--------------

**Description:**

The `Download and Explore NEON Data API <https://www.neonscience.org/download-explore-neon-data>`_ covered the basics of downloading data directy in R from the ``neonUtilities`` R package.  

Our team created a NEON Shiny App for interfacing with the NEON API in R Studio in a graphical manner.

The Shiny app can be launched using `Docker <https://hub.docker.com/r/cyversevice/shiny-geospatial/neon-shiny-browser>`_, in RStudio or an RStudio-Server. 

When started the Shiny app will create a new folder called ``~/NEON_Downloads`` in the home working directory. For the R Studio instance on CyVerse, this is set as ``/home/rstudio/NEON_Downloads``.

Data that are selected and downloaded go into this folder and are organized using the same ontology as the NEON Data API. 


*Download the Shiny App*
~~~~~~~~~~~~~~~~~~~~~~~~

.. 	#### Comment: Step title should be descriptive (i.e. Cleaning Read data) ###

**1.** Have an instance of RStudio-Server in VICE already started, see `Your Workspace <./step2.html>`_ for details. 

**2.** Click on the ``Terminal`` tab in the R Console

**3.** Type or copy this text into the linux terminal:

   .. code ::

      git clone https://github.com/cyverse-gis/neon-shiny-browser

**4.** The contents of the Git Repository should now be in your workspace files in the lower right of RStudio

**5.** Set the working directory to the ``neon-shiny-browser`` directory

*Starting the Shiny App*
~~~~~~~~~~~~~~~~~~~~~~~~

We are going to run the Shiny app as a background process. This will keep the R Console active and allow us to continue work in the R Studio while the App is running. 

|background_job|

**6.** Select the ``Jobs`` option in the Console

**7.** Set the working directory as ``neon-shiny-browser`` and select the ``background.R`` script.

**8.** Start the Job

   The job should start as a background process.

   By using the Job function, you keep Shiny as a background task which leaves your R Console still available.

**9.** This particular App will likely need to install a few missing dependencies before it starts running. Don't worry, it will do this automatically. After it has installed the missing package dependencies, it should begin to echo out logs and then start to run on the ``localhost`` address number ``127.0.0.1`` using a randomly assigned PORT number:

   .. code ::

      (A bunch of stuff above this...)

      Reading       layer `D19_HEAL_R3_P1_v1' from data source `/home/rstudio/      neon-shi      ny-browser/NEON-data/Flightdata/      Flight_b      oundaries_2017/D19_HEAL_R3_P1_v1      .geojson' using driver       `GeoJSON      '      
      Simple f      e      ature collection with 1 feature       and 4 fields
      geometry             type:  MULTIPOLYGON      
      dimensio      n      :      XY      
      bbox:                 xmin: -149.3151 ymin: 63      .82981 xmax: -149.1116       ymax: 63.93015
      CRS:            4326

      Listening on http://127.0.0.1:5716

  The part we want to copy is the ``http://127.0.0.1:5716``, the ``5716`` number here will be randomly assigned

**10.** Back in the R Console, type the following using the PORT number from the job:

   .. code ::

      rstudioapi::viewer("http://127.0.0.1:5716")      

**11.** The App should start to run and appear in the lower right "Viewer". You can pop the app out into its own browser tab, and begin to use it.    

*Downloading Data via the NEON API*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**12.** Browse the App and find a dataset that you're interested in downloading. 

|neon-shiny|

**13.** AOP data use a slightly different protocol in the NEON Data API, so make sure to select the AOP data check box when you are ready.

**14.** After you've initiated the download, the data will begin being downloaded to the ``~/NEON_Downloads`` folder. 

   When the data download is complete you will get a notification.

**15.** Important: Your data are in a directory which is not set as the WORKDIR by the Docker container in the Discovery Environment. This means that your downloaded data will NOT be saved back to the Data Store when your analysis completes.


**Output/Results**

.. list-table::
    :header-rows: 1

    * - Output
      - Description
      - Notes
    * - NEON Data!
      - Data should be in the ``/home/rstudio/NEON_Downloads`` directory
      - These data use the same file-tree hierarchy as the NEON Data API. 


----

**Description of output and results**


----

**Fix or improve this documentation**

- Search for an answer:
  |CyVerse Learning Center|
- Ask us for help:
  click |Intercom| on the lower right-hand side of the page
- Report an issue or submit a change:
  |Github Repo Link|
- Send feedback: `learning@CyVerse.org <learning@CyVerse.org>`_

----

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_

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

.. |background_job| image:: ./img/shiny_app/background_job.gif
    :width: 800

.. |neon-shiny| image:: https://data.cyverse.org/dav-anon/iplant/home/tswetnam/vice_screencaps/neon-shiny.gif
    :width: 800


.. |Github Repo Link|  raw:: html

   <a href="https://github.com/CyVerse-learning-materials/2020-neon-aop-workshop" target="blank">Github Repo Link</a>

