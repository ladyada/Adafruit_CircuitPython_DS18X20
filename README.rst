
Introduction
============

.. image:: https://readthedocs.org/projects/adafruit-circuitpython-ds18x20/badge/?version=latest
    :target: https://circuitpython.readthedocs.io/projects/ds18x20/en/latest/
    :alt: Documentation Status

.. image :: https://img.shields.io/discord/327254708534116352.svg
    :target: https://adafru.it/discord
    :alt: Discord

.. image:: https://travis-ci.com/adafruit/Adafruit_CircuitPython_DS18X20.svg?branch=master
    :target: https://travis-ci.com/adafruit/Adafruit_CircuitPython_DS18X20
    :alt: Build Status

CircuitPython driver for Dallas 1-Wire temperature sensor.

Dependencies
=============
This driver depends on:

* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
* `Adafruit OneWire <https://github.com/adafruit/Adafruit_CircuitPython_OneWire>`_

Please ensure all dependencies are available on the CircuitPython filesystem.
This is easily achieved by downloading
`the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.

Installing from PyPI
====================

On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
PyPI <https://pypi.org/project/adafruit-circuitpython-ds18x20/>`_. To install for current user:

.. code-block:: shell

    pip3 install adafruit-circuitpython-ds18x20

To install system-wide (this may be required in some cases):

.. code-block:: shell

    sudo pip3 install adafruit-circuitpython-ds18x20

To install in a virtual environment in your current project:

.. code-block:: shell

    mkdir project-name && cd project-name
    python3 -m venv .env
    source .env/bin/activate
    pip3 install adafruit-circuitpython-ds18x20

Usage Example
=============

.. code-block:: python

    import board
    from adafruit_onewire.bus import OneWireBus
    from adafruit_ds18x20 import DS18X20
    ow_bus = OneWireBus(board.D2)
    ds18 = DS18X20(ow_bus, ow_bus.scan()[0])
    ds18.temperature


Contributing
============

Contributions are welcome! Please read our `Code of Conduct
<https://github.com/adafruit/Adafruit_CircuitPython_DS18X20/blob/master/CODE_OF_CONDUCT.md>`_
before contributing to help this project stay welcoming.

Documentation
=============

For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
