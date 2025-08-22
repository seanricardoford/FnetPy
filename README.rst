FnetPy is a Python package to request seismic waveform data from `NIED F-net <http://www.fnet.bosai.go.jp>`_.  

This is forked from `FnetPy <https://github.com/seisman/FnetPy>`_ by `seisman <https://github.com/seisman>`_. Thanks, Dongdong!

Install
=======

::

    pip install https://github.com/seanricardoford/FnetPy/archive/master.zip

Usage
=====

.. code-block::

   from FnetPy import Client
   from datetime import datetime

   starttime = datetime(2011, 1, 2, 5, 10)
   client = Client(username, password)
   client.get_waveform(starttime, duration_in_seconds=300)
