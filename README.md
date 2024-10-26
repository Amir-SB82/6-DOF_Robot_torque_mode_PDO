# torque mode

                                            +---------------+
                                            |  torque mode  |
                                            +---------------+
## Overview

**torque mode** Applying torque to the motor, if we want to apply it correctly, we must use the control loop due to position, velocity, and acceleration.   

---

## Features

- ⚡ **PDO message**: you should send torque to the drive with PDO message because torque most be sent at any moment.
- ◆ *warning* Applying torque in this way is dangerous and the motor may want infinite torque. To apply the torque correctly, a control loop must be used.
---

## Getting Started

To set up the project locally, follow these steps.

### Prerequisites
- **STM32CubeIDE**: Ensure you have [STM32CubeIDE version 1.13.0(recommended)]
- **CANopen stack**: you need this stack for your communication 
i have used this stack in the code, you can also download and including it from [github website](https://github.com/CANopenNode/CANopenNode)

### Run code
1. **open new project**: 
    go to file --> new --> STM32 project
2. **add the stack**: 
    Go to project --> properties --> paths and symbols --> includs --> add --> file systrm
    Then choose CANopenNode and core/CANopenNode_STM32
    Ensure there is CANopenNode in the source location(if this file does not exist in the source location, first apply and close and build the project, then come to the source location again.)
3. **run**:
    now, you can use this mode by upload the code to micro.

---

## License
- you can download
 *CANopenNode* document from this link(https://drive.google.com/file/d/1Lg_B5r14P_CGMcFEsO6PIyp6nOz_elqh/view?usp=drive_link)

---

## Contact
- **Email**: bestbs.1382@gmail.com
- **Github**: Amir-SB82