glom
====

*Restructuring data, the Python way*

|release| |calver|

**glom** is a new approach to working with data in Python, featuring:

* :ref:`Path-based access <access-granted>` for nested structures
* :ref:`Declarative data transformation <glom-func>` using lightweight, Pythonic specifications
* Readable, meaningful :ref:`error messages <exceptions>`
* Built-in :ref:`data exploration and debugging <debugging>` features
* And *more*!

While it may sound like a lot, glom's straightforward approach becomes
second-nature very quickly. :doc:`Get started with the five-minute
tutorial! <tutorial>`

Installation
------------

glom is pure Python, and tested on Python 2.7-3.7, as well as
PyPy. Installation is easy::

  pip install glom

Then you're ready to get glomming!

.. code-block:: python

   from glom import glom

   target = {'a': {'b': {'c': 'd'}}}
   glom(target, 'a.b.c')  # returns 'd'

There's much, much more to glom, check out the :doc:`tutorial` and :doc:`API reference<api>`!


*Just glom it! ☄️*


.. |release| image:: https://img.shields.io/pypi/v/glom.svg
             :target: https://pypi.org/project/glom/

.. |calver| image:: https://img.shields.io/badge/calver-YY.MINOR.MICRO-22bfda.svg
            :target: https://calver.org

.. toctree::
   :maxdepth: 2

   tutorial
   api
   cli
   faq
   by_analogy
   snippets
