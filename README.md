# ESP8266 Blyss light-switch

This is an Arduino Sketch for ESP8266 Wifi module to control a light power switch [Blyss&#174;](http://www.castorama.fr/images/products/i/i_664294.jpg) using RF433MHz signal.

ESP8266 receives the commands from MQTT message events and transmit them via RF433MHz TX

**Schema:**
![schema](https://cloud.githubusercontent.com/assets/1721344/21017306/34c2b7f6-bd69-11e6-8165-4ecc0e22d117.png)

# Setup the Blyss RF Key 

Thanks to the [blyss hack project](https://github.com/skywodd/arduino_blyss_hack) to sniff my RF Key ID.

Use the [blyss sniffer](https://github.com/skywodd/arduino_blyss_hack/tree/master/Blyss_arduino_code/RF_Blyss_Sniffer) to retreived the Key then update the code with them:
```javascript
  if ( ((String)topic).indexOf("salon") != -1) {
    // update RF KEY
    RF_KEY[0] = 0x73;
    RF_KEY[1] = 0x61;
    RF_KEY[2] = 0x68;
```

# Uploading Sketch in ESP8266

TODO

# MQTT

TODO
