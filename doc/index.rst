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

The output:

.. code-block:: text

   $ mys run
   ...
   $ tail /var/log/syslog
   ...

API
===

.. mysfile:: src/lib.mys

.. _Mys programming language: https://mys-lang.org
