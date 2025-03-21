# LifeSim
The U.S. Army Corps of Engineers LifeSim software is an agent-based system for estimating consequences with the fundamental intent to simulate population redistribution during an evacuation.  Life loss and economic damages are then determined by the hazard (e.g. flooding).

## Downloads
LifeSim was developed for the U.S. Army Corps of Engineers Risk Management Center. However, software developed at the Risk Management Center is made available to the public whenever appropriate. Use is not restricted and individuals outside of the Corps of Engineers may use the program without charge. RMC will not provide user assistance or support for this software to non-Corps users. However, we will respond to any reported software bugs.  Downloading this software indicates full acceptance of your responsibility in the use of this program. Please see the distribution policy for more details.

* [Download Version 2.1.5](https://github.com/USACE-RMC/LifeSim/releases/download/v2.1.5/LifeSim_2.1.5.7z)

## Features
LifeSim is designed to simulate the entire warning and evacuation process for estimating potential life loss and direct economic damages resulting from catastrophic floods. The following is a description of the major capabilities of LifeSim.
* Graphical User Interface
* Agent Based Modeling
* Evacuation Simulation
* Uncertainty
* Graphics and Reporting

## Graphical User Interface
The user interacts with LifeSim through a graphical user interface (GUI). The interface is designed to make it easy to use the software, while still maintaining a high level of efficiency for the user. The interface provides for the following functions:
* File Management
* Data Entry and Editing
* Life Loss and Direct Damage Analyses
* Tabulation and Graphical Displays of Input and Output Data
* GIS mapping and animations of results
* Reporting Facilities
* Context Sensitive Help

## Agent Based Modeling
LifeSim uses an agent-based approach to track individuals throughout the warning and evacuation process. During an evacuation, agents are interacting with the roads, other vehicles, and the incoming hazard. After the warning and evacuation process has been simulated, LifeSim calculates lethality for those people that are exposed and direct damages due to the hazard. By tracking individual people and their movements, LifeSim can help identify where people are most at risk of losing their lives, whether it is on roads or in structures.  We can now pinpoint the locations of greatest potential life loss, which is useful when developing alternative project formulations.
 
## Evacuation Simulation
Three modes of evacuation are included in LifeSim: cars, sports utility vehicles (SUV’s), and pedestrians. For vehicular evacuation, a dual-regime modified Greenshields model (USDOT) in conjunction with spillback enforcement is used for traffic propagation to represent the effects of traffic density and road capacity on vehicle speed. Each road is assigned default values for the number of lanes, free flow speed, traffic jam densities, and minimum stop-and-go speeds based on the Highway Capacity Manual (HCM) (TRB 2000).
To define the routes people use to evacuate, a road network is provided where each segment of the network contains information such as road category, directionality, ground offset (for bridges), and interconnectivity. The road network can be imported from an existing GIS polyline shapefile or from OpenStreetMap. OpenStreetMap is a collaborative project to create a free editable map of the world.
During each time step at the user defined interval Δt, evacuating groups move as far as the model allows until a destination point is reached, the group gets caught, or becomes stranded. If a flooded road is encountered, a new route is determined unless they are on a one-way street with no turns (e.g. highway off-ramp). The population group then keeps the flooded road in memory so that it will not try to evacuate through the road again.  If no new route can be found, the population group is considered stranded. More information on the evacuation simulation can be found in the LifeSim Technical Reference Manual (RMC 2021).
 
## Uncertainty
LifeSim applies both natural variability and knowledge uncertainty through monte carlo analysis. Multiple parameters can be entered with uncertainty including those that influence the warning and evacuation timeline. Each iteration in a simulation represents a scenario that could occur given the data uncertainties in the model. The results of the analysis provide a distribution of estimated consequences from a given hazard.

## Graphics and Reporting
To accommodate both the uncertainty and the agent-based computations, robust results reporting are available through plots, tables, animations, and GIS data layers. Output can be viewed as box and whisker plots which summarizes the results over all iterations of the monte carlo simulation. Results by iteration can be viewed by iteration number or by various sampled parameters to help determine which uncertain parameters results are most sensitive to. Detailed information can be generated for individual iterations which can be used to animate the evacuation process and display various plots, tables, and GIS layers for individual iterations.

## Support
The RMC is dedicated to maintaining and supporting the software, delivering updates, bug fixes, and enhancements annually or as needed. If you're experiencing a problem with LifeSim, please submit the following information to RMC.Software@usace.army.mil, along with a graphical representation of the bug (if available).

## Documentation
* [LifeSim User's Guide](https://iwrlibrary.sec.usace.army.mil/resource/06bd49f2-cdd5-4e50-b58b-96c804c18886)
* [LifeSim Technical Reference Manual](https://iwrlibrary.sec.usace.army.mil/resource/c1dae7c1-c83f-4e9d-82e9-f311fa67f2ef)
* [LifeSim Training Videos](https://www.youtube.com/playlist?list=PLCYnGQpA5NVbWlp1oIGDF74CjODRR31K2)
* [LifeSim Workshop Presentations](https://drive.google.com/file/d/1RYq88t5pGEB48jxVFTDISWdVVoqU8kqa/view)
* [Malpasset Validation Dataset](https://www.rmc.usace.army.mil/Software/LifeSim/Malpasset-Validation-Dataset/)
* [Joso Validation Dataset](https://www.rmc.usace.army.mil/Software/LifeSim/Joso-Validation-Dataset/)
* [ASDSO 2024 - A New Quantitative Risk Analysis Software for Dam and Levee Safety, RMC-TotalRisk](https://github.com/user-attachments/files/17684807/ASDSO.-.2024.-.New.Quantitative.Risk.Analysis.Software.RMC-TotalRisk.pdf)

## Training
* [Risk Management Center Training Center](https://www.rmc.usace.army.mil/Training/)
