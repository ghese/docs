# DVL-A50

## Description
The DVL A50 is – by far – the world’s smallest commercially available Doppler Velocity Log.

The A50 is establishing a new market standard with its high performance, ultra-small 4 beam setup, open interface protocol and low cost.

The DVL estimates velocity relative to the sea bottom by sending acoustic waves from the four angled transducers and then measure the frequency shift (doppler effect) from the received echo. By combining the measurements of all four transducers and the time between each acoustic pulse, it is possible to very accurately estimate the speed and direction of movement.

## Key specifications

* 0.05 - 50 meter range
* 1 MHz transducer frequency
* 4-10 Hz ping rate (altitude dependent)
* 2 m/s max velocity
* ± 0.1 cm/s long term accuracy
* 1000 meter depth rating
* 10-30 V input voltage (reversed-polarity protection)
* Ethernet and UART

!!! note
    We are using a constant speed of sound equal to 1500 m/s (Release 1.3.1). This will be user configurable in comming releases.

## LED Signals

* No green light: Power is off.

* Flashing green light (slow): DVL loocking for bottom lock.

* Fixed green light: DVL has bottom lock. The LED is mostly on and blinks quickly to show we are alive.

## Wiring interface

The tables below shows the pinning of the DVL-A50 interface.

| Interface           | Color |
| :------------------ | :-- |
| Positive (10-30V) | Red  |
| Negative/Ground | Black   |
| ETH TX+ | Orange/White   |
| ETH TX- | Orange   |
| ETH RX+ | Green/White  |
| ETH RX- | Green  |
| UART TX | Brown/White   |
| UART RX | Brown  |

## Terminal Interface

The DVL-A50 has a 3.3 volt UART interface (5V tolerant).

| Settings           | Value |
| :------------------ | :-- |
| Baud rate | 115200  |
| Data parity stop | 8N1   |
| Flow control | None  |


Description of the [serial protocol](./dvl-protocol.md).

## Ethernet Interface

Description of the [ethernet services](./dvl-a50-details.md#ethernet-interface).

<!--
## Libraries and code examples

Example code and libraries that can be used to communicate with the DVL on the terminal interface:

* [Python](https://github.com/waterlinked/dvl-python)
 -->


## Dimensions

![dvl_a50_dimensions](../img/dvl_dimensions.png)


## Mounting Holes

![dvl_a50_mounting_holes_drawing](../img/dvl_mounting_holes_drawing.png)


## Other details

See [details](./dvl-a50-details.md) for description of axis conventions, transducer numbering and other details.

## Datasheet

[Datasheet](https://www.waterlinked.com/datasheets/dvl-a50/)
