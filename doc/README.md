### At middle point (see photo) can connect +12V/2A for power MCU and main board equipments. ###

## BOARD AB86653 (MCU) ##

MCU program socket

[1] GND

[2] MCU VCC (+5V)

[3] RxD (pin 13 MCU, P3.0/RxD)

[4] TxD (pin 14 MCU, P3.1/TxD)

## MAIN BOARD ##

[1] GND

[2] MCU VCC (+5V)

[relay pin]

[1] Pin 31 MCU (PWM7_3/ADC10/P0.2). Positive pulse 100ms will switch relay OFF

[relay pin]

[1] Pin 32 MCU (PWM8_3/ADC11/P0.3). Positive pulse 100ms will switch relay ON

[2] Pin 1 MCU (PWM1P/ADC0/P1.0/Tx1) Passed to wireless board CB3S pin 3 (P11/D11/TX1) by step-down (5V=>3V3) level converter.

[3] Pin 2 MCU (PWN1N/ADC1/P1.1/Rx1) Passed to wireless board CB3S pin 4 (P10/D10/RX1) by step-up (5V<=3V3) level converter.

[4] Pin 3 MCU (T2/PWM2P/ADC2/P1.2) Analog input, about +1.465V on 230V AC (not used?)

[5] Pin 7 MCU (PWM4P/ADC6/P1.6/RxD3) Input data from HLW8032 (4800BPS, 8E1)

[6] Pin 8 MCU (PWM5_2/PWM4N/ADC7/TxD3) Output data to HLW8032 (reserved?)


## ATML143 ###

A0, A1, A2 - GND

VCC - MCU VCC

SDA - pin 25 MCU (P2.4/MISO_2/I2C_SDA2)

SCL - pin 26 MCU (P2.5/SCLK_2/I2C_SCL2)

WP - GND


## Keyboard & LED ##

Pin 24 MCU (P2.3) - common for all LED cathode

Pin 29 MCU (P0.0) - PULSE LED (green)

Pin 23 MCU (P2.2) - WiFi LED (red), SET button from anode LED and GND

Pin 22 MCU (P2.1) - V LED (red), UP button from anode LED and GND

Pin 21 MCU (P2.0) - A LED (red), DOWN button from anode LED and GND

Pin 30 MCU (P0.1) - L LED (red), ON/OFF button from anode LED and GND
