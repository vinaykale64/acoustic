euphony (Home)
==============

|py27| |py36| |black| |pypi| |license|

Have you ever got bored of running long chunks of code?

It can get repetitive to monitor the progress of the code continuously.

Euphony can help you. It is a Python package that plays classical music
in background while your code runs whether it be on terminal or script
or jupyter notebook. Once your code is complete or if it errors out, it
stops so you can go back to it.

How to use
----------

Its pretty simple to use. Create a instance of the ``player`` class and
let your code run enclosed in a ``with`` statement with the object. You
can choose between ``bach``, ``beethoven`` or ``mozart``. If not
specified, it chooses artist randomly.

.. code:: python


     from euphony.player import Player
     mozart = Player(artist = 'mozart') # options: ['bach', 'beethoven']

     with mozart:
         for i in range(1000000000):
             pass
     # plays music while the code runs

That’s all ~!

Note: Since it requires native audio output, you cannot use this when
running code remotely like on AWS.

Installation
------------

Euphony is pip-installable. Just run following cmd in terminal:

.. code:: bash

     pip install euphony


Documentation
-------------

`Link to documentation <https://vinaykale64.github.io/euphony/build/html/includeme.html>`_

.. |py27| image:: https://img.shields.io/badge/python-2.7-brightgreen
.. |py36| image:: https://img.shields.io/badge/python-3.6%2B-brightgreen
.. |black| image:: https://img.shields.io/badge/black--white
.. |pypi| image:: https://img.shields.io/badge/pypi-v0.0.9-blue
.. |license| image:: https://img.shields.io/badge/license-MIT-white
