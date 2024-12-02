.. _assemble_smart_car:

2.Assemble Smart Car
======================

The link here is a detailed assembly video of the trolley

`<https://youtu.be/4j7h5OY7Oq4>`_

If the site does not open, you can try the following website

`<https://www.bilibili.com/video/BV1jW41197F6>`_


First, after ensuring that the system has been successfully burned, the WiFi is 
configured, and the small car is assembled, we can officially use the small car.

We install the Raspberry Pi small car with 3*18650 batteries and power it on. 
Note that when it is powered on for the first time, the small car needs to 
perform some initialization, and the OLED screen usually does not display at 
this time. You can wait for a minute, then press to turn off the power of the 
small car (the two buttons on the small car pop up), and then power it on again 
(the two buttons on the small car are pressed down).


.. image:: ./img/2/侧面.png

After that, we should be able to see the OLED display normally.

.. image:: ./img/2/oled(1).jpg

.. image:: ./img/2/oled(2).jpg

Once we can see the OLED display as described above, it means the system has 
obtained an IP address, which is the normal behavior. If the system fails to 
obtain an IP address and the OLED screen displays "IP not found," please refer 
to the steps in the following section, specifically Step 5, to check your WiFi 
configuration during the burning process and re-burn the system if necessary.

* :ref:`system_burning&configuration`

.. image:: ./img/1/image15(1).png