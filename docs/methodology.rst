Threat Model Methodology
========================

This project used a structured approach to ensure a thorough analysis and documentation of 
potential adversarial techniques, tailored to the specific assets and architecture of the 
organization. By following these steps, organizations can effectively delineate their attack 
surface, compile relevant threat intelligence, apply rigorous selection criteria, and build 
a comprehensive threat collection to bolster their cybersecurity defenses.

Step 1. Identify the attack surface.
------------------------------------

The first step is to identify the attack surface. This includes the system components that are in 
scope, the range of technologies comprising the system, and the user archetypes involved in the system. 
Delineate the security boundary, especially in vendor scenarios where responsibilities may be shared 
with or delegated to a partner organization. Determine the relevant technologies where a threat actor can 
impact operations and generate a reference architecture that depicts technologies in scope for a hybrid 
IT/OT system. For Defending OT with ATT&CK's threat collection, the attack surface is compromised of all the 
assets selected for the :doc:`architecture` table.

**Objective:**  Define the system components, technological assets, and user archetypes that 
form the architecture's attack surface.

**Actions:**

* Identify System Components and Enumerate Technologies
  
  * Determine the scope of the systems, including enterprise IT platforms and ICS, by listing the assets and technologies involved (e.g., Hardware, Network, Operating Systems, Applications, Cloud services, Containers, etc.).

* Categorize Reference Architecture Assets

  * Categorize total assets, identifying key assets with known adversarial risks from IT/OT perspectives.

**Example Assets:**

* Servers and Endpoints: Control Server, Programmable Logic Controller, Application Server
* Identity and Access Management: Azure AD/Entra ID
* Networking Components: Routers, Switches, Firewalls
* ICS Assets: Human-Machine Interface, Safety Controllers, Data Gateway

To learn more about assets, visit :doc:`architecture`

Step 2. Compile source information.
-----------------------------------

The second step is to gather information resources and applicable cyber threat intelligence 
including ATT&CK adversary behavior used to target the identified IT/OT systems. The adversarial 
techniques from relevant cyber threat intelligence (CTI) sources are combined to form a list of 
candidates for the threat collection, yet some of these techniques will not be applicable to all 
assets. To create a broad picture of all feasible adversarial techniques that could affect the 
architecture, it is important to consult multiple sources to identify key CTI and datasets from 
the ATT&CK framework:

* Industrial Control Systems
* Linux  
* Cloud (IaaS, SaaS, Azure, AWS, GCP, O365)
* Containers
* Windows
* Azure AD
* Network

**Objective:** Gather relevant cyber threat intelligence (CTI) sources to identify potential adversarial techniques for each listed asset.

**Actions:**

* Consult CTI Sources

  * Use sources like MITRE's ATT&CK for Enterprise and ICS.

* Generate Comprehensive List

  * Combine adversarial techniques relevant to each type of asset.

* Categorize Techniques

  * Based on asset types such as ICS, Linux, Cloud (e.g., IaaS, SaaS), Containers, Windows, Azure AD, and Network.

**Key Focus Areas:**

* Industrial Control Systems (ICS)
* Operating Systems (Linux, Windows)
* Cloud Services (AWS, Azure, GCP)
* Containers (Docker)
* Identity Management (Azure AD)

Step 3. Define selection criteria. 
----------------------------------

This next step develops the criteria to determine which candidate techniques are down selected into 
the final collection. Selection criteria should offer clear guidance when evaluating all adversarial 
risks from the compiled assets, domains and platforms. Develop guidelines for including or excluding an 
adversary activity from the threat model. Selection criteria includes virtualized infrastructure (e.g., 
virtual machines, cloud), physical technologies (e.g., identity access management servers, network), and 
operational technologies (e.g., PLC, HMI). 

Assets with adversarial risks that overlap ATT&CK for Enterprise and ATT&CK for ICS include:

* Control Servers
* Human-Machine Interfaces (HMIs)
* Jump Hosts
* Application Servers
* Engineering Workstations
* Routers in OT Networks
* Data Historians
* VPN Servers
* Firewalls

**Objective:** Establish criteria for selecting or excluding adversarial techniques based on asset relevance.

**Actions:**

* Develop Criteria

  * Provide clear guidelines for evaluating adversarial techniques.

* Identify Overlapping Techniques

  * Especially those affecting both ATT&CK for Enterprise and ICS.

* Evaluate Impact

  * Focus on feasible techniques that could impact assets or operational networks.

* Generate an initial list of adversarial techniques for each asset type in the architecture.

**Guidance:**

* Select relevant adversarial techniques for each asset.
* Exclude techniques that are N/A for each asset.
* Evaluate potential impact to ICS and operational network.

Step 4. Review applicable adversarial techniques. 
-------------------------------------------------

The fourth step determines which techniques to include in the threat collection. Review and 
evaluate adversary techniques for each asset according to previously defined criteria to curate 
the list of adversarial techniques for each asset for the final collection. Exclude any 
non-applicable techniques.

**Objective:** Curate a refined list of adversarial techniques for each asset.

**Actions:**

* Review and Curate

  * Collaborate with SMEs to review techniques.

* Document Reasoning

  * Include notes explaining the inclusion or exclusion of techniques.

* Determine Final Threat Collection

  * Determine the final set of techniques for the threat collection.

**Guidance:** 

* Include comments to explain the reasoning for the inclusion or exclusion of techniques.
 
  * These annotations are helpful later for extending, modifying, or updating the collection when the underlying architecture changes. 
  * The rationale for each technique can clarify ambiguities in the process.

Step 5. Build custom threat collection.
---------------------------------------

The final step is to assemble the techniques into a custom threat collection. Generate a tailored 
threat intelligence collection for hybrid IT/OT systems. Provide the collection in a sharable and 
extensible format, preferably a machine-readable STIX bundle, to share throughout the organization 
or externally.

**Objective:** Assemble the selected techniques into a shareable threat collection.

**Actions:**

* Assemble Techniques

  * Create a threat collection in a machine-readable format (e.g., STIX bundle).

* Share Collection

  * Distribute the threat collection throughout the organization for awareness and defense preparation.
  * Externally publish the collection to benefit the community.
    * Please see the `guidance for contributors <https://github.com/center-for-threat-informed-defense/defending-ot-with-attack/blob/main/CONTRIBUTING.md>`_ if are you interested in contributing to the Center's repository.

**Guidance:**

  * Utilize tools like the Center's `ATT&CK Workbench <https://github.com/center-for-threat-informed-defense/attack-workbench-frontend/blob/master/README.md>`_ for compilation.