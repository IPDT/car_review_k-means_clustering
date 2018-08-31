# k-means clustering for car reviews
## Three dataset as below
### tags before cluster

   ||car_reviews|edmunds|thecarconnection
   :-:|:-:|:-:|:-:
   1|Audio and Infotainment|comfort|green
   2|Cargo Space and Storage|driving|performance
   3|Driving Impressions and Performance|interior|quality
   4|Exterior Design and Dimensions|performance & mpg|safety
   5|Fuel Economy and Driving Range|safety|styling
   6|Interior and Passenger Space|technology|
   7|Powertrain and Charging|trim levels & features|
   8|Safety and Driver Assistance|utility|
   9|Warranty and Maintenance Coverage|
   10|Engine and Transmission|
    
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
    ```
    27412 documents
    Cluster distribution:
    Cluster 5: {0: 2271, 1: 21821, 2: 1051, 3: 1577, 4: 692} 0.8931739140359255
    Cluster 6: {0: 20436, 1: 1186, 2: 1101, 3: 2799, 4: 361, 5: 1529} 0.8844235485391917
    Cluster 7: {0: 862, 1: 856, 2: 2604, 3: 7652, 4: 1718, 5: 13063, 6: 657} 0.8795675106660413
    Cluster 8: {0: 942, 1: 800, 2: 1202, 3: 1892, 4: 893, 5: 6581, 6: 14553, 7: 549} 0.8701556685113421
    Cluster 9: {0: 16918, 1: 1165, 2: 780, 3: 3081, 4: 800, 5: 1457, 6: 745, 7: 709, 8: 1757} 0.8558720335350157
    Cluster 10: {0: 1024, 1: 13240, 2: 991, 3: 3405, 4: 704, 5: 544, 6: 655, 7: 4002, 8: 1691, 9: 1156} 0.8517616401189498
    Cluster 11: {0: 814, 1: 10887, 2: 1346, 3: 1074, 4: 1306, 5: 997, 6: 3396, 7: 1037, 8: 654, 9: 4023, 10: 1878} 0.8457740803778363
    Cluster 12: {0: 568, 1: 715, 2: 1352, 3: 12767, 4: 4198, 5: 440, 6: 699, 7: 1013, 8: 1525, 9: 2183, 10: 990, 11: 962} 0.8307214349288249
    Cluster 13: {0: 1236, 1: 10372, 2: 3556, 3: 1068, 4: 2020, 5: 996, 6: 3961, 7: 677, 8: 204, 9: 745, 10: 1033, 11: 1174, 12: 370} 0.8286565026891466
    Cluster 14: {0: 990, 1: 3929, 2: 1449, 3: 2052, 4: 798, 5: 689, 6: 354, 7: 627, 8: 939, 9: 361, 10: 10006, 11: 640, 12: 1573, 13: 3005} 0.8121522578356923
    ```

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
    
    ```
    172248 documents
    {0: 109887, 1: 13993, 2: 9173, 3: 30612, 4: 8583}
    5 0.9012698050052816
    {0: 9149, 1: 106555, 2: 8560, 3: 5963, 4: 12332, 5: 29689}
    6 0.889721494694458
    {0: 8556, 1: 17490, 2: 17163, 3: 5959, 4: 28760, 5: 4850, 6: 89470}
    7 0.8858911655005254
    {0: 14060, 1: 12957, 2: 16034, 3: 4496, 4: 9189, 5: 22483, 6: 5553, 7: 87476}
    8 0.8796700664810887
    {0: 65859, 1: 8258, 2: 9029, 3: 38090, 4: 5944, 5: 18060, 6: 14403, 7: 5569, 8: 7036}
    9 0.8658370227351719
    {0: 8252, 1: 31105, 2: 53068, 3: 10689, 4: 4551, 5: 4840, 6: 5522, 7: 16049, 8: 32716, 9: 5456}
    10 0.8662924133979836
    {0: 8159, 1: 26257, 2: 6670, 3: 7306, 4: 27240, 5: 7777, 6: 5916, 7: 49504, 8: 15057, 9: 13828, 10: 4534}
    11 0.8661859018849154
    {0: 13568, 1: 7016, 2: 5562, 3: 5955, 4: 8319, 5: 4831, 6: 17276, 7: 34364, 8: 4605, 9: 4281, 10: 59403, 11: 7068}
    12 0.845146120840502
    {0: 9851, 1: 8310, 2: 5932, 3: 13905, 4: 11330, 5: 12478, 6: 4598, 7: 5542, 8: 13509, 9: 4343, 10: 70715, 11: 6913, 12: 4822}
    13 0.840640235763226
    {0: 6091, 1: 8184, 2: 12987, 3: 11967, 4: 4755, 5: 4584, 6: 64184, 7: 8931, 8: 5914, 9: 5446, 10: 10445, 11: 10195, 12: 13032, 13: 5533}
    14 0.8402796078490573
    ```

### thecarconnection
* result
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
* cost trend

    ![thecarconnection](thecarconnection_(3,8).png)
    ```
    107715 documents
    Cluster distribution:
    Cluster 3: {0: 79077, 2: 18331, 1: 10307} 0.9248839267944382
    Cluster 4: {2: 55226, 3: 36969, 0: 10188, 1: 5332} 0.918130590608453
    Cluster 5: {1: 14711, 0: 64793, 4: 12830, 3: 10145, 2: 5236} 0.9117029461838286
    Cluster 6: {1: 13305, 2: 22135, 4: 47575, 5: 9897, 0: 9604, 3: 5199} 0.9067644559857724
    Cluster 7: {6: 36020, 1: 13401, 2: 18572, 5: 16371, 3: 8934, 4: 9251, 0: 5166} 0.9035498516286458
    ```
  