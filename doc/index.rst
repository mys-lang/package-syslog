|discord|_
|test|_
|stars|_

About
=====

The syslog package in the `Mys programming language`_.

Project: https://github.com/mys-lang/package-syslog

Example
=======

Generate a syslog message.

.. code-block:: mys

   from syslog import SYSLOG
   from syslog import LEVEL_WARNING

   func main():
       SYSLOG(LEVEL_WARNING, "A message.")

The output on a Ubuntu machine:

.. code-block:: myscon

   ❯ mys run
    ✔ Reading package configuration (0 seconds)
    ✔ Building (1.05 seconds)
   ❯ tail -1 /var/log/syslog
   Jul 21 07:57:04 erik-GR8 app: A message.

API
===

.. mysfile:: src/lib.mys

.. |discord| image:: https://img.shields.io/discord/777073391320170507?label=Discord&logo=discord&logoColor=white
.. _discord: https://discord.gg/GFDN7JvWKS

.. |test| image:: https://github.com/mys-lang/package-syslog/actions/workflows/pythonpackage.yml/badge.svg
.. _test: https://github.com/mys-lang/package-syslog/actions/workflows/pythonpackage.yml

.. |stars| image:: https://img.shields.io/github/stars/mys-lang/package-syslog?style=social
.. _stars: https://github.com/mys-lang/package-syslog

.. _Mys programming language: https://mys-lang.org
