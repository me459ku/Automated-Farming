---
title: "Product Specifications"
date: 2022-01-16T09:40:39+03:00
draft: false
---

#### Customer Requirements and Importance



To make use of the customer, the customer needs previously gathered in the initial market research stage must first be interpreted into semi-technical terms where the team can use to base their design and functionality. After the interpretation of the needs, it is also required to assign an importance rating for each of the interpreted customers' needs to help the team decide what needs they answer in their first iteration or so-called their minimum viable product. The interpreted needs with their respective importance rating (1 lowest & 5 is highest) are represented in the following table.

| No.   |      Interpreted Customer Need      |  Importance |
|----------|:-------------:|------:|
| 1 |  No permanent fasteners | 5 |
| 2 |  Use standard parts that are easy to find and are av. for DIYer and enthusiasts | 5 |
| 3 |  Detect when plants need to be watered| 5 |
| 4 |  Detect when weeds emerge| 5 |
| 5 |  Measure relative humidity | 3 |
| 6 |  Measure pH level of soil | 2 |
| 7 |  Detect when crops are ready for harvest | 1 |
| 8 |  Quality materials | 5 |
| 9 |  Can be controlled by the regular farmer/person | 5 |
| 10 |  Commonly used components | 4 |
| 11 |  Re-assemble | 5 |
| 12 |  Open source| 3 |
| 13 |  Water plants | 5 |
| 14 |  Measure Temp. | 3 |
| 15 |  Monitor health of plant | 5 |
| 16 |  Harvest crops | 1 |
| 17 |  Tasks have a small no. of steps to be completed | 4 |
| 18 |  Kill weeds | 5 |
| 19 |  Mobile application | 4 |
| 20 |  Humidity regulation | 3 |
| 21 |  Supplement system with delivery | 2 |
| 22 |  Controllable light system | 3 |
| 23 |  Temp. control system (with vent.) | 3 |


From the previous table, the top 10 needs based on their importance can be summarized in the following list:
- No permanent fasteners with easy to find spare parts
- Detect when plants need to be watered and water them
- Detect the emergence of weeds and eliminate them
- Quality materials
- Can be controlled by the regular farmer/person
- Re-assemble-able
- Monitor health of plants
This list gives an indication of what the targeted customer is looking for which offers insight into what features the system must have to be considered a minimum viable product, nevertheless, other needs should also be taken into account as this rating is subjective and when the time comes for the customer to pay its a completely different scenario, thus; the team must take into account not just the needs they think they need at the current time and consider how to build a product that can help pivot their life to a better place. This level of depth is not required by the team, but it would be nice to consider, making the other needs open for debate whether to be included or not which will be due to cost-benefit analysis as this project has a strict deadline.



### List of Metrics
The customer needs must also be interpreted to technical terms for them to be measurable. Identifying the metrics for each need and assigning a unit to it will not just help in the understanding of the needs but will also pave the path for the upcoming steps where the team must benchmark their proposed solution against other currently existing alternatives in the market. The metrics and units are available in the following table.


