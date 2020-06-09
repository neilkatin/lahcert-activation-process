
LAH CERT Actions After an Earthquake
======================================

This is the document source for the Los Altos Hills CERT (Community Emergency Response Team)
and ECC (Emergency Communications Committee) action after an earthquake.

The documents is available online on [los-altos-hills-initial-deployment-guide.readthedocs.io](https://los-altos-hills-initial-deployment-guide.readthedocs.io/en/latest/).

This git repository holds the source to that document.  The document is authored in
[RestructuredText](https://docutils.sourceforge.io/rst.html) using the
[Sphinx publishing system](https://www.sphinx-doc.org/en/master/).

Building -- system packages
--------

I (Neil) did development on Windows using Cygwin.  The [cygwin-packagex.txt](cygwin-packages.txt)
document describes the extra cygwin packages that needed to be installed.

Building -- python
-----------

I use python 3.8 and pipenv to manage my python packages and virtual environment.
Use these steps to get up and running (from the root of the git repo):

```shell
pipenv --python 3.8
pipenv update
pipenv make autobuild
```

This will start a web server on [http://127.0.0.1:8000/](http://127.0.0.1:8000/) that will
update the web page every time a file changes in the tree.

Publishing
----------

The readthedocs.io site is set to republish ever time the git repo changes; please use a branch other
than "master" for any drafts.



