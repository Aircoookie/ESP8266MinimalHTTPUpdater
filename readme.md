This is a simple tool to reflash/upload new binary software to  the ESP8266 micro-controller over-the-air.

Often it can be cumbersome to compile code with lots of dependencies just to use it.
Therefore, some projects (including my WiFi-LED solution WLED) provide ready to flash binaries.
You just need to compile and flash this sketch in the Arduino IDE, the only dependency is the ESP8266 Arduino Core.

Usage:

1. Manually compile and upload the updater.ino sketch to your ESP board via the Arduino IDE. Wait until sketch is fully flashed.

2. Disconnect your ESP8266 from power, wait a second and reconnect it. This is neccessary due to a reset issue after uploading via the IDE.

3. Use a WiFi-enabled device to connect to the board's WiFi Access Point "UpdateMe". The passwort is "updater1".

4. In your browser, type "192.168.4.1" in the address bar. This is the module's IP.

5. You should now see a welcome screen and be able to upload your binary file.