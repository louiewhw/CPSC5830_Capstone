# CPSC5830_Capstone

## Problem Statement

On-time performance plays an important role in airline operations and management since the on-time performance needs to be as efficient as possible to save costs and improve airline productivity.

Given that, the vision of the project aims to analyze the on-time stats of several major airlines, be updated daily, and display it through an interactive dashboard.

## Approach
The approach begins by joining the flight data which we obtained from ADSB and external schedule data to get the on-time statistics for several major airlines. After that, we will use the joined data to build a data pipeline for the ADSB and external schedule data. 

Next, we will analyze and build an interactive dashboard that will display these on-time stats and be updated daily automatically whenever new data is available in S3.

## Dataset

Our data requires that both ADSB and Flight schedule datasource to have the 'ICAO' code and departure and arrival times to be able to join the datasets together. The data must also correspond to the exact dates from both datasets, with ample attribute fill-rates.​

**ADSB Observations Dataset: Flight tracking data**

- 'ICAO' Code

- 'Gnd' (Grounded)

- 'From' (Departure Airport)

- 'To' (Arrival Airport)

- 'Fseen/PosTime' (Actual Departure time & Arrival time)

- 'Lat' and 'Long' (Location)



**External Datasource: Flight schedule API** [aviation-edge](https://aviation-edge.com/premium-api/)

(aviation-edge support team)

```Aviation Edge collects flight and airport data from hundreds of sources, including official authorities as well as other established industry partners such as airlines and airports and compiles this data in their extensive database.```

- 'ICAO' Code

- From

- To

- Departure Time

- Arrival Time
