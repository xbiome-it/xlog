.. raw:: html

    <p align="center">
        <a href="#readme">
            <img alt="Xlog logo" src="https://www.xbiome.cn/images/logo.png">
        </a>
    </p>
    <p align="center">
        <a href="https://pypi.org/project/xlog/"><img alt="Pypi version" src="https://img.shields.io/pypi/v/loguru.svg"></a>
        <a href="https://pypi.org/project/xlog/"><img alt="Python versions" src="https://img.shields.io/badge/python-3.5%2B%20%7C%20PyPy-blue.svg"></a>
        <a href="https://pypi.org/project/xlog/"><img alt="Documentation" src="https://img.shields.io/readthedocs/loguru.svg"></a>
        <a href="https://pypi.org/project/xlog/"><img alt="Build status" src="https://img.shields.io/travis/Delgan/loguru/master.svg"></a>
        <a href="https://pypi.org/project/xlog/"><img alt="Coverage" src="https://img.shields.io/codecov/c/github/delgan/loguru/master.svg"></a>
        <a href="https://pypi.org/project/xlog/"><img alt="Code quality" src="https://img.shields.io/codacy/grade/4d97edb1bb734a0d9a684a700a84f555.svg"></a>
        <a href="https://pypi.org/project/xlog/"><img alt="License" src="https://img.shields.io/github/license/delgan/loguru.svg"></a>
    </p>

=========

**Xlog** 
Xbiome logging Frame in Python.


.. end-of-readme-intro

Installation
------------

::

    pip3 install xlog


Features
--------

* Format the pipeline logging.


Take the tour
-------------

Ready to use it with simple method.
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
::

    from xlog import xlog

    xlog.init('ProjectName','LogPath')

    xlog.logger('YourMessage','LogLevel')

OutPut Example:
-----------------

>>> from xlog import xlog
>>> xlog.init('16s','./')
>>> xlog.logger('This is a INFO log test!!!','INFO')
>>> xlog.logger('This is a DEBUG log test!!!','DEBUG')
>>> xlog.logger('This is a ERROR log test!!!','ERROR')


After that we will get three files: 

In 16s_2020-11-10_INFO.log
::

	2020-11-10-15:26:23  |  INFO  |  This is a INFO log test!!!
	2020-11-10-15:26:48  |  ERROR  |  This is a ERROR log test!!!

In 16s_2020-11-10_DEBUG.log
::
	2020-11-10-15:26:23  |  INFO  |  This is a INFO log test!!!
	2020-11-10-15:26:35  |  DEBUG  |  This is a DEBUG log test!!!
	2020-11-10-15:26:48  |  ERROR  |  This is a ERROR log test!!!

In 16s_2020-11-10_ERROR.log
::
	2020-11-10-15:26:48  |  ERROR  |  This is a ERROR log test!!!	
