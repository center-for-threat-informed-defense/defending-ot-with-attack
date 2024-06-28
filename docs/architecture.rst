Reference Architecture
======================

Scope
-----
Determine the relevant technologies where a threat actor can impact operations and 
generate a reference architecture that depicts technologies in scope for a hybrid IT/OT system.

Scoping considerations: 
Adapted Purdue Reference Model (historically the primary reference to describe the structure of OT networks), ATT&CK for ICS asset list, international standards, potential sector-based use cases (e.g., factory automation, maritime transport).
•	Understand the Purdue Reference Model: 
The Purdue Enterprise Reference Architecture (PERA) model is a framework for organizing industrial control systems (ICS) into hierarchical levels. It helps in structuring the segmentation of industrial processes and IT systems, enhancing security by delineating clear boundaries between different operational zones. The Purdue Model is widely used in industrial settings to define and manage interactions between IT and OT systems. It helps in implementing robust security measures by segregating networks and systems based on their functions and criticality.

Reference Assets
-----------------
The following considerations were taken for defining the assets that comprise Defending OT 
with ATT&CK's reference architecture:

* Enterprise IT and OT Security
  -  Enterprise IT and OT security attack surface management, OT and ICS areas of interest, 
     network assets, wireless protocols in energy sector, manufacturing systems.
* Network Segmentation, Governance, and Compliance
  - Measured inclusion due to the limitations of mapping these assets to attack vectors, 
* Architecture and Attack Vectors
  - Abstraction of cloud OT and on-prem OT to account for different attack vectors. 
* Adversaries and Goals in IT compared to OT
  - Distinction emphasized between IT networks where adversaries seek information exfiltration 
    and OT networks where objectives are focused on operations disruption.
* Impacting ICS
  - Understanding impact to assets, particulary in context of ICS and application of ATT&CK 
    in IT and OT environments.