# ESP32-S3-BOX firmware with different wakeword models

The current [ESP32-BOX firmware version 0.2.1](https://github.com/espressif/esp-box) uses the __Hi ESP__ wakeword that has a poor response. See this [issue](https://github.com/espressif/esp-box/issues/9).

The firmwares in this respository have been built using [the ESP-BOX factory demo](https://github.com/espressif/esp-box/tree/master/examples/factory_demo) but modified as follows:
* `ESP-BOX_firmware_Alexa.bin` configured with the __Alexa__ wakeword model that has a much better response.
* `ESP-BOX_firmware_fixed_HiESP.bin` incorporating the updated `hiesp8` wakeword model in an unreleased fix for the `esp-sr` component. Has a significantly improved response to the __Hi ESP__ wakeword.
*`ESP-BOX_firmware_hacked_ESP.bin` is a crudely modified version of the factory demo to use the multinet model to provide a wakeword - in this case __E S P__



