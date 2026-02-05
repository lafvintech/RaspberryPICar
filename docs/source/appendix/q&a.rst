.. _q&a:

Q&A
=====

This section lists some common issues you might encounter and provides solutions for them.
--------------------------------------------------------

Q: What should you do if there is suddenly no image during use?

A: It could be that the camera or the Raspberry Pi interface has become loose. Reinstall it and restart the car by pressing the power button, then reconnect.

Q: What if the car's buzzer beeps twice or four times in a regular pattern while in use?

A: This is a battery warning from the car, indicating that the car's battery is low. It is recommended to replace the batteries and recharge them.

Q: What should you do if the OLED does not display anything after the car is burned and started?

A: After the car's first burn, it needs to be restarted. Once restarted, if your WiFi configuration is correct, the OLED will display the car's IP address.

Q: What if the car's ultrasonic sensor fails to avoid obstacles successfully?

A: The obstacle needs to be at least 10cm in height and maintain a certain distance.

Q: If the OLED does not display the IP address and operation information properly after the cart is burned in, the OLED will not display the IP address and operation information properly.

A: It is possible that the trolley has not been burned successfully, so it is recommended to re-burn it.

Q: If the trolley can get the IP address, but can not connect to the trolley through the APP.

A:Please check whether the cell phone and the cart are connected to the same WiFi network; if the cart is sure in the same network, you can ssh into the Raspberry Pi and type ``sudo systemctl status main-server.service`` to check whether the cart service is running normally.

If you encounter any issues beyond the above, please contact us for assistance:

- 官方技术支持邮箱： **tech_edu_service@outlook.com**

