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

1. Click the **Data** button

2. Open your personal user name space in the file browser
   
   Your space has a path in the data store, e.g.
   
   .. code :: 
     
     /iplant/home/username
   
   This is your personal space, it is private to you. You can create new folders and upload or download files.
   
3. Create a new folder called ``NEON_Downloads``

   The new folder is located at:
   
   .. code ::
   
      /iplant/home/username/NEON_Downloads
      
   This folder is private, only you can see it.   

4. Share the folder with somone or with the rest of the CyVerse community

   Click on the 'Share' tab and 'Share with Collaborators' option.
   
   Type in a user's given name and it should be searched and pop up. You will not see their ``username``, only their identity and institution information.
   
   You have three options in granting privileges to others: ``read`` ``write`` or ``own``
   
   * ``read`` permissions allows the users to see and download the files and folder
   
   * ``write`` permissions allows the user to modify the file and folder name.
   
   * ``own`` permissions allows the user to modify the file and folder **and the ability to create and delete**
   
   Type in 'Public User' -- adding this user will share the directory with all other CyVerse users.
   
   Type in 'Anonymous User' -- adding this user will share the directory with the open internet (it will become visible on the internet via `https://data.cyverse.org/dav-anon/ <https://data.cyverse.org/dav-anon/>`_

5. Look into the Community Data folder

   These are public folders that have been 'shared' with all CyVerse users or with the open internet (via the Anonymous User group): 
   
   .. code ::
   
      /iplant/home/shared/
      
   Navigate to 'cyverse_training/' and 'datasets/'
   
   .. code :: 
          
      /iplant/home/shared/cyverse_training/datasets
   
   There are some sample NEON AOP Data in here that we'll get to tomorrow.
   
   There are many more Community Data folders in CyVerse that you cannot see -- that's because they have not been shared with the 'Public' or 'Anonymous' user groups.

6. Look into the 'Shared with Me' folder

   These folders are private user accounts that have public data in them or have been shared with you personally. 

7. Access the Data Store from Cyberduck (Windows and Mac OS X only)
   
   Download |Cyberduck| program onto your local computer.
   
   Add the |Cyberduck Profile| file to your installation. This will request your CyVerse credentials.
   
   View the contents of your Data Store. Drag and drop files and Cyberduck will upload / download them for you.
   
8. Access the Data Store from WebDav (browser based)

   In your browser, navigate to `https://data.cyverse.org <https://data.cyverse.org>`_
   
   WebDav is a read-only space for viewing data that are already in the data store
  
   The ``https://data.cyverse.org/dav/`` folder path requires authentication with your CyVerse username and password
   
   The ``https://data.cyverse.org/dav-anon/`` folder path is public and anonymous read only to anyone on the interent. 

   .. admonition:: Where does your data live?

     When do you download data from the internet to your local computer, you can work on them, but how do you share them with your team?
     
     Keeping your data in the cloud makes them more accessible, and mobile.
     
   .. admonition:: How to work with your data in CyVerse? 
   
     Downloading data from commercial cloud storage providors directly into CyVerse Data Store requires you have a running instance (virtual machine, or container in Discovery Environment) where the data can be staged before moving them onto the Data Store.
     
     Uploading data to CyVerse is dependent upon your local internet service provider. 
     
     
*Starting a VICE app*
~~~~~~~~~~~~~~~~~~~~~

1. Log into the Discovery Environment `https://de.cyverse.org <https://de.cyverse.org>`_

2a. Click one of our quick launch buttons:

   - Workspace: |workspace-geospatial-latest|
   - RStudio: |rstudio-geospatial-3.6.3|
   
2b. Search using the 'Apps' window search bar.

    Search for "workspace geospatial" or "rstudio geospatial" and see what comes up

3. Open the Analyses field to view your running instance.

   .. admonition:: input data

     When you launch a new VICE app, you can add data to it before it is launched. If you do this, it will slow down the launch, as the service must copy the data from the data store into your new instance before it becomes available. 
     
     A faster option is to start the container without the data, and then copy the data into the running container later using WebDav, iCommands, or file system mount.

..
	#### Comment: Suggested style guide:
	1. Steps begin with a verb or preposition: Click on... OR Under the "Results Menu"
	2. Locations of files listed parenthetically, separated by carets, ultimate object in bold
	(Username > analyses > *output*)
	3. Buttons and/or keywords in bold: Click on **Apps** OR select **Arabidopsis**
	4. Primary menu titles in double quotes: Under "Input" choose...
	5. Secondary menu titles or headers in single quotes: For the 'Select Input' option choose...
	####

**Output/Results**

.. list-table::
    :header-rows: 1

    * - Output
      - Description
      - Example
    * -
      -
      -


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

.. |Data Store Guide|  raw:: html

   <a href="https://learning.cyverse.org/projects/data_store_guide/en/latest/" target="blank">Data Store Guide</a>

.. |Cyberduck|  raw:: html

   <a href="https://cyberduck.io/" target="blank">Cyberduck</a>

.. |Cyberduck Profile|  raw:: html

   <a href="https://learning.cyverse.org/projects/data_store_guide/en/latest/step1.html" target="blank">Cyberduck Profile</a>
   
.. |workspace-geospatial-latest| image:: https://de.cyverse.org/Powered-By-CyVerse-blue.svg
.. _workspace-geospatial-latest: 

.. |rstudio-geospatial-3.6.3| image:: https://de.cyverse.org/Powered-By-CyVerse-blue.svg
.. _rstudio-geospatial-3.6.3: https://de.cyverse.org/de/?type=quick-launch&quick-launch-id=e7383172-dafd-42a2-b539-a67a9b65425e&app-id=6943b4f2-b663-11ea-92c5-008cfa5ae621

.. |Github Repo Link|  raw:: html

   <a href="https://github.com/tyson-swetnam/2020-neon-aop-workshop" target="blank">Github Repo Link</a>
