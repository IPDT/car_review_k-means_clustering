# k-means clustering for car reviews
## there's 3 dataset as below
### car reviews
* 10 classes (before cluster)
  * Audio and Infotainment
  * Cargo Space and Storage
  * Driving Impressions and Performance
  * Engine and Transmission
  * Exterior Design and Dimensions
  * Fuel Economy and Driving Range
  * Interior and Passenger Space
  * Powertrain and Charging
  * Safety and Driver Assistance
  * Warranty and Maintenance Coverage
  
### edmunds
* 8 classes (before cluster)
  * comfort
  * driving
  * interior
  * performance & mpg
  * safety
  * technology
  * trim levels & features
  * utility
  
### thecarconnection
* 5 classes (before cluster)
  * green
  * performance
  * quality
  * safety
  * styling
 
## first version of k-means cluster
### car reviews
* result
```
Top terms per cluster:
None
Cluster 0: with standard wheel is automatic speed on for all drive
Cluster 1: assigns stars overall nhtsa cars five rating an out quicker
Cluster 2: to it is of in its that but for as
Cluster 3: visibility by laser roof pillar width location pillars blind spots
Cluster 4: system infotainment inch touchscreen is standard to apple android carplay
Cluster 5: seat rear seats space of in cargo to front is
Cluster 6: highway mpg our fuel loop on economy epa 200 mile
Cluster 7: usb devices current all response amps latency ports following times
Cluster 8: sound decibels pressure at of meter while is 70 cruising
Cluster 9: safety iihs pick tests top vehicles highway nhtsa crashworthiness evaluate
Cluster distribution:
{0: 5189, 2: 10189, 6: 1563, 4: 1780, 5: 3180, 8: 1015, 1: 823, 3: 1921, 7: 1046, 9: 706}
0.853754658731952
```

* cost trend

    ![car reviews](car_review_(5,15).png)

### edmunds
* result
```
Top terms per cluster:
None
Cluster 0: are available on of there to as for seats in
Cluster 1: mph 60 in seconds testing edmunds from zero to feet
Cluster 2: system power inch with package rear wheels adds an heated
Cluster 3: to it of you can be but in is that
Cluster 4: mpg speed transmission automatic combined city manual six highway is
Cluster 5: torque liter hp lb ft of pound feet horsepower produces
Cluster 6: is in of with for on as trim available that
Cluster 7: side airbags impact for frontal front stars crash safety curtain
Cluster distribution:
{6: 54532, 0: 16175, 3: 38871, 2: 27526, 1: 5957, 4: 11925, 5: 8323, 7: 8939}
0.8781821498579485
```
* cost trend

    ![edmunds](edmunds_(5,15).png)

### thecarconnection
```
Top terms per cluster:
None
Cluster 0: safety crash side for test airbags iihs of in features
Cluster 1: mpg highway city combined epa at drive with fuel rated
Cluster 2: of it to is in that with on its for
Cluster 3: seats seat space in for comfort of rear room is
Cluster 4: speed engine to liter with of automatic is in torque
Cluster distribution:
{3: 14693, 2: 64812, 4: 12831, 0: 10143, 1: 5236}
0.9117029397988335
```
 
  