

# Plastic_transport_saigon

Code supporting the publication "Plastic does not simply flow into the sea: Transport dynamics affected by tides and floating plants"

Processes raw trajectory csv files by detecting periods the trajectory was stopped, filling in gaps, and removing missing data


# Dataset can be found at doi:10.4121/21582996 

Title of the dataset:
Lagrangian observations floating macroplastic litter in the Saigon River, Vietnam 2022

Creators:
Romi Lotcheris
Khiet Bui

Contributers: 
Louise Schreyers
Khoa Thi

Description:
This study examined the combined patterns of transport, trapping, and remobilisation of macroplastic items in a tropical tidal river over the course of a full month, with a focus on dynamics over a single tidal cycle. We used GPS trackers, released at different stages during the tidal cycle, to collect high frequency observations of both trapping and transport dynamics. Experiments were carried out from 17 May 2022 to 15 June 2022. 

We used GPS trackers affixed to expanded polystyrene (EPS) boxes to replicate the transport dynamics of macroplastic items in the Saigon River in Ho Chi Minh City, Vietnam. Items were released from 3 bridges in the study region, from most downstream to most upstream: Thu Thiem bridge (10.786274, 106.718091, n = 2), Binh Loi bridge (10.825698, 106.709175, n = 53), and Phu Long bridge (10.890252, 106.692063, n = 3). The study region included 40km stretch of river, from the confluence of the Saigon with the Dong Nai South of the city to 5km upstream of the most upstream bridge. Trackers travelling beyond either the upstream or downstream boundary were considered to have left the system.

For each tracker experiment, four to six trackers were released at the same locations at the mid-point of the release bridges. Trackers were released at different times to cover the full range of tidal conditions for short time-scales (daily - weekly): 24 at ebb tide, 34 at flood tide, 27 at spring tide, 31 at neap tide (41% vs. 59%, and 47% vs. 53% respectively). The trackers remained in the system for at least one tidal cycle (24 hours and 50 minutes). Trackers (n = 58) were deployed for an average time period of 2 days 12:15:54 ± 3 days 01:05:31 (median = 1 day 11:53:50). Water and air pressure were measured for the Thu Thiem and Binh Loi bridges from which the water level was calculated. This was used to determine the phase of the tide throughout the study period (flood, ebb, and slack water). 

Keywords:
Plastic pollution
Tidal dynamics
Hydrology
Macroplastic
Estuaries

Spatial coverage:
The Saigon River in Ho Chi Minh City, Vietnam

Temporal coverage:
17 May 2022 to 15 June 2022. 

This dataset contains the follow files: 
1. 58 .csv files labelled 'track_x.csv', where x corresponds to the trajectory number from 1 ... 58. Each trajectory file is a series of points each with a numberical identifier ('id'), the GPS tracker label ('tracker_id'), the bridge of release ('bridge'), a timestamp ('date_time'), and the longitude ('long') and latitude ('lat') of each point in the trajectory. 

2. Four .csv files with the water and air pressure data for Binh Loi and Thu Thiem bridges. Each file has a timestamp, the measured pressure ('pressure') and temperature ('temperature') at each measurement point. Measurements were taken every minute.   
		'binh_loi_baro.csv'
		'binh_loi_water.csv'
		'thu_thiem_baro.csv'
		'thu_thiem_water.csv'

3. A csv file labelled 'locations_found.csv' detailing the characteristics of the sites where each item was retrieved at the end of its trajectory. The dataset contains the numerical identifier for each trajectory, and then classifies the locations based on a nested classification system. 'Loc_1' refers to where in the river cross-section the item was found (midstream, edge, or canal). 'Loc_2' refers to, based on where in the river cross section it was found, what kind of environment the item was associated with (infrastructure, riparian vegetation (excl. hyacinths), or none i.e. free-floating). The third category 'hyacinths' refers to whether or not the item was found in association with waterr hyacinths (either yes or no). 'Tide_phase_retrieve' is a calcualted value based on the tidal data and the end time of trajectories and refers to whether the tide was in its spring or neap phase when it was retrieved. 'Tide_state_retrieve' is also a calculated value calculated in the same way, and refers to wether the item was retrieved during flood, ebb, or slack tide. 'Net_transport_direction' refers to wether the item was retrieved upstream or downstream with respect to the release location. 



