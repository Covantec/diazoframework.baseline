=======================
diazoframework.baseline
=======================


Introduction
============

``diazoframework.skeleton`` package provides the diazo framework implementation of the 
`Baseline CSS framework`_ using the **theming** and **packaging** features available in the 
`diazoframework.plone`_ core package for create `Diazo`_ theme using `plone.app.theming`_.

They are useful for creating themes based on `Baseline CSS framework`_. For documentation 
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

- Provides the *Baseline CSS framework* v0.5.2 resources.
- Included Diazo rules for the **head** that contains the ``base`` CSS styles.
- Included Diazo rules for the **body** that contains the ``columns`` CSS styles.


Installation
============

This add-on can be installed has any other add-ons. It's doesn't have any profile, so 
just add it to your Zope instance, for doing that please the follow steps: 


Buildout
--------

If you are a developer, you might enjoy installing it via buildout.

For install ``diazoframework.baseline`` package add it to your ``buildout`` section's 
*eggs* parameter e.g.: ::

   [buildout]
    ...
    eggs =
        ...
        diazoframework.baseline


and then running ``bin/buildout``.

Or, you can add it as a dependency on your own product ``setup.py`` file: ::

    install_requires=[
        ...
        'diazoframework.baseline',
    ],


Resources
=========

The resources of this framework can be reached through 
``/++framework++baseline`` and there are placed at 
``diazoframework.baseline/diazoframework/baseline/framework/`` 
directory with following resources files:

::

      css
      _ alternate
        _ baseline.ie.css
          _ baseline.reverse.table.css
      _ background-grid
        _ grid.baseline.column.css
        _ grid.baseline.css
        _ grid.column.css
          _ images
           _ baseline+column.png
           _ baseline.png
           _ baseline+unit.png
           _ column.png
           _ unit.png
      _ compressed
        _ baseline.compress.css
          _ baseline.iphone.compress.css
      _ credits.css
      _ deprecated
        _ baseline.form.padding.css
          _ baseline.type.padding.css
      _ iphone
          _ baseline.iphone.css
      _ uncompressed
        _ baseline.base.css
        _ baseline.form.css
        _ baseline.grid.css
        _ baseline.reset.css
        _ baseline.table.css
          _ baseline.type.css
      _ version.history.css
    _ example
      _ forms.html
      _ grid.html
      _ images
        _ baseline+column.png
        _ baseline.png
        _ baseline+unit.png
        _ column.png
        _ header.png
        _ unit.png
        _ untitled.jpg
      _ index.html
      _ iphone.html
      _ lorem.html
      _ scripts
        _ html5.js
      _ tables.html
      _ typography.html
    _ psd templates
      _ Baseline.psd
      _ baseline.pxm
    _ rules
      _ body
        _ columns.xml
      _ head
        _ base.xml
    _ preview.png


Current themes
==============

The `diazoframework.baseline`_ package have the following themes:

`diazotheme.baseline`_
    which contains themes that can both be used as starters for your 
    own *Baseline CSS* based theme.


For more frameworks see: the `diazoframework.plone`_ package.


Contribute
==========

- Issue Tracker: https://github.com/TH-code/diazoframework.baseline/issues
- Source Code: https://github.com/TH-code/diazoframework.baseline


License
=======

The project is licensed under the GPLv2.

The *Baseline CSS framework* is licensed under the Creative Commons Attribution-Share Alike 3.0.

Credits
-------

- Thijs Jonkman (t.jonkman at gmail dot com).


Amazing contributions
---------------------

- Leonardo J. Caballero G. aka macagua (leonardocaballero at gmail dot com).

You can find an updated list of package contributors on https://github.com/TH-code/diazoframework.baseline/contributors


.. _`Baseline CSS framework`: http://baselinecss.com/
.. _`diazoframework.plone`: https://github.com/collective/diazoframework.plone#current-frameworks
.. _`Diazo`: http://diazo.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
.. _`diazoframework.baseline`: https://github.com/TH-code/diazoframework.baseline
.. _`diazotheme.baseline`: https://github.com/TH-code/diazotheme.baseline
