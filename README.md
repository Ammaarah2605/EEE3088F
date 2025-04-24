# EEE3088F
**OVERVIEW**

This project involves designing a Power Subsystem PCB for the MM (Micromouse) as a group. Each team member is responsible for specific sections of the design, while the demonstration and final PCB are assessed collectively. The project is a continuation of the previous breadboard assignment, now transitioning to a custom PCB solution.
The final design must meet a series of electrical and physical requirements to support motor control, battery management, voltage regulation, and interfacing with the MM’s motherboard.

**Power subsystem requirements**
- Operate up to 4 bidirectional motors using available pins:
    - 2x brushed DC motors @ 200mA (max) on 1S1P battery voltage.
    - 2x auxiliary motors @ 500mA each.
- Include and configure an INA219 on the I2C bus for battery monitoring.
- Charge the battery from a 9V input pin with two current modes:
    - 200mA (low), ~600mA ±100mA (high).
- Integrate USB-C input to provide 9V via USB Host.
- Implement 2x External Load Switches at 1A each (high-side, 5V).
- Regulate:
    3.3V output (±5%, 300mA max)
    5V output (±5%, 1.5A max)
- Include a power ON/OFF switch:
    - OFF: < 30µA battery draw
    - ON: Support robot peak current of 2A
    - Must shut down both 3.3V and 5V rails.

**Team Members & Responsibilities**

Nuha: 
- Control **4 bidirectional motors** (2x 200mA brushed DC motors, 2x 500mA auxiliary motors) using available pins.  
- Integrate and correctly configure an **INA219** sensor on the **I2C bus** for battery monitoring.  
- Provide **2x high-side external load switches**, each capable of **1A at 5V**.  
- Provide regulated outputs: **3.3V ±5% (300mA max)** and **5V ±5% (1.5A max)**.

Ammaarah:
- **Charge the battery** via the **9V input pin**.  
- Support **two battery charging modes**: **200mA (low)** and **~600mA ±100mA (high)**.  
- **Integrate USB-C** to deliver **9V from the USB Host**.  
- Include an **ON/OFF switch**:  
  - **OFF state**: battery draw < 30µA  
  - **ON state**: supply up to **2A peak current** and shut down both **5V and 3.3V rails**.

**Tools used**
- KiCad
- JLCPCB parts library
