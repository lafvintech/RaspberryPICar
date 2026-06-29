.. _q&a:

Q&A
=====

This section covers common issues you may encounter when using the Raspberry Pi car.
Follow the checks below first, then contact technical support if the problem still remains.

.. note::
   After the first boot following flashing, the car may need some time to initialize.
   If the OLED screen stays blank, wait about 1 minute, power the car off, and then
   power it on again as described in :ref:`assemble_smart_car`.

**No camera image appears in the app**

* **Symptom**: The app connects, but the video window is blank or stops updating.
* **Possible Causes**:

  1. The camera cable is loose.
  2. The Raspberry Pi camera connector is not seated correctly.

* **Solutions**:

  1. Power off the car.
  2. Reconnect the camera cable and make sure the connector is fully inserted.
  3. Power the car on again and reconnect from the app.

**The buzzer beeps twice or four times repeatedly**

* **Symptom**: The buzzer sounds in a regular warning pattern during use.
* **Possible Causes**:

  1. The battery voltage is low.

* **Solutions**:

  1. Replace the batteries with fully charged 18650 batteries.
  2. Recharge the removed batteries before using them again.

**The OLED screen does not display anything after flashing and powering on**

* **Symptom**: The OLED screen remains blank after the car is powered on.
* **Possible Causes**:

  1. The first boot initialization has not finished yet.
  2. The car has not been restarted after the first successful flash.

* **Solutions**:

  1. Wait about 1 minute after the first boot.
  2. Power the car off and then power it on again.
  3. If the Wi-Fi configuration is correct, the OLED screen should display the car's IP address after restart.

**The ultrasonic obstacle avoidance function does not work well**

* **Symptom**: The car does not avoid obstacles reliably.
* **Possible Causes**:

  1. The obstacle is too short for the ultrasonic sensor to detect.
  2. The obstacle is too close or positioned outside the effective detection range.

* **Solutions**:

  1. Use obstacles that are at least 10 cm tall.
  2. Keep the obstacle in front of the car with enough distance for detection.

**The OLED screen does not show the IP address**

* **Symptom**: The car powers on, but the OLED screen does not show an IP address or shows incorrect startup information.
* **Possible Causes**:

  1. The Wi-Fi name, password, or country setting was entered incorrectly during flashing.
  2. The image may not have been flashed successfully.

* **Solutions**:

  1. Review the Wi-Fi configuration in :ref:`system_burning&configuration`, especially Step 5.
  2. Re-flash the image and enter the Wi-Fi settings again.
  3. Restart the car after flashing is complete.

**The app cannot connect even though the OLED shows an IP address**

* **Symptom**: The OLED screen shows a valid IP address, but the phone or computer app cannot connect to the car.
* **Possible Causes**:

  1. The phone or computer is not connected to the same Wi-Fi network as the car.
  2. The main service on the Raspberry Pi is not running normally.

* **Solutions**:

  1. Make sure the car and your phone or computer are connected to the same local network.
  2. Use SSH or VNC to access the Raspberry Pi and run ``sudo systemctl status main-server.service`` to check the service status.
  3. If needed, run ``sudo systemctl start main-server.service`` or restart the car, then try connecting again.

If you still need help, please contact technical support:

* **tech_edu_service@outlook.com**
