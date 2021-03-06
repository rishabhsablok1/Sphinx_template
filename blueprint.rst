Cheat Sheet: Title
===================

Important code to run in terminal: python -m sphinx -b html . docs

This is a subtitle
------------------

.. DANGER::
   - Here is the link to the cheat sheet -> https://docutils.sourceforge.io/docs/ref/rst/directives.html
   - Here is another one: https://sublime-and-sphinx-guide.readthedocs.io/en/latest/index.html     
   - One more: https://sphinx-rtd-theme.readthedocs.io/en/latest/index.html


This is how a warning sign is displayed
-----------------------------------------

.. DANGER::
    Here is an example warning sign

This is how a note is displayed
--------------------------------

.. NOTE ::
    This is an example note

This is how to bullet something
-------------------------------

My bulleted normal text
    - This is bulleted and indented
    - This one is too (Nested stuff is bolded)
        - This is nested
        - This one is also nested

.. NOTE ::
    This is the topic
        - This is bulleted and indented
        - This too

This is how to get attention
-------------------------------

.. ATTENTION ::
    Attention HERE

This is how to put your own info on the warning thing
---------------------------------------------------------

.. admonition:: Used admonition

    Look at the doc here, admonition used

There is also many others like:
---------------------------------

.. caution::
    Be careful, caution used

.. error::
    This can be used for a error message

.. hint::
    This can be used to give hints

.. important::
    This is important stuff

.. tip::
    Any usefull tip?

.. warning::
    A warning here!

This is how to add an image
-------------------------------

The image has natural size and is left aligned

.. image:: image.png

This image has changed dimensions, and has other features as well

.. image:: image.png
    :height: 100px
    :width: 200px
    :scale: 500%
    :alt: Alternate text here
    :align: center


.. figure:: image.png
    :scale: 50%


    This is the caption for the image


Here is an example of a table with images:
------------------------------------------------


+-----------------------+-----------------------+
| Symbol                | Meaning               |
+=======================+=======================+
| .. image:: image.png  | Campground            |
+-----------------------+-----------------------+
| .. image:: image.png  | Lake                  |
+-----------------------+-----------------------+
| .. image:: image.png  | Mountain              |
+-----------------------+-----------------------+

How to make a ordered list
---------------------------

This is an example of an ordered list
    #. First number
    #. Second number
    #. Third number

How to make a box of text to the left
-----------------------------------------

.. sidebar:: Optional Sidebar Title
   :subtitle: Optional Sidebar Subtitle

   Subsequent indented lines comprise
   the body of the sidebar, and are
   interpreted as body elements.

Anything after the sidebar will come to the left 
of the sidebar, and that is very nice!

How to make topic
------------------

.. topic:: Topic Title

    Subsequent indented lines comprise
    the body of the topic, and are
    interpreted as body elements. If 
    there was more information, it would start 
    wrapping around the sidebar and then start 
    taking up full lines instead of one. So, 
    you can see how it is now taking an whole 
    new area.

This is how to write a code block
----------------------------------

.. note::
    Code blocks can be highlighted using :emphasize-lines:
    with line numbers (Only works in code-block)


.. code-block:: python
    :emphasize-lines: 1, 7

    def my_function() -> None:
        """This is my function, it does nothing

        Returns:
            None
        """
        return None


.. code:: python


    print("How are you")
    print("I am a code not a code-block")


.. code-block:: bash

    Example code


another way of writing quotes is ``env`` this.

Here is the ``single line code``, cannot be used to 
write multiline

I can write math formulas here
--------------------------------

.. note::
    Here is the LATEX information for math -> http://tug.ctan.org/info/short-math-guide/short-math-guide.pdf

.. warning::
    I am using "math" markup without a Sphinx 
    math extension active, please use one of 
    the math extensions described at 
    http://sphinx-doc.org/ext/math.html

.. rubric::
    Here is a rubric, It is nothing but an 
    informal heading

Here is how to write quotes
-------------------------------

.. epigraph::

    East or West I am the best

    -- Rishabh

Highlights
-----------

.. highlights::
    Highlights of the code here

    More information here 

    It looks like indented paragraph


.. compound::

   This is a very nice way of adding some 
   code/information on system commands ::

       clear
       mkdir ABC

This will clear the screen and make a 
directory named ABC

This is what a container looks like
---------------------------------------

.. container:: custom

    This can be used as an container

    More stuff in container:
        #. My first thing
        #. Second thing


    .. image:: image.png

This is another table
-----------------------

.. table::
    :widths: auto
    :align: center


    =====  =====
      A    not A
    =====  =====
    False  True
    True   Falsemmm
    =====  =====


+------+--------+
|  AK  | 99ABCD |
+======+========+
|  99  |   12   |
+------+--------+
|  23  |   kk   |
+------+--------+


A list table
-------------

.. list-table:: A random table here!
    :widths: auto
    :align: center
    :header-rows: 1

    * - Treat
      - Quantity
      - Description
      - OH LOL, another one

    * - Albatros
      - 2.99
      - On a stick
      - A Number Letter Something

    * - Albatros
      - 2.99
      - On a stick
      - B Number Letter Something
    
    * - Lake
      - 299
      - Ostick
      - C Number Letter Something

    * - English
      - 058
      - On a stick
      - D Number Letter Something

    * - New Person
      - 4.23
      - What is this
      - E Number Letter Something

    * - Albatros
      - 2.99
      - On a stick
      - F Number Letter Something

Table of contents:
----------------------

.. contents:: Table of contents
    :depth: 4

The depth can be changed to different values to see 
what is to be nested into the table of contents

The automatic section numbering
---------------------------------

Is done by using sectnum


Date time
----------

.. Warning::
    The date time is the time and date when the 
    code was last written and uploaded


.. |date| date::
.. |time| date:: %H:%M:%S

Todays date is |date|
Time right now is |time| (Refresh to see latest time)

This is how to include a file
-------------------------------

.. Warning::
    There might be some potential security issues

The copy_paste text of the file
*******************************

.. include:: index.rst
    :code: rst


.. include:: my_file.txt

Link to the exact file
************************

.. literalinclude:: index.rst
  :language: rst

Class thing
=============

.. class:: special

This is a "special" paragraph. Here is some 
dummy text to see how the text wraps around 
the text box.

.. class:: exceptional remarkable

An Exceptional Section
----------------------

This is an ordinary paragraph.

.. class:: multiple

   First paragraph.

   Second paragraph.





Heading lists
=================


Here are some headings aranged largest to smallest
------------------------------------------------------


Lower in the nesting
***********************


This is how to add links
------------------------------

`Go google it! <https://google.com>`_


How to change text
===================

Italic -> *Italic Again*
-------------------------

This is an *italic* text


Bold -> **Bold Again**
-----------------------

This is a **bolded** text


.. only:: Internal


    This info is for **internal** people only!



glossary
----------


.. glossary::


    Sphinx
      Sphinx is a tool that makes it easy to create intelligent and beautiful documentation. 
      It was originally created for the Python documentation, and it has excellent facilities 
      for the documentation of software projects in a range of languages.

    RST
      RST is an easy-to-read, what-you-see-is-what-you-get plain text markup syntax 
      and parser system. It is useful for in-line program documentation (such as 
      Python docstrings), for quickly creating simple web pages, and for standalone 
      documents. RST is designed for extensibility for specific application domains. 
      The RST parser is a component of Docutils.

    Sublime Text
      Sublime Text is a sophisticated text editor for code, markup and prose. 
      You'll love the slick user interface, extraordinary features and amazing performance.