**No**|**Needs**|**Metric**|**Imp**|**Units**|**Desired**|**Target Value**|**further justification**
:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:
1|1,2,10,11,12|Generic Screws,Fasteners,Parts (Widely Av.)|5|List|From List|-|to be specified later
2|3,4,7,14,15,19|Smart Vision System|5|Binary|Yes|Yes|-
3|2,10|Number of places the items are accessible|4|List and Count|high|-|to be specified later
4|18|Min Avg. Radius of weed |3|mm|low|10mm|Reducing the size will increase the complexity of the weed detection system, hence smaller diameter is not needed since the system will not be able to detect a weed before that
5|18|Max Avg. Radius of weed |3|mm|high|50mm|the device shouldnt allow for weeds to reach that size so the edlimination criteria is smaller than that.
6|18|Accuracy of targeting|4|mm|small|5mm|Because of the above mentioned justifications
7|5|Accuracy of measurement (RH)|3|% Error|small|3%|Within industry standard for affordable and availble components and no further accuracy is needed for the targeted customer 
8|5|Resolution of measurement (RH)|3|%|Medium|3 to 5%|No further accuracy is needed for the application as a small deviation wouldnt have a huge effect espeicially for the use case of the product
9|5|Range of measurement (RH)|3|%| |10% to 90%|Most plants are grown within this range. 10% cacti and 90% for pinaples (tropical)
10|6|Range of measurement (PH)|4|PH (unitless)| |0 to 14 (Standard)|This is an industry sandard and it covers the entire range including the needed range
11|6|Accuracy of measurement (PH)|4|PH (unitless)| |0.1|It covers the needs of the application
12|6|Resolution of measurement (PH)|4|PH (unitless)| |0.1|This is the res. for most availble meters, smaller res. are availble but are not needed since the range of PH for most plants is between 5 to 7.5 (some may require higher or lower)
13|8|Life|5|months|High|5 to 10 years|May differ later
14|13|Accuracy & Precision of watering|5|%|high |75%|since all that is required to to water the area that the plant is in and the water will get soaked up and the plant can get it through its roots
15|13|Min Radius of watering (plant)|1|mm|medium|-|doesnt matter after further analysis
16|13|Max Radius of watering (plant)|4|mm|high|1m|to make sure the area of any plant is covered
17|13|Nozzle exit pressure|4|kPa|low|65 to 200 kPa|to allow for the water to reach the desired lication and not harm the plants when its relaeased on top of it and this range is availble domestically and in most buildings thus it might eliminate the need of a pump 
18|13|Resolution of amount of water released|4|mL/s|medium|10 mL/s|this is to be conntrolled to not over/under water the plants - cant be decided now since it is related to the nozzle exit size 
19|14|Resolution of measurement|3|C|low|1C|no further res is rquired since all that is needed is to be within the range of the desired temperature and deviation by the amount of the desired value for the target wouldnt have a substantial effect for the use case of the device
20|14|Range of measurement|3|C|medium|0 to 60C|Most plants (for the use of the device to be built can only be grown in that range)
21|14|Accuracy and Precision of measurement|3|%|medium|1 to 3%|equipment is widely availble and all that is needed is be in range of a required temperatue
22|17|Avg no. of steps for each task|3|no. of steps|low |-|must be compared with other devices on the market (will be decided in the benchmarking process)
23|3|Accuracy and Precision of detection|5|%|high|90%|this value needs to be high since it is somewhat harmful for the plant to not be watered when it is needed and for thart to be repeated multiple times
24|4|Accuracy and Precision of detection|5|%|high|90%|weeds will feed on the resources that are avialble for the main plants so they must be eliminated as soon as the emerge hence a high accuracy is required
25|7|Accuracy and Precision of detection|5|%|high|70%|leaving a crop for a while before harvesting it would/shouldnt have a huge effect (even getting it before it is 100% ripe)
26|9|No. of steps to setup|4|No. of steps|low|-|must be compared with other devices on the market (will be decided in the benchmarking process)
27|9|Ease of setup|4|Custom rating|high|-|must be compared with other devices on the market (will be decided in the benchmarking process)
28|9|Ease of use|4|Custom rating|high|-|must be compared with other devices on the market (will be decided in the benchmarking process)
29|9|Ease of troubleshooting|4|Custom rating|high|-|must be compared with other devices on the market (will be decided in the benchmarking process)
30|16|Types of crops that can be harvested|2|List|long list|-|-
31|16|Crops storage area|1|m3|high|-|To be specified later
32|21|No. of supplement type that can be stored|3|Count|medium|4 to 6|since multiple suppliments are usually needed - maybe the device can have an nexpansion kit
33|21|Amount of supplement that can be stored|2|L|medium|2 to 3 L|To allow for the storage of multiple types of suppliments (different compartments adding up to 2 to 3L with 500ml for each)
34|21|Exit pressure of supplement deliv. system|2|kPa|low|65 to 200 kPa|Similar to water exit pressure
35|20|Resolution of control (level of humidity)|3|%|medium|2% to 5%|all is required is to be within the range of the desired RH values
36|20|Time to change 1% of rel. humidity per m3|3|S/m3|low|10min|since the range needed shouldnt vary by too much and the existance for this system is just to maintain the required value (10 min) should be enough. it should also be able to completly change the number but can take longer times to setup if it rquirees to go from 10% to 80% for example
37|22|power rating of system|3|Watt|low|50 to 150W|within the range of a small home appliance - excluding greenhouse env. control - in standby it should be as close as possible to 0 
38|22|% of Area Covered|3|%|high|100%|Must cover the entire growing area to achive the required effect of emitating the sun
39|22|WaveLength Range|5|nm|custom|400-700nm|This is the range of wavvelength that replicate the sun
40|23|Resolution of control (level of Temp)|3|C|decent|1 to 3C|All that is needed is to be within the vicinity of the required growing temperature
41|23|Time to change temp 1C (Heating)|2|min|low|15|Faster change is not rquired for the application
42|23|Time to change temp 1C (cooling)|2|min|low|15|Faster change is not rquired for the application
43|19|Can be controlled by remotely|4|Binary|Yes|Yes|Not needed 





The first column of the previous table shows the number of the metric, the following column represents the number of the needs related to that specific metric which can be used to cross- reference with the former needs table. The third column shows the metric itself followed by its importance in the next column, and finally, the unit for each metric can be found in the last column.


### Target Specifications

The product specifications are objective, precise, and measurements of the product performance and by meeting the specifications, the product meets customer requirements as defined in the Textbook. In order to obtain the specifications, the customer needs were organized into a hierarchy and each need was assigned with an importance and a metric as it was shown in the presented information above.
The current target specifications are based on the components available in the market and/or the interpreted needs based on the understanding of the team members. The target specifications discussed below are not final and are subject to change after further market research is done. The change will be made with the objective of positioning the developed product in the area that allows for targeting the desired customer and keeping the costs as low as possible. The assumed target specifications are shown in table xx below with the justification (if any) for each one of them.

