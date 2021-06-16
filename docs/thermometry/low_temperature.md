---
id: LT_thermo
title: Low Temperature Thermometers
---

## Introduction

The low temperature thermometers provide information about the coldest three stages of the fridge, the mixing chamber, cold plate, and still. Of the low temperature thermometers the mixing chamber and cold plate thermometers are ruthenium-oxide thermometers and the still thermometer is a Cernox. This means that the still thermometer is capable of providing relatively accurate readings over the full range of fridge temperatures (from room to base temperature). Conversely, the mixing
chamber and cold plate thermometers are only accurate at temperatures less than roughly 20K.

On the thermometer webpage the first row is the mixing chamber thermometer, the second row is the cold plate thermometer, and the third row is the still thermometer.

## Instructions
### Start of cooldown
At the start of the cooldown only the still thermometer is required, the other thermometers can be setup but their readings will not be meaningful. To setup the thermometers at the beginning of the cooldown use the parameters in the table below.

| Thermometer | MODE | I MODE | I RANGE | 
| ---------- | ---------- | ---------- | ---------- | 
| Mixing chamber | FIX CURRENT | AUTO RANGE  | N/A | 
| Cold plate | FIX VOLTAGE | AUTO RANGE  | N/A | 
| Still | FIX VOLTAGE | AUTO RANGE  | N/A | 

### Start of condensation
Once the fridge reaches low enough temperatures the mixing chamber and cold plate RuOx thermometers will be required. The settings in the table below should be appropriate for this time.

| Thermometer | MODE | I MODE | I RANGE | 
| ---------- | ---------- | ---------- | ---------- | 
| Mixing chamber | FIX CURRENT | FIX RANGE  | 10pA-100nA | 
| Cold plate | FIX VOLTAGE | AUTO RANGE  | N/A | 
| Still | FIX VOLTAGE | AUTO RANGE  | 3nA-30uA | 

*NOTE: When using the FIX RANGE current mode in order to set the current in the thermometer you will need to type a value in the appropriate current range in the box labelled I and then press return.*
