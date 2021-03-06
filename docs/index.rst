.. serialProtocols documentation master file, created by
   sphinx-quickstart on Mon Dec 27 23:45:55 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to serialProtocols's documentation!
===========================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   spi
   uart

When you connect a microcontroller to a sensor, display, or other module, do you ever think about how the two devices talk to each other? What exactly are they saying? 
How are they able to understand each other?

Communication between electronic devices is like communication between humans. Both sides need to speak language. In electronics, these languages are called 
*communication protocols*. Luckily for us, there are only a few communication procols we need to know when building most electronics projects. The three most common proctolos are: 

* **Serial Peripheral Interface (SPI)**
* **Inter-integrated CIrcuit (I2C)**
* **Universal Asynchronous Receiver/Transmitter (UART)**

Purpose
------------
This purpose of this documentation is to give a general overview of the most commont serial procols in Embedded Systems.
The following serial protocols are covered: 

* :ref:`UART`
* :ref:`SPI`

Electronic communication
------------------------

Frst, we’ll begin with some basic concepts about electronic communication.

Serial VS parallel communication
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Electronic devices talk to each other by sending bits of data through wires physically connected between devices. 
A bit is like a letter in a word, except instead of the 26 letters (in the English alphabet), a bit is binary and can only be a 1 or 0. 
Bits are transferred from one device to another by quick changes in voltage. 
In a system operating at 5 V, a 0 bit is communicated as a short pulse of 0 V, and a 1 bit is communicated by a short pulse of 5 V.

The bits of data can be transmitted either in parallel or serial form. In parallel communication, the bits of data are sent all at the same time, 
each through a separate wire. 
Figure 1 shows the parallel transmission of the letter “C” in binary (01000011):

.. image:: images/exampleOfParallelCommunication.PNG

Figure 1. Example of parallel communication.

In serial communication, bits are sent one by one thorugh a single wire. Figure 2 shows the serial transmission of the letter "C" in binary (01000011):

.. image:: images/serialCommunication.PNG

Figure 2. Example of serial communication. 


References 
----------

* `SPI reference <https://www.analog.com/en/analog-dialogue/articles/introduction-to-spi-interface.html>`_
* `SPI reference extention <https://www.circuitbasics.com/basics-of-the-spi-communication-protocol/>`_
* `UART reference <https://www.analog.com/en/analog-dialogue/articles/uart-a-hardware-communication-protocol.html>`_

Author
------

**Name:** Aaron Escoboza Villegas 
**Linkedin:** https://www.linkedin.com/in/aaronev/

Indices and tables
------------------

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
