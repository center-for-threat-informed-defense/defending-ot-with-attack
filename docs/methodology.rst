Threat Model Methodology
========================

This project used a structured approach to ensure a thorough analysis and documentation of 
potential adversarial techniques, tailored to the specific assets and architecture of the 
organization. By following these steps, organizations can effectively delineate their attack 
surface, compile relevant threat intelligence, apply rigorous selection criteria, and build 
a comprehensive threat collection to bolster their cybersecurity defenses.

Step 1. Identify the attack surface.
   Determine the relevant technologies where a threat actor can impact operations and 
   generate a reference architecture that depicts technologies in scope for a hybrid 
   IT/OT system.
   
   **Objective:**  Define the system components, technological assets, and user archetypes that 
   form the architecture's attack surface.
   
   **Actions:**

   * Identify System Components and Enumerate Technologies
     
     * Determine the scope of the systems, including enterprise IT platforms and ICS, by listing the assets and technologies involved (e.g., Hardware, Network, Operating Systems, Applications, Cloud services, Containers, etc.).
   
   * Categorize Reference Architecture Assets
   
     * Categorize total assets, identifying key assets with known adversarial risks from IT/OT perspectives.

   Example Assets:

   * Servers and Endpoints: Control Server, Programmable Logic Controller, Application Server
   * Identity and Access Management: Azure AD/Entra ID
   * Networking Components: Routers, Switches, Firewalls
   * ICS Assets: Human-Machine Interface, Safety Controllers, Data Gateway

To learn more about assets, visist :ref:

Step 2. Compile source information.
   
   Gather information resources and applicable cyber threat intelligence including ATT&CK 
   adversary behavior used to target the identified IT/OT systems.

   **Objective:** Gather relevant cyber threat intelligence (CTI) sources to identify potential adversarial techniques for each listed asset.

   **Actions:**

   * Consult CTI Sources

     * Use sources like MITRE's ATT&CK for Enterprise and ICS.

   * Generate Comprehensive List

     * Combine adversarial techniques relevant to each type of asset.

   * Categorize Techniques

     * Based on asset types such as ICS, Linux, Cloud (e.g., IaaS, SaaS), Containers, Windows, Azure AD, and Network.

Key Focus Areas:
* Industrial Control Systems (ICS)
* Operating Systems (Linux, Windows)
* Cloud Services (AWS, Azure, GCP)
* Containers
* Identity Management (Azure AD)

Step 3. Define selection criteria. 
   
   Develop guidelines including or excluding an adversary activity from the threat model. 
   Selection criteria includes virtualized infrastructure (e.g., virtual machines, cloud), 
   physical technologies (e.g., identity access management servers, network), and operational 
   technologies (e.g., PLC, HMI).

**Objective:** Establish criteria for selecting or excluding adversarial techniques based on asset relevance.

**Actions:**

* Develop Criteria

  * Provide clear guidelines for evaluating adversarial techniques.

* Identify Overlapping Techniques

  * Especially those affecting both ATT&CK for Enterprise and ICS.

* Evaluate Impact

  * Focus on feasible techniques that could impact assets or operational networks.

Assets with adversarial risks that overlap ATT&CK for Enterprise and ATT&CK for ICS include:

* Control Servers
* HMIs
* Jump Hosts
* Application Servers
* Engineering Workstations
* Routers in OT Networks
* Data Historians
* VPN Servers
* Firewalls

Guidance:

* Select relevant CTI sources, based on asset features.
* Exclude non-applicable techniques for each asset.
* Evaluate the impact of the techniques by identifying those that could cause significant disruption.
* Compile an initial list of applicable ATT&CK techniques for each asset.

Step 4. Review applicable adversarial techniques. 
   
   Review and evaluate adversary techniques for each asset according to previously defined 
   criteria. Exclude non-applicable techniques.

**Objective:**

Curate a refined list of adversarial techniques for each asset.

**Actions:**

* Review and Curate

  * Collaborate with SMEs to review techniques.

* Document Reasoning

  * Include notes explaining the inclusion or exclusion of techniques.

* Determine Final Threat Collection

  * Determine the final set of techniques for the collection.

Step 5. Build custom threat collection. 
   Generate a tailored threat intelligence collection for hybrid IT/OT systems. Provide 
   the collection in a sharable and extensible format.

**Objective:**
Assemble the selected techniques into a shareable threat collection.

**Actions:**

* Assemble Techniques

  * Create a threat collection in a machine-readable format (e.g., STIX bundle).

* Use ATT&CK Workbench

  * Utilize tools like the Center's ATT&CK Workbench for compilation.

* Share Collection

  * Distribute the threat collection throughout the organization for awareness and defense preparation.