# Dataset feature description
The set of features is described in the tables below (organized by events). Each table highlights the generated features of the according event.


### Hands-On Events
Event indicating the detection of the driver's hands on the steering wheel.

| Variable | Description                 |
| :------- | :-------------------------- |
| n_lod_0  | Number of no hands events   |
| n_lod_1  | Number of left hand events  |
| n_lod_2  | Number of right hand events |
| n_lod_3  | Number of both hand events  |


### Drowsiness Events
Event indicating driver drowsiness level (based on KSS).

| Variable       | Description                         |
| :------------- | :---------------------------------- |
| n_drowsiness_0 | Number of drowsiness events level 0 |
| n_drowsiness_1 | Number of drowsiness events level 1 |
| n_drowsiness_2 | Number of drowsiness events level 2 |
| n_drowsiness_3 | Number of drowsiness events level 3 |


### Driving Behavior Events
Events indicating occurrence of harsh acceleration, harsh braking, and harsh cornering behaviours.

| Variable | Description                                              |
| :------- | :------------------------------------------------------- |
| n_ha     | Number of harsh acceleration events                      |
| n_ha_l   | Number of harsh acceleration events with low severity    |
| n_ha_m   | Number of harsh acceleration events with medium severity |
| n_ha_h   | Number of harsh acceleration events with high severity   |
| n_hb     | Number of harsh braking events                           |
| n_hb_l   | Number of harsh braking events with low severity         |
| n_hb_m   | Number of harsh braking events with medium severity      |
| n_hb_h   | Number of harsh cornering events                         |
| n_hc_l   | Number of harsh braking events with high severity        |
| n_hc     | Number of harsh cornering events with low severity       |
| n_hc_m   | Number of harsh cornering events with medium severity    |
| n_hc_h   | Number of harsh cornering events with high severity      |


### Distraction Events
Real-time mobile phone use events from the driver app.

| Variable         | Description                     |
| :--------------- | :------------------------------ |
| distraction_time | Time spent distracted (seconds) |
| n_distractions   | Number of distraction events    |


### Ingnition Events
Ignition events.

| Variable       | Description                   |
| :------------- | :---------------------------- |
| n_ignition_on  | Number of ignition ON events  |
| n_ignition_off | Number of ignition OFF events |


### Mobileye Advanced Warning System Events
Gives information about the safety and warning state of the Mobileye system.

| Variable        | Description                                                                 |
| :-------------- | :-------------------------------------------------------------------------- |
| fcw_time        | Time forward collision warning was active (seconds)                         |
| hmw_time        | Time headway monitoring was active (seconds)                                |
| ldw_time        | Time lane departure warning was active (seconds)                            |
| pcw_time        | Time pedestrian collision warning was active (seconds)                      |
| n_pedestrian_dz | Number times a pedestrian is detected in danger zone                        |
| light_mode      | Trip Lighting condition (Most frequent)                                     |
| n_tsr_level     | Number of times the speed limit was exceeded                                |
| n_tsr_level_0   | Number of times the speed limit was not exceeded                            |
| n_tsr_level_1   | Number of times 0-5 units over speed limit                                  |
| n_tsr_level_2   | Number of times 5-10 units over speed limit                                 |
| n_tsr_level_3   | Number of times 10-15 units over speed limit                                |
| n_tsr_level_4   | Number of times 15-20 units over speed limit                                |
| n_tsr_level_5   | Number of times 20-25 units over speed limit                                |
| n_tsr_level_6   | Number of times 25-30 units over speed limit                                |
| n_tsr_level_7   | Number of times 30+ units over speed limit                                  |
| zero_speed_time | Time the vehicle was stopped (seconds)                                      |
| n_zero_speed    | Number of times the vehicle stopped (first time ignition ON does not count) |


### Mobileye Car Events
Gives information about the about the car parameters needed for the Mobileye system.

| Variable         | Description                                           |
| :--------------- | :-----------------------------------------------------|
| n_high_beam      | Number of times high beam is ON                       |
| n_low_beam       | Number of times low beam is ON                        |
| n_wipers         | Number of times wipers are ON                         |
| n_signal_right   | Number of times right turn signal is ON               |
| n_signal_left    | Number of times left turn signal is ON                |
| n_brakes         | Number of times breaks are ON                         |
| speed            | Mean Speed (km/h)                                     |
| over_speed_limit | Number of times over speed limit (with openstreetmap) |


### Forward Collision Warning (FCW) Events
Computed geolocations of Mobileye FCW events.

| Variable | Description          |
| :------- | :------------------- |
| n_fcw    | Number of FCW events |


### Headway Monitoring & Warning (HMW) Events
Computed geolocations of Mobileye HMW events.

| Variable | Description          |
| :------- | :------------------- |
| n_hmw    | Number of HMW events |


### Lane Departure Warning (LDW) Events
Computed geolocations of Mobileye LDW events.

| Variable    | Description                |
| :---------- | :------------------------- |
| n_ldw       | Number of LDW events       |
| n_ldw_left  | Number of LDW left events  |
| n_ldw_right | Number of LDW rigth events |


### Pedestrian Collision Warning (PCW) Events
Computed geolocations of Mobileye PCW events.

| Variable | Description          |
| :------- | :------------------- |
| n_pcw    | Number of PCW events |


### Fatigue Events
Real-time fatigue intervention levels.

| Variable    | Description                                                   |
| :---------- | :------------------------------------------------------------ |
| n_fatigue_0 | Number of fatigue level 0 events, no warning                  |
| n_fatigue_1 | Number of fatigue level 1 events, visual warning              |
| n_fatigue_2 | Number of fatigue level 2 events, visual and auditory warning |
| n_fatigue_3 | Number of fatigue level 3 events, visual and auditory warning |


### Headway Events
Real-time headway intervention levels.

| Variable     | Description                                            |
| :----------- | :----------------------------------------------------- |
| n_headway__1 | Number of headway level -1 events, no vehicle detected |
| n_headway_0  | Number of headway level 0 events, vehicle detected     |
| n_headway_1  | Number of headway level 1 events, vehicle detected     |
| n_headway_2  | Number of headway level 2 events, first warning stage  |
| n_headway_3  | Number of headway level 3 events, second warning stage |


### Overtaking Events
Real-time overtaking intervention levels.

| Variable       | Description                                                      |
| :------------- | :--------------------------------------------------------------- |
| n_overtaking_0 | Number of overtaking level 0 events, no warning                  |
| n_overtaking_1 | Number of overtaking level 1 events, visual warning              |
| n_overtaking_2 | Number of overtaking level 2 events, visual and auditory warning |
| n_overtaking_3 | Number of overtaking level 3 events, frequent warning            |


### Speeding Events
Real-time speeding intervention levels.

| Variable       | Description                                                    |
| :------------- | :------------------------------------------------------------- |
| n_speeding_0   | Number of speeding level 0, events no warning                  |
| n_speeding_1   | Number of speeding level 1, events visual indication           |
| n_speeding_2   | Number of speeding level 2, events visual speeding warning     |
| n_speeding_3   | Number of speeding level 3, events visual and auditory warning |