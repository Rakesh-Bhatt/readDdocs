.. Read the docs tutorial documentation master file, created by
   sphinx-quickstart on Fri Nov 19 12:31:54 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Read the docs tutorial's documentation!
==================================================

This file is created for the sole purpose of getting the detailed knowledge of 
``reStructured`` text with ``sphinx`` and later on using
**read the docs to host the project**

.. note::
   new changes here

.. caution:: 
   please pay attention to the documentation given.
   We can use following element of Admonition here 
   
   #. Caution 
   #. Tip
   #. Danger
   #. Note



We can provide links of our project inside the index page
Click here :doc:`/Options/hyperlink`


for another type of hyperlink :doc:`Click me </Options/hyperlink>`

To link on specific page on specificlocation you have to 
create an link of that location lets say inside Guidelines.
:ref:`Go inside Guidelines => content page <here>`

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Options:

   Options/justlogic
   Options/justcode
   Options/bullet
   Options/show
   Options/table
   Options/hyperlink
   

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Guidelines:

   Guidelines/content


.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Fun:

   Fun/fun
.. toctree::
   :maxdepth: 2
   :hidden:
   
   billingSection


