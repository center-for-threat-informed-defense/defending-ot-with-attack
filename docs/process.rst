Process
=======

Defending OT with ATT&CK uses the methodology and tooling created as part of the Center's 
Defending IaaS with ATT&CK project.

Scope
-----

Determine the relevant technologies where a threat actor can impact operations and 
generate a reference architecture that depicts technologies in scope for a hybrid IT/OT system.

Scoping considerations: 
Adapted Purdue Reference Model (historically the primary reference to describe the structure of OT networks), ATT&CK for ICS asset list, international standards, potential sector-based use cases (e.g., factory automation, maritime transport).

Reference Assets
-----------------
The following considerations were taken foe defining the assets that comprise Defending OT 
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

Threat Model Methodology
------------------------

1. Identify the attack surface.
   Determine the relevant technologies where a threat actor can impact operations and 
   generate a reference architecture that depicts technologies in scope for a hybrid 
   IT/OT system.

2. Compile source information.
   Gather information resources and applicable cyber threat intelligence including ATT&CK 
   adversary behavior used to target the identified IT/OT systems.

3. Define selection criteria. 
   Develop guidelines including or excluding an adversary activity from the threat model. 
   Selection criteria includes:
   - Virtualized infrastructure (e.g., virtual machines, cloud)
   - Physical technologies (e.g., identity access management servers, network)
   - Operational technologies (e.g., PLC, HMI)

4. Review applicable adversarial techniques. 
   Evaluate adversary techniques according to prior defined criteria. Exclude 
   non-applicable techniques.

5. Build custom threat collection. 
   Generate a tailored threat intelligence collection for hybrid IT/OT systems. Provide 
   the collection in a sharable and extensible format.