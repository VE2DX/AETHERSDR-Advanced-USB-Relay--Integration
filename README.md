# AETHERSDR-Advanced-USB-Relay-Integration

# Version

00.01.00 May 21 2026 by Richard VE2DX

# Introduction

Proposed changes in AETHERSDR of USB Relay integration for a more advanced integration offering more flexibility and better SO2R integration.

# 1- The Author

Richard G. Desaulniers Sr., VE2DX, was the Owner, President, and Lead designer at VE2DX Electronics Design Inc.
A Canadian-based Ham Radio Electronics company founded in 2020 and closed in late 2025 following worldwide economic instability.

This project will be submitted to the AETHERSDR team as a possible evolution of the USB relay interfacing.

# 2- Context

While the FlexRadio integration offers a great, low-cost, simple interface, the USB-based relay integration is lacking some badly needed improvements. Among those;

- The possibility to assign multiple bands or frequency ranges to a single relay output to address multiband antennas like a common 80/40 dipole or the very common tribander yagy.

- A better SO2R integration.

- Adding the CH340/341 chip sets to the Flexradio Radio OS, to be able to support, at the radio end, more advanced hardware like the WinKeyer

- and Software Defined Interlock(c) (SDI(c)) to prevent two radios from transmitting or receiving on the same antenna or band.

# 3- Technical Information.

# 3.1- FlexRadio present approach.

<img width="1146" height="798" alt="image" src="https://github.com/user-attachments/assets/2f2c3f9d-eaeb-423b-bdd3-3299f9379149" />

The present approach by FlexRadio in the latest version as of this document publishing, is flawed in couple different ways. It does not address the specific requirements of SO2R, It lacks flexibility, it does not address the specific requirements for multiband antennas, etc...

3.1.1- The source is always output oriented, this is ok and gives the user some flexibility, but in SO2R you need to be able to manage a group of output, thus offering an SO2R mode in the top of this window, with added Source pull down in that same upper area and SO2R mode again in that same area would address this concern (item 1 in the image).

3.1.2- The band select or frequency range selection is limited to ONE item, these should be replace by a pull down where, in the band mode would list all the possible bands, and in frequency range mode 

