# Thermostat ideas

Thinking a bit along the Nest(TM) line:

* Simple on-board UI with e-ink display and a knob
* Remote access via web browser to change the schedule, etc
* Powered by a USB charger
* Battery backup when AC power missing (low-power mode keeps schedule and on-board UI alive but no remote access)
* No cloud services, registration or black boxes with Chinese firmware

Hardware?

* ATMega family
* Separate WiFi module which can be completely powered down
* Remote sensors using NRF24L01+ on Arduino:
   * [NRF24L01P spec](https://www.sparkfun.com/datasheets/Wireless/Nordic/nRF24L01P_Product_Specification_1_0.pdf)
   * [tutorial](https://lastminuteengineers.com/nrf24l01-arduino-wireless-communication)
   * [enchanced library](https://nrf24.github.io/RF24/) but for Arduino only
   * [simple library](https://github.com/kehribar/nrf24L01_plus) for AVR.  This looks promising.

For stand-alone hardware, the Multi-Tens project is a possible starting point.  Fits in a nice bud box.  ([wiki](http://ohm.bu.edu/trac/edf/wiki/MultiTEMS))

