.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_

`Learning Center Home <http://learning.cyverse.org/>`_

Discovery Environment
---------------------

**Description:**

After you have created your CyVerse account and been granted access to the visual interactive computing environment (VICE) portion of the Discovery Environment data science workbench, you'll be able to start a GUI based app.

..
	#### Comment: short text description goes here ####

----

*The Data Store*
~~~~~~~~~~~~~~~~

|Data Store Guide|

**1.** Click the |data_button| icon labeled **Data**  

**2.** Open your personal user name space in the file browser

  |data_window|
   
   Your space has a path in the data store, e.g.
   
   .. code :: 
     
     /iplant/home/username
   
   This is your personal space, it is private to you. You can create new folders and upload or download files.
   
**3.** Create a new folder called ``NEON_Downloads``

   The new folder is located at:
   
   .. code ::
   
      /iplant/home/username/NEON_Downloads
      
   This folder is private, only you can see it.   

**4.** Share the folder with somone or with the rest of the CyVerse community

   Click on the 'Share' tab and 'Share with Collaborators' option.
   
   Type in a user's given name and it should be searched and pop up. You will not see their ``username``, only their identity and institution information.
   
   You have three options in granting privileges to others: ``read`` ``write`` or ``own``
   
   * ``read`` permissions allows the users to see and download the files and folder
   
   * ``write`` permissions allows the user to modify the file and folder name.
   
   * ``own`` permissions allows the user to modify the file and folder **and the ability to create and delete**
   
   Type in 'Public User' -- adding this user will share the directory with all other CyVerse users.
   
   Type in 'Anonymous User' -- adding this user will share the directory with the open internet (it will become visible on the internet via `https://data.cyverse.org/dav-anon/ <https://data.cyverse.org/dav-anon/>`_

**5.** Look into the Community Data folder

   These are public folders that have been 'shared' with all CyVerse users or with the open internet (via the Anonymous User group): 
   
   .. code ::
   
      /iplant/home/shared/
      
   Navigate to 'cyverse_training/' and 'datasets/'
   
   .. code :: 
          
      /iplant/home/shared/cyverse_training/datasets
   
   There are some sample NEON AOP Data in here that we'll get to tomorrow.
   
   There are many more Community Data folders in CyVerse that you cannot see -- that's because they have not been shared with the 'Public' or 'Anonymous' user groups.

**6.** Look into the 'Shared with Me' folder

   These folders are private user accounts that have public data in them or have been shared with you personally. 

**7.** Access the Data Store from Cyberduck (Windows and Mac OS X only)
   
   Download |Cyberduck| program onto your local computer.
   
   Add the |Cyberduck Profile| file to your installation. This will request your CyVerse credentials.
   
   View the contents of your Data Store. Drag and drop files and Cyberduck will upload / download them for you.
   
**8.** Access the Data Store from WebDav (browser based)

   In your browser, navigate to `https://data.cyverse.org <https://data.cyverse.org>`_
   
   WebDav is a read-only space for viewing data that are already in the data store
  
   The ``https://data.cyverse.org/dav/`` folder path requires authentication with your CyVerse username and password
   
   The ``https://data.cyverse.org/dav-anon/`` folder path is public and anonymous read only to anyone on the interent. 

   .. admonition:: Where does your data live?

     When you download data from the internet to your local computer they're isolated. How do you share them back with your team?

     Many of us use services like Box or Google Drive to hold our files. These services are incredibly useful. 

     However, these file sharing platforms were not designed for machine readability and fast access of many (i.e. thousands to millions) of requests by anonymous users or even by trusted users. (`Google Drive vs Google Cloud <https://suitebriar.com/blog/google-cloud-vs-google-drive>`_)
     
     Conventional file services like FTP (file transfer protocol), function over HTTP and HTTPS. The same is true for Amazon Web Services 'S3' storage object buckets. (`S3 explained <https://dzone.com/articles/confused-by-aws-storage-options-s3-ebs-amp-efs-explained>`_)
     
   .. admonition:: How to work with your data in CyVerse? 
   
     Downloading data from commercial cloud storage providors directly into CyVerse Data Store requires you have a running instance (virtual machine, or container in Discovery Environment) where the data can be staged before moving them onto the Data Store.
     
     Uploading data to CyVerse is dependent upon your local internet service provider. 
     
     
*The App Catalog*
~~~~~~~~~~~~~~~~~

|Apps and Tool Guide|

If you signed up for the workshop, you will have already been added to the NEON Community group.  We have added a couple of apps that have all of the tools needed for the workshop.

These Apps are yours to use! You can install new packages and software into them, but if that becomes too time consuming, consider learning about how to integrate your own Tools and Apps using the Guide link given above. 

*TERMINOLOGY*
+++++++++++++

**App** -- a graphical interface for starting a "Tool" here in the Discovery Environment. The App window can be customized to use any set of conditionals, parameters, resource requirements, input data, or output folders needed to do your analysis.

**Tool** -- a "Tool" is a Docker container which has been added to the Discovery Environment tool manager. It should be public on the Docker Hub or another Docker Registry (e.g. quay.io, NVIDIA NGC, etc.). After a tool has been added to the Discovery Environment using the "Manage Tools" feature in the Apps window, a DE App can be created for it. 


**9.** Click the |apps_button| icon labeled **Apps** 

**10.** Under **Categories** and "My Apps" and "My Communities" you should see a group called NEON

|neon_community|

**11.** In the group are a couple of shared apps with the |beta| tag. 

  In the next section, we're going to go over starting one of these apps, and beginning an Analysis, which you can view using the |analyses_button| icon labeled 'Analyses'



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

.. |Data Store Guide|  raw:: html

   <a href="https://learning.cyverse.org/projects/data_store_guide/en/latest/" target="blank">Data Store Guide</a>

.. |analyses_button| image:: ./img/de/analyses_icon.png
    :width: 25
    :height: 25

.. |apps_button| image:: ./img/de/apps_icon.png
    :width: 25
    :height: 25

.. |data_button| image:: ./img/de/data_icon.png
    :width: 25
    :height: 25

.. |data_window| image:: ./img/de/data_window.png
    :width: 400

.. |neon_community| image:: ./img/de/neon_my_community.png
    :width: 400

.. |Cyberduck|  raw:: html

   <a href="https://cyberduck.io/" target="blank">Cyberduck</a>

.. |Cyberduck Profile|  raw:: html

   <a href="https://learning.cyverse.org/projects/data_store_guide/en/latest/step1.html" target="blank">Cyberduck Profile</a>
   

.. |Apps and Tool Guide| raw:: html

   <a href="https://learning.cyverse.org/en/latest/tools_and_apps.html" target="blank">Apps and Tool Guide</a>

.. |workspace-geospatial-latest| image:: https://de.cyverse.org/Powered-By-CyVerse-blue.svg
.. _workspace-geospatial-latest: 

.. |rstudio-geospatial-3.6.3| image:: https://de.cyverse.org/Powered-By-CyVerse-blue.svg
.. _rstudio-geospatial-3.6.3: https://de.cyverse.org/de/?type=quick-launch&quick-launch-id=e7383172-dafd-42a2-b539-a67a9b65425e&app-id=6943b4f2-b663-11ea-92c5-008cfa5ae621

.. |Github Repo Link|  raw:: html

   <a href="https://github.com/genophenoenvo/2020-tripods-neon-workshop" target="blank">Github Repo Link</a>
