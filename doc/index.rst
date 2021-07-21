|test|_

About
=====

The syslog package in the `Mys programming language`_.

Project: https://github.com/mys-lang/package-syslog

Example
=======

Generate a syslog message.

.. code-block:: python

   from syslog import syslog
   from syslog import LEVEL_WARNING

   def main():
       syslog(LEVEL_WARNING, "A message.")

The output on a Ubuntu machine:

.. code-block:: text

   $ mys run
   ...
   $ tail -1 /var/log/syslog
   Jul 21 07:57:04 erik-GR8 app: A message.

API
===

.. mysfile:: src/lib.mys

.. |test| image:: https://github.com/mys-lang/package-syslog/actions/workflows/pythonpackage.yml/badge.svg
.. _test: https://github.com/mys-lang/package-syslog/actions/workflows/pythonpackage.yml

.. _Mys programming language: https://mys-lang.org
