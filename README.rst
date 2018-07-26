=======================
diazoframework.baseline
=======================


Introduction
============

``diazoframework.baseline`` package provides the diazo framework implementation 
of the `Baseline CSS framework`_ using the **theming** and **packaging** 
features available for create Diazo_ theme using `plone.app.theming`_. 

They are useful for creating themes based on `Baseline CSS framework`_. 
A Diazo framework should provide the framework resources and diazo rules to reuse 
and add to in a Diazo theme.


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest version (https://plone.org/download)
- The ``plone.app.theming`` package (*You will need enable it via ``Add-ons`` control 
  panel to use this package*)
- The ``diazoframework.plone`` package (*You will need enable it via ``buildout`` 
  configuration to use this package*)


Features
========

- Provides the *Baseline CSS framework* resources.
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

    _ css
    _ example
    _ psd templates
    _ rules
      _ body
        _ columns.xml
      _ head
        _ base.xml
    _ preview.png


Current themes
==============

The `diazoframework.baseline <https://github.com/TH-code/diazoframework.baseline>`_ package have the following themes:

- `diazotheme.baseline <https://github.com/TH-code/diazotheme.baseline>`_.


Contribute
==========

- Issue Tracker: https://github.com/TH-code/diazoframework.baseline/issues
- Source Code: https://github.com/TH-code/diazoframework.baseline


License
=======

The project is licensed under the GPLv2.


Credits
-------

- Thijs Jonkman (t.jonkman at gmail dot com).


Amazing contributions
---------------------

- Leonardo J. Caballero G. aka macagua (leonardocaballero at gmail dot com).

You can find an updated list of package contributors on https://github.com/TH-code/diazoframework.baseline/contributors


.. _`Baseline CSS framework`: http://baselinecss.com/
.. _`diazoframework.baseline`: https://github.com/TH-code/diazoframework.baseline
.. _`Diazo`: http://diazo.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
