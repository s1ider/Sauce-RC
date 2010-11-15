Sauce RC
========

Sauce RC is a commercially supported, open-source distribution of `Selenium 
<http://saucelabs.com/docs/quickstart>`_ RC from `Sauce Labs <http://saucelabs.com/>`_.

Source Organization
===================

* Controller is the web backend that does the actual work
* win32 hold the win32 GUI
* mac holds the mac script and app compiling profile
* All the files in the root directory are just used for building the different executables

Running
=======
For dev running, just do:

  ./controler/server.py

Building
========
Just run `make [windows|mac]`.

Dependencies
------------

* See dependencies in Makefile
* On Windows, we're building under the msys-git shell, just run `make windows`.

To create a new build do:

* `prebuild`
* `make [windows|mac]`
* Run some tests
* `tag-build` (if you're happy with the build)

.. comment: vim:spell
