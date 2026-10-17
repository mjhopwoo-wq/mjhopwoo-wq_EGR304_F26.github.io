---
title: Component Selection
---


**Voltage Regulators**

1. L805CV Linear Regulator

    <img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/b098f6f3-2e5f-4a80-8b03-07eaab7534ac" />

    * $1/each
    * [link to product](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805CV/585964)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Cheap and available | Bad efficiency roughly 40% loss |
    | Up to 35V of input voltage | Voltage tolerance not as good as other l7805 unit |


2. L7805ABV Linear Regulator

    <img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/8a140cb3-49d0-4821-b753-1651555b1eaa" />

    * $1/each
    * [link to product](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805ABV/634711)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Cheap and available | Bad efficiency roughly 40% loss |
    | Tighter tolerances on voltage output compared to the other L7805 | Ever so slightly more expensive than the others |

3. MC7805CTG Linear Regulator

    <img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/1327da7f-7f1b-45c7-bd78-c1153015c7f8" />

    * $1/each
    * [link to product](https://www.digikey.com/en/products/detail/onsemi/MC7805CTG/919333)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Cheap and available | Bad efficiency roughly 40% loss |
    | Easy to model package and standard pin configuration for a breadboard | Lower current output compared to the others at 1A |

**Choice:** Option 2: L805CV Linear Regulator

**Rationale:** While its slightly more expensive than the others its basically negligible in regards to overall budget and its just a bit better than the others so its a worth it tradeoff.

**H-Bridges**

1. Texas Instruments SN754410NE

    <img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/cd4f77e3-ea23-4e1e-92f0-4cba1f27b16a" />

    * $4.40/each
    * [link to product](https://www.digikey.com/en/products/detail/texas-instruments/SN754410NE/380180)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Standard 16-DIP package for easy hand soldering or IC socket mounting. | Bipolar transistor design creates ~1.2V–1.8V internal voltage drop, reducing voltage to the motor. |
    | Features built-in output ESD protection diodes. | Max 1A continuous output current per channel. |


2. STMicroelectronics L298N

    <img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/3c015a6a-3b48-4b23-b819-f798630d702c" />

    * $13.60/each
    * [link to product](https://www.digikey.com/en/products/detail/stmicroelectronics/L298N/585918)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | High output current capacity (up to 2A continuous per channel). | Large physical package with non-standard pin staggered row spacing. |
    | Accepts wide motor supply voltage ranges (up to 46V) | High voltage drop requires external flyback diodes on custom PCBs. |

3. Texas Instruments L293D

    <img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/5794417a-7fcb-441f-b25a-b90bccdb2e24" />

    * $10.60/each
    * [link to product](https://www.digikey.com/en/products/detail/stmicroelectronics/L293D/634700)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Industry standard, extremely easy to find and drive with logic levels. | Lower current handling capacity (600mA continuous per channel). |
    | Built-in internal clamp diodes protect against inductive kickback. | High internal saturation voltage loss under heavy motor loads. |

**Choice:** Option 1: Texas Instruments SN754410NE

**Rationale:** It is the most cost efficient option on top of checking all the necessary boxes and allowing for easy and effective design through its standard dip package. 

**Vibration Motors**

1. Vybronics VC1030B028F

    <img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/1bf6476e-a40a-48a8-b20a-ce7b2be0e5aa" />

    * $2.94/each
    * [link to product](https://www.digikey.com/en/products/detail/vybronics-inc/VC1030B028F/7732327?s=N4IgTCBcDaIGoGECMAGAzCgQisAOAYiALoC%2BQA)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Smallest footprint size compared to the others | Weakest haptics of the bunch at 0.9G which may be too little |
    | Draws only ~64–80mA typical current | Fixed single axis motion meaning vibration is restricted strictly perpendicular to the mounting plane. |


2. Vybronics VC1234B016F

    <img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/4d92e750-e272-40ae-b8ab-007265dd7e72" />

    * $3.23/each
    * [link to product](https://www.digikey.com/en/products/detail/vybronics-inc/VC1234B016F/9974297?s=N4IgTCBcDaIGoGECMYDMAWAQgBiQNgDEQBdAXyA)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Stronger haptics than the first option at 2G | Larger footprint compared to the first one |
    | Deeper Vibration because it operates at a lower frequency | Takes slightly longer to spin up to speed and stop due to its heavier internal rotating mass. |

3. Vybronics VZ7AL2B1692082

    <img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/09d3d1f8-a262-4387-98a9-7a7effa027c1" />

    * $4.04/each
    * [link to product](https://www.digikey.com/en/products/detail/vybronics-inc/VZ7AL2B1692082/6009928)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Significantly stronger than both options at 5.1G | Cylindrical shape requires special housing/mounting compared to sticking it on part of the chasis |
    | Everything is fully enclosed so no need to worry about physical interference | Largest by volume, while it is thinner it is taller |

**Choice:** Option 3: Vybronics VZ7AL2B1692082

**Rationale:** They are are fairly similar in price and with that being taken into consideration the significantly improved haptics on option 3 make it the best fit. While the drawbacks in terms of size may require more design considerations the tradeoff of better haptics is well worth it.
