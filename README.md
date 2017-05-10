# FauxMoESP_WS2812FX
Control WS2812 RGB & RGBW pixels from Alexa using a NodeMCU ESP8266.

## Requirements
### Hardware
This code was tested on a HiLetgo NodeMCU ESP8266 board. You need some WS2812B LEDs (e.g. NeoPixel) connected to 5V and GND and a data pin of the ESP8266.

### Software
You need to install the following additional libraries to compile the code:<br>
Adafruit_NeoPixel: https://github.com/adafruit/Adafruit_NeoPixel<br>
ESPAsyncTCP: https://github.com/me-no-dev/ESPAsyncTCP<br>
ESPAsyncWebServer: https://github.com/me-no-dev/ESPAsyncWebServer<br>
FauxmoESP: https://bitbucket.org/xoseperez/fauxmoesp<br>
WS2812FX: https://github.com/kitesurfer1404/WS2812FX<br>

## How to use
1. Create a `credentials.h` with your WIFI_SSID & WIFI_PASS<br>
```cpp
#define WIFI_SSID "EnterYourSSID"
#define WIFI_PASS "EnterYourPASS"
```
2. Update the `LED_COUNT` & `LED_PIN` variables.
3. Compile and run on your NodeMCU