---
title: Power Budget
---

## Overview

The goal of the power budget is to get an idea of how much current will be flowing through all the devices in the subsystem. But also more importantly to confirm whether or not the component configuration will work properly and not over strain the voltage regulator. This was a concern as there is only one used voltage rail on the board which is 5V. That rail will power logic for the Nano and H-bridge while also powering the motor while other passive components take up power too. To be extra safe there is also a requirement for at least a 25% current safety margin on top of the base current usage. 

<img width="878" height="688" alt="image" src="https://github.com/user-attachments/assets/4fb8d306-3363-498b-a367-978034699d81" />

## Conclusions

Using the calculations from the power budget we only use 110mA worth of current including the 25% extra safety margin. This is well within the output limit of the 5V regulator which can output 1A max. 

## Resouces

The power budget as a PDF download is available [*here*](https://github.com/user-attachments/files/34202373/PowerBudget.pdf), and a Microsoft Excel Sheet [*here*](https://github.com/user-attachments/files/34202386/PowerBudget.xlsx).
