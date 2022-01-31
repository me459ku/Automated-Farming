+++
title = "4- Farmbot"
date = 2022-01-16T12:26:22+03:00
weight = 5
+++

## Product Architecture
Farmbot offers a wide variety of options to select from when purchasing a farmbot device there are multiple decisions to consider, in the beginning the customer should deicide on the level of automation desired in the device as farmbot offers two main version which are the Farmbot Express and the Farmbot Genesis. The Farmbot Express offers a lower level of automation, it doesnt have x axis tracks as it it runs over the raised bed meaning the customer must make sure the surface would allow for such motion and it has less computing power, for the Genesis version of the Farmbot, it offers a higher level of automation where it is more a set it and forget it for most of the time type of device, and it has greater computing power. The farmbot Express is more suitable for the customer who is willing to have daily interaction with their Farmbot. The Genesis is more suitable for scale operations as the time required to upkeep the device is lower, but on the other hand it will require more knowledge in electronics and simple mechanics as it has more components thus more points of failure. After selecting the version of farmbot that is desired, then comes the other decision of deciding the growing are for each device. Both the Genesis and the Express have regular size version with a growing dimension of (1.5m x 3m) 4.5m2 and (1.2m x 3m) 3.6m2 respectively. For the XL version the Express offers a maximum growing are of (2.4m x 6m) 14.4m2 and the Genesis Xl has a growing area of (3m x 6m) 18m2. All farmbot devices can be modified for personal projects and different use cases, it can also be inside a greenhouse with a controller for environmental variables (seperate and not part of Farmbot products).
## Details of the Farmbot product
For demonstration purposes and to meet the required customer needs the team has decided to analyze the advanced version of Farmbot, which is the newly released Genesis V1.6. (https://genesis.farm.bot/v1.6/assembly/intro) Farmbot Genesis is the most sophisticated Farmbot model which comes with the most useful features and it is flexible since most of the parts can be replaced with new parts that can be useful to accomplish new tasks and functionalities. It can grow plants, protect them, and take care of them with the highest level of precision. The tools and the functionality of the device can be modified to run experiments which helps improve the agricultural industry. Genesis has two versions depending on the size of the device. One of the versions is called Genesis which has a gantry width of 1.5 [m] and track length of 3[m]. The other version is called Genesis XL which islarger, its gantry width is 3 [m], and its track length is 6 [m]. Both of the versions have a maximum plant height of 0.5 [m] and they are shown in the figure below.

![](/images/Farmbot1.png)

There are two ways to mount the device on the planting field. The first way is to mount it on a bed. There are two types of beds which are a fixed raised bed and mobile raised bed as shown in the figure below. Genesis requires a bed size of an outer width of 1.48 [m] and the recommended outer bed length is 3 [m]. Genesis XL requires a bed size of an outer width of 2.98 [m] and the recommended outer bed length is 6 [m]. The second way is to mount on wood posts and it is called pier block supports.

![](/images/Farmbot2.png)


FarmBot Genesis V 1.6 uses two tracks to enable the gantry to move precisely along the x- axis. They are designed to be attached to a raised bed or other similar structure. Each track is made up of 1.5m-long aluminum extrusions that are connected end-to-end to create a 3m-long track for the Genesis model. By removing or adding a section of the aluminum extrusion, the tracks can be shortened or lengthened. According to the Farmbot website, assembling the tracks should take between two and twelve hours, depending on the size of the bed used. Plates are used to secure the tracks to the bed. Plates are classified into two types: track end plates and track joining plates. The track end plate is used to secure the start and end of the tracks to the bed, whereas the track joining plate is used to connect and secure the extrusions to the bed.

![](/images/Farmbot3.png)

The figure shows the 3d model of the the whole assembly of the track and plates attached to the bed.

![](/images/Farmbot4.png)

The gantry acts as the y-axis for Farmbot and made of V-slot aluminum extrusion. The gantry is attached to the tracks by gantry wheel plates. Two motors are attached to each side of the gantry to allow it to move in the x-axis, the gantry is designed in this style where it is elevated above the bed level to minimise interference with any growing plants. The estimated time required to assemble the gantry is two hours.

![](/images/Farmbot5.png)

This figure shows Farmbot's z-axis, which is used to plant seeds, water plants, eliminate weeds, and monitor soil moisture using a universal tool mount. It is able to slide on the gantry using a cross-slide which shown in the figure below.

![](/images/Farmbot6.png)

After assembling all of the parts mentioned above the completed model of the Farmbot Genesis V1.6 will look like the 3D mockup shown in the figure below.

![](/images/Farmbot7.png)

The figure above shows a picture of the 3D model of the completed device including all the parts. After connecting and assembling all the parts together, the final product should be a fully functioning device that can plant the seeds, water the plants, detect the weeds, eliminate the weeds, read the soil properties, and monitor the planting area along with the plants' health using a camera. The device uses a 3D printed mount called the universal tool mount which can be attached and connected to a tool using magnets. The universal mount shown in the figure below.


![](/images/Farmbot8.png)

In order to water the plants the device will connect the universal tool mount with the watering
tool which is the watering nozzle and it is shown in the figure below. The device has a pressure regulator to control the water output. Since it is an open source product the watering tool can be redesigned using its 3D model to change the water output.


![](/images/Farmbot9.png)
The figure above shows the water nozzle attached to the universal tool mount during the plants watering process. As shown in the figure the water stream has been defused using the water nozzle to prevent the plants from getting damaged from the concentrated water stream.

![](/images/Farmbot10.png)
The figure above shows the seed planting tool which is called the seeder or the seed injector. The tool includes a needle that can be changed by the user depending on the seed's size. The concept is to use a vacuum pump to suction and hold the seed and inject it into the ground at the selected location. The device will go back and forth picking up the seeds from a cup or an external source and to the selected locations.
![](/images/Farmbot11.png)
The two tools shown above are the tools that have been used to kill the weeds in their vulnerable stages. One of the wedding tools is called the weeder which kills the weed by smashing and pushing them into the ground which prevent the weeds from growing. The other tool is called the rotary tool which has a DC motor and two blades to cut the weeds besides its other functions such as soil surface milling and an additional function which is 5 [mm] drilling which requires a drilling chuck.
![](/images/Farmbot12.png)
The figure above shows the soil sensor tool which helps getting an accurate reading for the soil properties. It has a moisture sensor that can measure the soil moisture which gives indications and information about the amount of water in the soil. The right side of the figure shows the soil sensor during the soil moisture measuring process.
![](/images/Farmbot13.png)
The figure above shows an actual existing product. It shows the variety of crops that can be grown using the device ( such as: spinach,beets, etc.) . The used device in the figure is the Genesis XL version 1.6 which is the latest version.
Farmbot is controlled by a custom microcontroller known as farmdunio. This microcontroller communicates via G-code with a Raspbery Pi. The stepper motors, universal tool mount, and other peripherals are controlled by Farmdunio. Additionally, it provides power to all electronic components. The Raspbery Pi, on the other hand, is in charge of tracking plants, taking photos, and controlling the push buttons. The electronic components are contained in a container referred to as the electronics box that is attached to the gantry. The figures below show the different components of the electronic box.

![](/images/Farmbot14.png)
![](/images/Farmbot15.png)
![](/images/Farmbot16.png)