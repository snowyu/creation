# Creation [![Join the chat at https://gitter.im/teamhost/creation](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/teamhost/creation?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

中文版本: [在这里](README.cn.md)

We talk about a variety of creation/innovation and analysis here.

Contribution are welcome. Please read [CONTRIBUTING.md][contributing] before contributing.

* Services
  * [sandstorm](https://sandstorm.io) - Sandstorm lets you run your own server and install apps like EtherCalc, GitLab, Etherpad, Wekan, and more as easily as you'd install apps on your phone.
  * [Slack](service/slack.md) - the analysis of [slack][slack]'s creation.
  * [Github](https://github.com) - While this is not something new, but it represents a turning point, and now it's ecosystem has been improved, competitions abundant , fully open source solutions already exist.
  * [Code Climate](service/codeclimate.md) - Code style quality and code coverage display services.
    * [Code Climate Web Site][codeclimate]
    * Support the badges:
      * Code Quality Rating: [![Code Climate](https://codeclimate.com/github/snowyu/property-manager.js/badges/gpa.svg)](https://codeclimate.com/github/snowyu/property-manager.js)
      * Code Test Coverage:[![Test Coverage](https://codeclimate.com/github/snowyu/property-manager.js/badges/coverage.svg)](https://codeclimate.com/github/snowyu/property-manager.js/coverage)
    * Similar Services:
      * [Coveralls](https://coveralls.io/) - code coverage display only.
        * I've used once in the past, but it display no data now after upload lcov.info, use Code Climate instead.
  * [WYSIWYG Form Builder]():
    * Formstack
    * TypeForm
    * JotForm
    * Wufoo
    * [screendoor](http://www.dobt.co/screendoor/): Smarter online forms
  * [bip.io - Web Automation For People and Robots](https://bip.io/):Open Source, Rapidly create workflows with the cloud components you love, no programming required.
  * [IFTTT](https://ifttt.com/)
  * [OpenBazaar](https://openbazaar.org/): OpenBazaar is an open source project to create a decentralized network for commerce online, using Bitcoin, that has no fees and cannot be censored.
  * [Gratipay - Gittip](https://gratipay.com): The First [Open Company][OpenCompany], give money every week to people and teams you believe in. The mission is to cultivate an economy of gratitude, generosity, and love.
* [Open Source Hardware](https://en.wikipedia.org/wiki/Open-source_hardware)
  * Building Blocks:
    * MakeBlock - http://www.makeblock.cc/
  * Main Board:
    * Arduino - https://www.arduino.cc/ - Sensor Controller
      * Microduino - https://www.microduino.cc/
      * Netduino - http://www.netduino.com/netduino - an open-source electronics platform using the .NET Micro Framework.
      *
    * Raspberry Pi - https://www.raspberrypi.org/ - HDMI box
      * CubieBoard - http://cubieboard.org/
    * [NL6621 ARM Wifi Soc](http://www.nufrontsoft.com/index.php/project/index/id/30.html)
      * 160 MHz ARM Cortex-M3 with 448 KB of RAM. The module has 32 GPIOs, SPI, I2C, I2S digital audio.
      * 802.11 b/g/n/p/e
      * https://github.com/NufrontIOT/NL6621_StandardSDK
      * https://www.gitbook.com/@nufrontiot :Chinese Books
    * ESP 8266 Wifi SoC
      * [NodeMCU](http://www.nodemcu.com/): An open-source firmware and development kit that helps you to prototype your IOT product within a few Lua script lines
        * NodeMCU 0.9 ESP-12 Module
        * NodeMCU 1.0 ESP-12E Module
      * [Arduino UNO R3 ESP8266 WiFi shiled(ESP-12E)](https://item.taobao.com/item.htm?id=521217451908)
    * WRTnode - http://wrtnode.com/ - Wifi Router
      * Vocore - http://vocore.io/
    * HackRF - https://github.com/mossmann/hackrf - Software defined Radio(SDR)
      * GSM
      * Bluetooth
      * Wifi
    * OpenPilot - https://www.openpilot.org/ - Flight-controller
      * ArduPilot - http://ardupilot.com/
      * Blog - http://www.rchacker.com/
      * KK2 - https://code.google.com/p/nextcopterplus/wiki/OpenAero2_Getting_Started
      * MultiWii(MWC) - http://www.multiwii.com/
        * NanoWii - http://www.nanowii.com/
  * Robot
    * Simplebot - https://github.com/nodebotsau/simplebot
  * Software
    * IoT Platform
      * AllSeen - https://allseenalliance.org/
      * OCF - http://openconnectivity.org/
        * The next [OpenInterconnect](http://openinterconnect.org/)
      * IoT.js - http://github.com/Samsung/iotjs
        IoT.js aims to provide inter-operable service platform in the world of IoT, based on web technology
      * [OpenHAB](http://www.openhab.org/) - is a software for integrating different home automation systems and technologies into one single solution that allows over-arching automation rules and that offers uniform user interfaces (Java).
        * [A web admin console for openHAB home automation](https://github.com/cdjackson/HABmin)
        * http://www.instructables.com/id/Uber-Home-Automation-w-Arduino-Pi/
        * https://github.com/openhab/openhab/wiki/Souliss-Arduino-based-SmartHome-Binding
      * [Souliss](http://souliss.net/) - The open-source SmartHome framework to empower your Arduino and Android devices
    * firmware
      * Javascript
        * JerryScript - https://github.com/Samsung/jerryscript
          JerryScript is the lightweight JavaScript engine intended to run on a very constrained devices
          * Only few kilobytes of RAM available to the engine (<64 KB RAM)
          * Constrained ROM space for the code of the engine (<200 KB ROM)
        * [duktape](https://github.com/svaarala/duktape): run on platforms with 256kB flash and 96kB system RAM.
        * [cesanta's v7](https://github.com/cesanta/v7): Compiled core is in 40 KB - 200 KB range.
          * [smart.js](https://github.com/cesanta/smart.js)
          * [Wifi ESP8266](http://espressif.com/en/products/esp8266/)
        * [Espruino](https://github.com/espruino/Espruino): 128kB Flash and 8kB RAM.
      * Forth - My Favorite MicroController Language
        * FlashForth - http://flashforth.com/ - https://github.com/oh2aun/flashforth.git
        * AmForth - http://amforth.sourceforge.net/
        * avrforth - http://krue.net/avrforth/
      * Microsoft .NET Micro Framework - https://netmf.github.io/
        * at least 256 KBytes of flash and 64 KBytes of RAM. A memory footprint of about 300 KB
        * Can run directly "on the metal" without an operating system
        * Running on an OS is also possible
        * ARM architecture processors (including ARM7, ARM9 and Cortex-M architectures)
        * Analog Devices Blackfin
      * OpenWRT -
    * protocol
      * MQTT - MQTT is a publish/subscribe messaging protocol designed for lightweight M2M communications. via IBM
        * http://mqtt.org/
        * [Specification](http://www.ibm.com/developerworks/webservices/library/ws-mqtt/index.html)
        * https://github.com/adamvr/MQTT.js/
      * CoAP - Constrained Application Protocol from the CoRE (Constrained Resource Environments) IETF group.
        * http://coap.technology/
        * Like HTTP, CoAP is a document transfer protocol. Unlike HTTP, CoAP is designed for the needs of constrained devices.
        * CoAP runs over UDP
        * [IP for Smart Objects Alliance](http://www.ipso-alliance.org/)
        * [Specification](http://tools.ietf.org/html/draft-ietf-core-coap)
        * Open source implementations:
          * http://sourceforge.net/projects/libcoap/
          * https://github.com/morkai/h5.coap
          * http://www.contiki-os.org/
      * Firmata - http://www.firmata.org/wiki/Main_Page
      * CAN -
    * IDE
      * processing with Firmata
      * node-red - https://github.com/node-red/node-red
      * scratch
      * snap

* Programming
  * Asynchronous, Stream and Architecture
    * [ReactiveX.io](http://ReactiveX.io)
      * [cycle.js](http://cycle.js.org): (human <--> computer)
      * [Kefir.js](https://github.com/rpominov/kefir): is a Reactive Programming library for JavaScript inspired by [Bacon.js][bacon.js] and [RxJS][rxjs], with focus on high performance and low memory usage.
    * [Gulp 4](https://github.com/gulpjs/gulp/tree/4.0) Keep It Simple and Stupid(KISS)
  * Stupid compiler and smart compiler



## License

[![CC BY 4.0](https://i.creativecommons.org/l/by/4.0/88x31.png)][CCBY4]

This work is licensed under a [Creative Commons Attribution 4.0 International License][CCBY4].


[slack]: https://slack.com/
[bacon.js]: https://github.com/baconjs/bacon.js
[rxjs]: http://reactive-extensions.github.io/RxJS/
[codeclimate]:https://codeclimate.com
[contributing]: https://github.com/teamhost/creation/blob/master/CONTRIBUTING.md
[OpenCompany]: http://www.opencompany.org
[CCBY4]: https://creativecommons.org/licenses/by/4.0/
