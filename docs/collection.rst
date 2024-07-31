Threat Collection
=================

The Defending OT with ATT&CK threat collection is a customized collection of MITRE
ATT&CK® techniques tailored to the attack surface and threat model for OT environments.
Historical attacks against OT and adversarial tactics, techniques, and procedures (TTPs)
as contained in ATT&CK for Enterprise, ATT&CK for ICS, and other relevant ATT&CK
datasets such as Cloud and Containers were analyzed to identify and define a reference
architecture and technology domains of interest specific to OT. The resultant collection
can be used by organizations that use OT to evaluate, plan, and employ security controls
based on known, real-world adversary behaviors targeting those environments.

Defending OT with ATT&CK provides a defined threat collection to assist defenders in
understanding which techniques adversaries could use within an IT/OT hybrid
architecture. This includes:

* Techniques that occur on enterprise system.
* Techniques on Industrial Control Systems (ICS), and
* Techniques on OT assets that run similar operating systems, protocols, and applications as enterprise IT assets.

The project team applied the :doc:`methodology` and employed the flexibility and customization
provided by ATT&CK Workbench to develop this collection of specific adversarial risks associated
with the 21 Defending OT with ATT&CK :doc:`architecture` assets. The resultant threat collection
contains a combined 692 techniques from ATT&CK for Enterprise and ATT&CK for ICS (251 techniques
and 441 sub-techniques).

Download the Threat Collection
------------------------------
.. raw:: html

    <p>
        <a class="btn btn-primary" target="_blank" href="..\modified_work_bench_file.json" download="modified_work_bench_file.json">
        <i class="fa fa-download"></i> Download ATT&CK Workbench Collection (6.2mb)</a>
    </p>
    <p>
        <a class="btn btn-primary" target="_blank" href="..\hybrid_att&ck_matrix.xlsx" download="hybrid_att&ck_matrix.xlsx">
        <i class="fa fa-download"></i> Download Hybrid ATT&CK Matrix - EXCEL (32kb)</a>
    </p>
    <p>
        <a class="btn btn-primary" target="_blank" href="..\defending-ot-with-att&ck-0.3.json" download="defending-ot-with-att&ck-0.3.json">
        <i class="fa fa-download"></i> Download JSON Threat Collection (8.875mb)</a>
    </p>

Building the Threat Collection
------------------------------

Defending OT with ATT&CK builds upon prior work developed by the Center, including
`Defending IaaS with ATT&CK
<https://mitre-engenuity.org/cybersecurity/center-for-threat-informed-defense/our-work/defending-iaas-with-attack/>`__
and `ATT&CK Workbench
<https://github.com/center-for-threat-informed-defense/attack-workbench-frontend/blob/master/README.md>`_.

**Defending IaaS with ATT&CK**

Defending OT with ATT&CK uses the methodology and tooling created as part of the
Center's `Defending IaaS with ATT&CK project
<https://center-for-threat-informed-defense.github.io/defending-iaas-with-attack/>`__ as
a basis. The Defending IaaS project methodology provides steps to identify and select
techniques across multiple ATT&CK matrices that align to a defined attack surface,
proving to be a solid foundation for developing Defending OT project resources,
including the threat collection.

The Center developed Defending IaaS With ATT&CK project to provide the community with a
collection of MITRE ATT&CK® techniques tailored to the unique attack surface and threat model
for Infrastructure-as-a-Service (IaaS). This collection can be used to plan and evaluate security
controls for organizations that use IaaS based on the known adversary behaviors described by ATT&CK.

**ATT&CK Workbench**

The Defending OT with ATT&CK project team used `ATT&CK Workbench <https://github.com/center-for-threat-informed-defense/attack-workbench-frontend/blob/master/README.md>`_ to explore and map adversarial
techniques, target assets, and campaigns. The team employed ATT&CK Workbench's search and
filter features for ATT&CK for Enterprise and ATT&CK for ICS domains, determined mapping of
assets to multi-domains from ATT&CK for Enterprise and ATT&CK for ICS techniques, and added
rationale in Workbench's note sections, to generate the shared mapping file.

The Center created ATT&CK Workbench to enable users to explore, create, annotate, and share
extensions of MITRE ATT&CK®. ATT&CK Workbench allows users to manage and extend their own
local version of ATT&CK and keep it synchronized with the ATT&CK knowledge base. ATT&CK Workbench
is an open source tool publicly available on `GitHub <https://github.com/center-for-threat-informed-defense/attack-workbench-frontend>`_.

ATT&CK Workbench enables a number of important use cases within the ATT&CK community, such as:

* **Cyber Threat Intelligence:** Take notes on techniques, groups, and other objects to collaborate within a threat intelligence team.

* **Red Teaming:** Track and manage coverage of Red Team engagements the same way you track your ATT&CK coverage.

* **Defensive Planning:** Stay up to date with the evolving threat landscape by downloading new releases of ATT&CK automatically.

* **Collaboration with ATT&CK and the community:** Share your custom datasets with the ATT&CK community and download datasets created by others.

Defending OT with ATT&CK builds upon the methodology from `Defending IaaS with ATT&CK
<https://center-for-threat-informed-defense.github.io/defending-iaas-with-attack/>`_ and
the tools from `ATT&CK Workbench
<https://github.com/center-for-threat-informed-defense/attack-workbench-frontend/blob/master/README.md>`_,
which are prior Center projects. The Defending IAAS methodology provides steps to
identify and select techniques across multiple ATT&CK matrices that align to a defined
attack surface, proving to be a solid foundation for developing Defending OT project
resources.

ATT&CK Workbench is a platform to explore and map adversarial techniques, target assets,
and campaigns. The Defending OT project employed ATT&CK Workbench's search and filter
features for ATT&CK for Enterprise and ATT&CK for ICS domains, determined mapping of
assets to multi-domains from ATT&CK for Enterprise and ATT&CK for ICS techniques, and
added rationale in Workbench's note sections, to generate the shared mapping file.
ATT&CK Workbench enables a number of important use cases within the ATT&CK community,
such as:

* **Cyber Threat Intelligence:** Take notes on techniques, groups, and other objects to
  collaborate within a threat intelligence team.
* **Red Teaming:** Track and manage coverage of Red Team engagements the same way you
  track your ATT&CK coverage.
* **Defensive Planning:** Stay up to date with the evolving threat landscape by
  downloading new releases of ATT&CK automatically.
* **Collaboration with ATT&CK and the community:** Share your custom datasets with the
  ATT&CK community and download datasets created by others.
