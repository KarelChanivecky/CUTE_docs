---
id: fridge
title: Fridge Diagram
---

## Introduction

This panel provides information on the current state of the fridge. Different pressures around the system are indicated by labelled text boxes with the name of the gauge (eg. P1 or K3) and it's reading. The numbered circles correspond to the pneumatic valves; a green outline indicates that the valve is open, while a red outline indicates the valve is closed. The pumps/compressors used for the vacuum and circulation are shown as circles around an abbreviation of the respective piece of equipment; an outline of green corresponds to the pump running, while an outline of red corresponds to the device being off. The abbreviations are: 
- TD - primary turbo pump 
- PPD - primary scroll pump 
- Comp - circulation compressor 
- TAux - vacuum turbo pump 
- PPAux - vacuum scroll pump 

When the fridge is running the helium circulates clock-wise, going into the fridge through the left side and out from the turbo pump (TD) down through the scroll pump (PPD).

## Comments
It should be noted that the status of the primary scroll pump (PPD) does not get properly saved in the data stream, as a result it can appear that the circulation is running while the scroll pump is off, but in reality it is just an artifact. 
