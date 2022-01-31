---
title: "A - Proof of Concept"
date: 2022-01-16T09:40:39+03:00
draft: false
---

To validate the proposed solution with the limited budget constraint, it was decided to use a 3D printer to replication a Farmbot. The 3D printer was modified to have a webcam attached to it to be used as the weed scanning tool, and the laser to be used in the finalized Farmbot was also attached to the 3D printer to be a part of the prototype.

![](/images/Proof1.png)



The figure above shows the exact model used in the fabrication of the prototype and the choice of a 3D printer was obvious as it has a 3 axis gantry system
which is exactly what Farmbot uses but this has a much smaller
form factor and is widely available and more affordable. The
reasons behind why this exact model was chosen are due to its low price and the fact that it has an open-source microcontroller and software that allowed the team to fully control the 3D printer through a serial connection with a USB cable. Since this is not a growing area and having weeds will cause a mess the weed was replaced with a red circle and a red whiteboard magnet such as the one presented in the figure below was used
![](/images/Proof2.png)



### Assembly
As mentioned previously the 3D printer had a camera and a laser module attached to it. A custom-designed mounting bracket was designed specifically for this application and then it was printed using the 3D printer.

![](/images/Proof3.png)

The custom-designed mount is shown in the figure above. The mount allowed for a seamless mounting arrangement that did not impair nor interfere with the 3D printing functionality.

![](/images/Proof4.png)

The figure above shows the completed assembly of the prototype used for the purpose of the validation process.

### Computer Program

To control the assembly a computer program was developed to drive the mechanisms a satisfy the required physical objective, which is to the red magnet representing a weed and pinpoint its exact location and then triggers the laser and moves the laser around the red magnet to make sure that if it was a weed that it is most likely to be burnt. For the purpose of this project, MATLAB was since it was the programming tool with which the team members are familiar using.

![](/images/Proof5.png)

The logic for the computer program used to control the system is presented in the diagram in the figure above. When the device is first turned on it will calibrate its location and then go to the idle home location waiting for a command to search for weeds. The search for weeds command can be triggered either by a specific event such as time i.e. 7:00 am every Sunday or manually. After the scan command is triggered the computer software will drive the motors to move the camera to multiple locations to take a snapshot of the bed which in this case represents the growing area, then the previously taken images are stitched together to make the full image of the bed as shown below

![](/images/Proof6.png)

The figure above shows the images taken at a different location and then the stitched version. After stitching the images, the final stitched image is then referenced to real-life coordinates of the bed. After having a way to convert pixel location to mm location on the bed of the 3D printer, the image is analyzed and a mask is applied where anything that is red in the image is then turned into white with everything else being black as shown in the figure below.


![](/images/Proof7.png)

In the figure above it shows the masked red regions with boxes around them. The reason for the boxes is to be able to get the XY pixel location for the red magnets and to eliminate the noise in the image by only considering the boxes that meet certain criteria (in this case the area of the box) and reject all other boxes. The information of all confirmed boxes is then stored in a matrix format. After location each red magnet the 3D printer is then instructed to take the camera to the location of the first red dot in the matrix of red dots (order is not important in this case), the reason the camera is first taken to the red magnet before the laser is to pinpoint the exact location of the red magnet with a certain accuracy which reduces any errors from the previous location estimation process in a dramatic manner.
The figure above shows the location of the red magnet before the enhancement and after and as it can be concluded that a great deal of correction has taken place. After doing so the distance from the head of the laser and the camera lens is known (in this case it is 48mm in the X and 23 mm in the Y). The printer will bring the lens of the laser to the center of the red magnet and then trigger the laser.
In the figure the pattern of which the laser will burn the weed is shown, the reason this pattern (The Archimedean Spiral) was chosen was that the magnet was circular and it was fairly simple to manipulate without causing any damage to the bed of the 3D printer, another pattern is used when a weed is to be eliminated)

![](/images/Proof8.png)


#### Pseudo-code
After describing what happens in each operation of the code the pseudo-code is presented for each function below (Taking into consideration)

##### Initiation
##### Scanning the area
##### Detecting Red Dots
##### Honing In On Red Dots
##### Eliminating The Red Dot

### Testing and Results
In the figure below the red magnets used are shown before and after the burning process using the laser

![](/images/Proof9.png)

As it can be seen that the laser was capable of melting the plastic cover of the white board magnet indicating that it will be powerful enough to burn organic leafs which will also be demonstrated in the following section of the report. The pattern used for attack (Archamedian spiral) can also be seen in the second burnt magnet on the right hand side.

### Proof of concept - weed elimination

In this section the results for burning an actual weed are shown. In the first figure below a small plant demonstrating a weed (in size) is used in a small, a perfectly healthy small plant.
![](/images/Proof10.png)

The plant in the figure above will go throught the burning process and the results are shown below in the next figure.

![](/images/Proof11.png)