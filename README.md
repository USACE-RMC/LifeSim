# LifeSim
The U.S. Army Corps of Engineers LifeSim software is used to estimate life loss and economic damages from flooding.

![image](https://github.com/user-attachments/assets/51919088-8250-48a8-8f18-bdbb3287051a)

## Downloads
LifeSim was developed for the U.S. Army Corps of Engineers Risk Management Center. However, software developed at the Risk Management Center is made available to the public whenever appropriate. Use is not restricted and individuals outside of the Corps of Engineers may use the program without charge. RMC will not provide user assistance or support for this software to non-Corps users. However, we will respond to any reported software bugs.  Downloading this software indicates full acceptance of your responsibility in the use of this program. Please see the [distribution policy](https://www.rmc.usace.army.mil/Software/Distribution/) for more details.

* [Download Version 2.1.5](https://github.com/USACE-RMC/LifeSim/releases/download/v2.1.5/LifeSim_2.1.5.7z)

## Features
LifeSim is designed to simulate the entire warning and evacuation process for estimating potential life loss and direct economic damages resulting from catastrophic floods.

The graphical user interface (GUI) is designed to make it easy to use the software, while still maintaining a high level of efficiency. The interface provides functionality for data entry and editing, tabulation and graphical displays, GIS mapping, and animation.

LifeSim uses an agent-based approach to track individuals throughout the warning and evacuation process. During an evacuation, agents are interacting with the roads, other vehicles, and the incoming hazard. By tracking individual people and their movements, LifeSim can help identify where people are most at risk of losing their lives.

The vehicular evacuation engine employs a dual-regime modified Greenshields model with spillback enforcement. During each time step at the user defined interval Δt, evacuating groups move as far as the model allows until a destination point is reached, the group gets caught, or becomes stranded. More information on the evacuation simulation can be found in the [LifeSim Technical Reference Manual](https://iwrlibrary.sec.usace.army.mil/resource/c1dae7c1-c83f-4e9d-82e9-f311fa67f2ef) (RMC 2021).

LifeSim applies both natural variability and knowledge uncertainty through monte carlo analysis. Multiple parameters can be entered with uncertainty including those that influence the warning and evacuation timeline. Each iteration in a simulation represents a scenario that could occur given the data uncertainties in the model. The results of the analysis provide a distribution of estimated consequences.

## Support
The RMC is dedicated to maintaining and supporting the software, delivering updates, bug fixes, and enhancements annually or as needed. If you're experiencing a problem with LifeSim, please submit the following information to RMC.Software@usace.army.mil, along with a graphical representation of the bug (if available).

## Tools
* [LifeSim ArcGIS Tools](https://github.com/BuchananKurt/LifeSim_ArcGIS_Tools)

## Documentation
* [LifeSim User's Guide](https://iwrlibrary.sec.usace.army.mil/resource/06bd49f2-cdd5-4e50-b58b-96c804c18886)
* [LifeSim Technical Reference Manual](https://iwrlibrary.sec.usace.army.mil/resource/c1dae7c1-c83f-4e9d-82e9-f311fa67f2ef)

## Datasets
* [Malpasset Validation Dataset](https://www.rmc.usace.army.mil/Software/LifeSim/Malpasset-Validation-Dataset/)
* [Joso Validation Dataset](https://www.rmc.usace.army.mil/Software/LifeSim/Joso-Validation-Dataset/)

## Training
* [Risk Management Center Training Center](https://www.rmc.usace.army.mil/Training/)
* [LifeSim Training Videos](https://www.youtube.com/playlist?list=PLCYnGQpA5NVbWlp1oIGDF74CjODRR31K2)
* [LifeSim Workshop Presentations](https://drive.google.com/file/d/1RYq88t5pGEB48jxVFTDISWdVVoqU8kqa/view)
