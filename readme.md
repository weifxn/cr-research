# Motor


<!-- ![Brush-v-brushless](https://www.unmannedsystemssource.com/wp-content/uploads/2017/12/bldc_nws.jpg)

![Commutator](http://hyperphysics.phy-astr.gsu.edu/hbase/magnetic/imgmag/comtat.png)


| Brushed | Brushless |  
|----------------- |-------------------| 
|Uses electromagnet system as rotor surrounded by permanent magnets|magnetic rotor surrounded by electro magnet|  
|Inefficient due to the **power losses from imperfect power transfer** through the commutator system|Efficient without power losses|  
|**Shorter lifetime** due to wear of brushes and commutators |Does not suffer from short lifetime because they doesn't have commutation parts |  
|Lowering voltage reduces speed also reduces torque|Torque is highest at slow speeds|
|Too fast to be useful (requires gearing system to reduce speed)|Frequently used directly without gearing|  -->


## Current
### [350W Electric Scooter Motor](https://www.cytron.io/c-dc-motor/c-automobile-dc-motor/p-xyd-6d-350)
![350W](https://www.cytron.io/image/cache/catalog/products/350w-electric-scooter-motor-33037-800x800.jpg)


| | |
| ---- | -------------------| 
|Price| RM150|
|Voltage| 24VDC|
|Rated Speed| 2600RPM|
|Rated Torque| 1.2Nm|
|Rated Current| 18Amp|
|Rated Output Power| 350W|

## Selected
### [450W Electric Scooter Motor](https://www.cytron.io/c-dc-motor/c-automobile-dc-motor/p-xyd-16-450)
![450W](https://www.cytron.io/image/cache/catalog/products/450w-electric-scooter-motor-with-gear-34900-800x800.jpg)


| | |
| ---- |-------------------| 
|Price| RM329|
|Voltage| 36VDC|
|Rated Speed| 395RPM|
|Rated Torque| 11Nm|
|Rated Current| 26.5Amp|
|Rated Output Power| 450W|

## Comparison

| | 350W Motor | 450W Motor |
| ---- |---|-------------------| 
|Price|RM150 |RM329|
|Voltage|24VDC |36VDC|
|Rated Speed|2600RPM| 395RPM|
|Rated Torque|1.2Nm|11Nm|
|Rated Current|18Amp|26.5Amp|
|Rated Output Power|350W|450W|

## Definition

sources: [1](https://platinumasi.com/Brushless%20Vs%20Brushless%20Motor.pdf) [2](
https://www.precisionmicrodrives.com/content/dc-motor-speed-voltage-and-torque-relationships/) [3](https://tutorial.cytron.io/2018/06/16/choosing-a-dc-motor/)

#### RPM
- Rotation Per Minute
- Speed of rotating object 

![rpm](https://tutorial.cytron.io/wp-content/uploads/2018/06/RPM-calculation-for-motor-of-a-mobile-robot.png)

#### Torque 
- Measure of how much force we need to rotate an object
- Torque = Force x Distance
- Torque = Mass of the load (in Newton) x Radius of the wheel (in meter)
- Higher torque, lower speed
- Higher torque, higher current

![torque](https://tutorial.cytron.io/wp-content/uploads/2018/06/Simplified-torque-calculation-for-a-motor-of-a-mobile-robot-1.png)

### Voltage
- Supply to power the motors, lower voltage will result in lesser power
- Does not affect torque
- Force that pushes current

### Current
- Current used to power the motor
- Pushing wall will spike

### Watt (Power)
- Load that can carry

### Gearing
- trades speed for torque


### Collision
- the higher the power of the motor, the higher the load torque
- when your components are rated 12v you can only supply 12v battery to your components if not more than that will fry your circuits because higher voltage would allow more current to flow through than it should be

# Battery

## Current
### LiPo Rechargeable Battery 24V 5000mAh

*[ no image ]*

| | |
| ---- |-------------------| 
|Price|  ?? |
|Voltage| 24V |
|Capacity| 5000mAh|
|C Rating| ?? |



## Selected
### [Tiger Lipo Batteries 3S 5200mAh](https://shopee.com.my/Tiger-Lipo-Batteries-(2200mah-5400mah)-i.2889569.473969173)
![bat](https://i.imgur.com/8RqTJYE.png)
![spec](https://i.imgur.com/LEtqryQ.png)

| | |
| ---- |-------------------| 
|Price|  RM150 |
|Voltage| 3S (3.7V x 3 = 11.1V) |
|Capacity| 5200mAh|
|C Rating| 45C (45 x 5.2 = 234A)|

## Comparison

| | 24V 5000mAh | 3S 5200mAh |
| ---- |-------------------| -----| 
|Price|  ?? | RM150 |
|Voltage| 24V | 3S (3.7V x 3 = 11.1V) |
|Capacity| 5000mAh| 5200mAh|
|C Rating| ?? | 45C (45 x 5.2 = 234A)|

### Calculations for 2 batteries (3S 5200mAh)
```
22.2V  = 11.1V x 2 batteries

10,400mAh = 5200mAh x 2 batteries
```

### Assuming using 2 motors (450W)
#### Total runtime (critical condition)
```
53A = 26.5A x 2 motors

0.19 hour = 10.4Ah(Capacity of 2 batteries)/53A

11.4 minutes = 0.19 hour x 60
```

#### Safe Voltage
```
22.2V (Batteries) < 24V (Motor)
```

### Assuming 4 motors (350W)
```
72A = 18A x 4 motors

0.14 hour = 10.4Ah(Capacity of 2 batteries)/72A

8.4 minutes = 0.14 hour x 60
```


## Definition

sources: [1](https://rogershobbycenter.com/lipoguide/)

#### Voltage/Cell Count
- **Nominal(default) voltage of 3.7V**. 7.4V battery means there are 2 cells in series (Voltage added together). 2S means 2 series

#### Capacity
- How much power the battery can hold
- **milli**Amp hours (mAh)/ how much drain can be put on the battery to discharge in one hour

#### Discharge Rating (‘C’ rating)
- **How fast battery can be discharged safely** without harming the battery.
- C in C Rating stands for **capacity**
- 30C = 30 x Capacity(in Amps)
- Going higher than that will degrade the battery faster than normal

# Comparison (4x350W vs 2x450W)

| | 4 x 350W | 2 x 450W |
| ---- |-------------------| -----| 
|Price|  RM600 (RM150 x 4) | RM658 (RM329 x 2) |
|Voltage| 24V | 3S (3.7V x 3 = 11.1V) |
|Total runtime| 8.4 minutes| 11.4 minutes|
|Torque| 4.8Nm (1.2Nm x 4) | 22Nm (11Nm x 2) |
|Speed| 2600RPM | 395RPM |


