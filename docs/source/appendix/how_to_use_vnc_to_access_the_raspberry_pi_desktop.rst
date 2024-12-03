.. _VNC:

How to use VNC to access the Raspberry Pi Desktop
==================================================
Please ensure that you have followed the steps in Chapter One to correctly burn 
the system into your SD card, configure the correct WiFi, and assemble the car 
correctly according to the video.

If everything is confirmed to be ready, we will officially start the tutorial.

Firstly, insert the SD card, install the battery, and ensure the car is powered 
on.

Then, press the two buttons. Under normal circumstances, the two lights next to 
the buttons will light up, and the Raspberry Pi and OLED display will also light 
up. Wait for a while, and the screen will display the IP address, followed by a 
beep from the car's buzzer.

Step 1
------
You need to download and install the  `VNC viewer <https://www.realvnc.com/en/connect/download/viewer/>`_ on personal computer. After the 
installation is done, open it.

Step 2
------
Then select “New connection”.

.. image:: ./img/RemoteDesktop_5.png

Step 3
------
Input IP address of Raspberry Pi and any Name.The IP here is from the car OLED

.. image:: ./img/RemoteDesktop_6.png

Step 4
------
Double click the connection just created:

.. image:: ./img/RemoteDesktop_9.png

Step 5
------
Enter Username (pi) and Password(admin).

.. image:: ./img/RemoteDesktop_7.png

Step 6 
------
Now you can see the desktop of the Raspberry Pi

.. image:: ./img/desktop1.png

.. image:: ./img/desktop2.png


At this point, we have successfully entered the Raspberry Pi system.

If you need to run the car's individual programs, you still need to follow these steps:

Open the terminal

.. image:: ./img/终端.png

Type in: ``sudo systemctl stop main-server.service`` to temporarily disable the 
main program.

.. image:: ./img/trunoff_main-server.png

Then you can navigate to the folder ``/home/pi/Code/Pi4/Server/`` to find all the 
car's files, where you can run individual programs.

If you have finished testing and want to run the main program again, you can 
enter ``sudo systemctl start main-server.service`` in the terminal.

.. image:: ./img/turnon_main-server.png

Alternatively, you can press the two buttons on the car's mainboard to restart 
the car. The restart will automatically launch the car's main program, and then 
you can control the car with the app.

