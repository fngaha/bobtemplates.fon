Introduction
============

``bobtemplates.fon`` provides `mr.bob`_ templates to generate packages for
Plone projects.

Available templates are:

* `Plone`_: a template for a full featured Plone add-on, including:

  * zc.buildout
  * GenericSetup install profile
  * Zope 3 browser layer
  * `z3c.jbot`_ overrides folder
  * ``static/`` resourceDirectory for serving static resources (images, CSS,
    JS, etc.)
  * `Sphinx`_ documentation
  * test suite with test coverage
  * `Travis CI`_ integration


Global settings
---------------

Some answers to bob's questions can be pre-filled based on global configuration
so you don't have to answer them every time. You can store this configuration
either on you local computer, or if you are working in a team, somewhere
online.


Creating a Plone add-on package
-------------------------------

    $ pip install mr.bob
    $ pip install bobtemplates.fon
    $ mrbob --config ~/.mrbob.ini -O collective.foo bobtemplates:plone

Then answer some questions::

    --> Name of the package: foo
    (namespace is already set in the ~/.mrbob.ini)

    ...

And your package is ready!
