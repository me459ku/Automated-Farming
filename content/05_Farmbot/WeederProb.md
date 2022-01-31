---
title: "C - Weeder Problem"
date: 2022-01-16T09:40:39+03:00
draft: false
---


As previously stated, the device employs a rotary tool equipped with a 24 [v] DC motor to kill weeds, which may result in undesirable vibration throughout the system. After repeated use, the rotary blades may become damaged, resulting in blade imbalance. Unbalanced blades will generate a series of vibrations that will travel from the motor to the gantry. Vibrations will affect both the tool and the universal mount, dislocating them and potentially affecting their alignment and accuracy. The figure below shows the parts which might be affected by the vibrations.

![](/images/Prob1.png)

The cross-slide might be affected by the vibrations by loosening up the belt shown in the figure below and leading to an unstable movement along the gantry.

![](/images/Prob2.png)


Besides the vibration problem, there are additional issues such as the weeder's power consumption and weeder limitation. Due to the length of the blades, the weeder can only target large weeds and cannot eliminate small weeds. Additionally, because it is imprecise, it may cause damage to nearby plants. After stating all of these issues, it's evident that the primary improvement to Farmbot would be to implement a different method of weeding. An email was sent to the Farmbot company to discuss feasible product improvements (can be found in the Appendix)


#### Initial Solution Approach
Since the Farmbot already has a UTM (universal tool mount) system then and the weed wacker is not fixed to the actual device then it can easily be swapped with a powerful laser module that has a UTM end on to it that can easily be operated by the same current software on the Farmbot with minor code adjustments. The following figures will show the initial design components and the general idea around the laser module to be added to the system which will be extensively discussed in the final Phase 3 version of the report.

![](/images/Prob3.png)