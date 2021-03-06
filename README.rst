========================
diazoframework.bootstrap
========================


Introduction
============

``diazoframework.bootstrap`` package provides the diazo framework implementation of the 
`Twitter Bootstrap CSS framework`_ using the **theming** and **packaging** features available in the 
`diazoframework.plone`_ core package for create `Diazo`_ theme using `plone.app.theming`_.

They are useful for creating themes based on `Twitter Bootstrap CSS framework`_. For documentation 
on the framework itself, check the website.

A Diazo framework should provide the framework resources and diazo rules to reuse 
and add to in a Diazo theme.


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest version (https://plone.org/download)
- The ``plone.app.theming`` package (*You will need enable it via "Add-ons" control 
  panel to use this package*)
- The ``diazoframework.plone`` package (*You will need enable it via "buildout" 
  configuration to use this package*)


Features
========

- Provides the *Twitter Bootstrap CSS framework* v2.2.2 resources.
- Provides the *Twitter Bootstrap Starter Theme* resources.
- Included Diazo rules for the **head** that contains ``base`` and ``theme`` CSS styles.
- Included Diazo rules for the **body** that contains ``columns-narrow``, ``columns``, 
  ``content``, ``edit``, ``footer-inverse``, ``footer-narrow-inverse``, ``footer-narrow``, 
  ``footer``, ``forms``, ``general``, ``general-narrow``, ``grid``, ``header-inverse``, 
  ``header-narrow``, ``header``, ``lead-hero``, ``lead-jumbotron``, ``lead``, ``no-edit`` 
  and ``portlets`` CSS styles.


Installation
============

This add-on can be installed has any other add-ons. It's doesn't have any profile, so 
just add it to your Zope instance, for doing that please the follow steps: 


Buildout
--------

If you are a developer, you might enjoy installing it via buildout.

For install ``diazoframework.bootstrap`` package add it to your ``buildout`` section's 
*eggs* parameter e.g.: ::

   [buildout]
    ...
    eggs =
        ...
        diazoframework.bootstrap


and then running ``bin/buildout``.

Or, you can add it as a dependency on your own product ``setup.py`` file: ::

    install_requires=[
        ...
        'diazoframework.bootstrap',
    ],


Resources
=========

The resources of this framework can be reached through 
``/++framework++bootstrap`` and there are placed at 
``diazoframework.bootstrap/diazoframework/bootstrap/framework/`` 
directory with following resources files:

::

    _ carousel.html
    _ css
      _ bootstrap.css
      _ bootstrap.min.css
      _ bootstrap-responsive.css
      _ bootstrap-responsive.min.css
    _ fluid.html
    _ hero.html
    _ img
      _ glyphicons-halflings.png
      _ glyphicons-halflings-white.png
    _ index.html
    _ js
      _ bootstrap.js
      _ bootstrap.min.js
    _ marketing-narrow.html
    _ preview.png
    _ rules
      _ body
        _ columns.xml
        _ columns-narrow.xml
        _ content.xml
        _ edit.xml
        _ footer.xml
        _ footer-inverse.xml
        _ footer-narrow.xml
        _ footer-narrow-inverse.xml
        _ forms.xml
        _ general.xml
        _ general-narrow.xml
        _ grid.xml
        _ header.xml
        _ header-inverse.xml
        _ header-narrow.xml
        _ lead.xml
        _ lead-hero.xml
        _ lead-jumbotron.xml
        _ no-edit.xml
        _ portlets.xml
      _ head
        _ base.xml
        _ theme.xml
    _ starter-template.html
    _ sticky-footer.html


Current themes
==============

The `diazoframework.bootstrap`_ package have the following themes:

`diazotheme.bootstrap <https://github.com/TH-code/diazotheme.bootstrap>`_
   which contains themes that can both be used as starters for your own Twitter Bootstrap based theme.

`diazotheme.bootswatch <https://github.com/collective/diazotheme.bootswatch>`_
   A bootswatch childthemes examples from ``diazoframework.bootstrap``.

`diazotheme.frameworks <https://github.com/collective/diazotheme.frameworks>`_
   A collection of Diazo themes with support to many CSS Frameworks like *Twitter Bootstrap*.


For more frameworks see: the `diazoframework.plone`_ package.


Contribute
==========

- Issue Tracker: https://github.com/collective/diazoframework.bootstrap/issues
- Source Code: https://github.com/collective/diazoframework.bootstrap


License
=======

The project is licensed under the GPLv2.

The *Twitter Bootstrap CSS framework* is licensed under the Apache v2.0.


Credits
-------

- Thijs Jonkman (t.jonkman at gmail dot com).


Amazing contributions
---------------------

- Leonardo J. Caballero G. aka macagua (leonardocaballero at gmail dot com).

You can find an updated list of package contributors on https://github.com/collective/diazoframework.bootstrap/contributors


.. _`Twitter Bootstrap CSS framework`: http://twitter.github.io/bootstrap/
.. _`diazoframework.plone`: https://github.com/collective/diazoframework.plone#current-frameworks
.. _`Diazo`: http://diazo.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
.. _`diazoframework.bootstrap`: https://github.com/collective/diazoframework.bootstrap
