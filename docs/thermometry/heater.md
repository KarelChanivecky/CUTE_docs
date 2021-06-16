---
id: heater
title: Heaters
---

## Introduction

There are three heaters inside the cryostat at the mixing chamber, cold plate, and still stages respectively. The heaters can be used to change the internal temperatures of the cryostat for different studies. Each heater is controlled by the respective row on the webpage, the first row is the mixing chamber heater, the second row is the still heater, and the third row is the cold plate heater.

## Instructions

There are two ways to use the heaters through the webpage. The most basic mode of operation is to specify the desired power of the heater, the other mode of operation is to specify the desired setpoint temperature and allow the heaters to regulate through PID control. The following sections will describe both modes of operation.

### Fixed power mode
Before using the fixed power mode, the PID settings must all be set to 0 (ie. P=I=D=0). There should now be a text box labelled "SET POWER", insert your desired power in this box (in units of Watts) and then select the "ON" option from the drop-down menu in the corresponding row. Once the output has been enabled you should see the actual current/power in the appropriate heater track at the bottom.

*NOTE: Sometimes the fixed power mode does not turn on properly, in this case you must access the main heater control on the Fridge PC.*

### Set temperature mode
Before using the set temperature mode you must ensure that the heater channels are pointed to the correct thermometry (otherwise you may excessively heat the wrong thermal stage). In the "NAME" field of each row put "MMR3_01_2_149", this will use the low temperature thermometers which are typically more accurate than the high temperature thermometers. Then in the "CH" field next to the "NAME" field put in 0 for the first row (mixing chamber), 2 for the second row (still), and 1
for the third row (cold plate).

After ensuring that each heater is using the correct thermometer, you must set the PID settings. Typical settings for each channel are given in the table below.

| Channel | P (W/K) | I (S^-1) | D (S) | 
| ---------- | ---------- | ---------- | ---------- | 
| Mixing chamber | 1 | 4 | 0 | 
| Cold plate | 2 | 4 | 8 | 
| Still | 3 | 6 | 9 | 

After changing the PID settings you can choose your desired temperature setpoint by typing it in the "SET POINT" input box (in units of Kelvin). To start the automated control select the "ON" option from the drop-down menu next to "PID #" where "#" is the desired heater track.

*NOTE: Sometimes the power output by the heaters can be too small for a particular application. If you enabled the heater output and expect a larger change in the temperature try changing the "Pmax" value to a larger number. The typical value for the mixing chamber is about 0.5W; the maximum value it can accept is 1W.*
