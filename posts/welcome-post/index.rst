.. title: Welcome post!
.. slug: welcome-post
.. date: 2016-11-25 13:09:04 UTC-08:00
.. tags: 
.. category: general 
.. link: 
.. description: 
.. type: text

Welcome to the SWOT-DA blog! Similar to the `SWOT Discharge Algorithm Working Group blog <https://swotdawg.wordpress.com>`_, we will use this blog to go through the development of data assimilation algorithms for SWOT observations, and an inter-comparison experiment. The latter will use the same datasets as the `Pepsi challenge <https://swotdawg.wordpress.com/2014/06/19/pepsi-challenge-plan/>`_.

.. TEASER_END

In terms of writing blog posts, I've used the `Nikola <https://getnikola.com>`_ static site generator. Nikola is based on Python, so we'll need to install it using pip

.. code-block:: bash

   pip install nikola

Since the blog is hosted on Github, the blog contents can be downloaded by

.. code-block:: bash

   git clone https://github.com/swot-da/swot-da.github.io.git
   git fetch
   git checkout sources


After you switch to the `swot-da.github.io` directory, a new post can be started with

.. code-block:: bash

   nikola new_post

which will create a page in Markdown language, under the `posts` directory. Please consult the `reStructuredText primer <http://www.sphinx-doc.org/en/stable/rest.html>`_ for information on the syntax you can use to write your post.

After you finish writing your post, you can test it out by running

.. code-block:: bash

   nikola build
   nikola serve

and examining the blog at `http:localhost:8000 <localhost:8000>`_. The blog post can then be deployed by running

.. code-block:: bash

   nikola github_deploy
