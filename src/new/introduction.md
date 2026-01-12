# Introduction # {#introduction}
Some info about GDI here.

## Goals and Scope of the Harmonized Minimal Data Model

The **Harmonized Minimal Data Model (HMDM)** has multiple purposes, some of these are:
1. Each dataset that is submitted to the catalogue should adhere (to a certain extend, still to be decided upon) to this model
2. Within the catalogue based on our model search options can be made available (filters/facets)
3. The HMDM can/needs to be implemented in the Beacons (and/or other discovery tools).

Next to the HMDM we provided a **minimal metadata for submission schema**.

Version 1 of metadata for submission model was released and can be seen [here](https://drive.google.com/drive/u/0/folders/1oojXociy39DD_VzUZHfx1n4queVJD1RE). This version was based on the version of HealthDCAT-AP from December 2024. Since the work on HealthDCAT-AP is still ongoing, there have been some changes since that time. This means our metadata for submission is not compliant to the [current version of HealthDCAT-AP](https://healthdcat-ap.github.io/) anymore.
We will update the metadata for submission to version 1.1, which will be, according to HealthDCAT-AP, provided in 3 variants, based on the access level of the dataset: *Open*, *Sensitive* and *Protected*, which differ in cardinalities of the properties. The metadata for submission model will include all the current mandatory fields from those HealthDCAT-AP vairants, as well as a custom class created specifically for the submission of metadata in GDI, called HMD Submission. 
The name spaces for HMD Submission class and its properties were made available through [FAIR Genomes repository](https://github.com/fairgenomes/fairgenomes-semantic-model).
There are also some mandatory fields that were already included in the GDI MS8 deliverable, which will stay mandatory for backwards compatibility. This update will be very minimal, so only extending the current model with new mandatory fields.


## Overview and Diagram

<img src="https://raw.githubusercontent.com/Health-RI/HarmonisedMinimalDatamodel/main/src/new/images/HMD_v1.1_UML.png" alt="UML diagram">