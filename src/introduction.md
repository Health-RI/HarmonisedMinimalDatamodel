# Introduction # {#introduction}
## About GDI

The Genomic Data Infrastructure (GDI) is a European project, co-funded under the Digital Europe Programme, designed to realize the ambition of the 1+ Million Genomes (1+MG) initiative.
Our primary goal is to establish a federated, sustainable, and secure infrastructure to enable cross-border access to human genomic, phenotypic, and clinical data across Europe. By providing this infrastructure, we aim to unlock the potential of genomic data to drive breakthroughs in medical research, advance personalized healthcare, and inform public health policymaking.
You can visit https://gdi.onemilliongenomes.eu/ for more information about the project.

## About the Harmonized Minimal Data Model for GDI
Within the GDI project, deliverable 8.2 encapsulates the collaborative efforts of GDI, 1+MG, Genome of Europe, B1MG(plus) and ERDERA initiatives towards establishing harmonised minimal data models and specifications for genomic data exchange and integration. Establishing harmonised minimal data models (i.e. a blueprint that shows how data is organized and connected) and specifications within GDI facilitates seamless data exchange, supporting better collaboration in healthcare and contributing to improved patient care. Efforts focused on leveraging prior work from 1+MG and B1MG initiatives to define minimal datasets for GDI use cases, particularly in Cancer, Infectious Diseases, Rare Diseases and the Genome of Europe.
This page outlines the content of the Harmonized minimal data model for GDI.

## Goals and Scope of the Harmonized Minimal Data Model

The **Harmonized Minimal Data Model (HMD)** has multiple purposes, some of these are:
1. Each dataset that is submitted to the catalogue should adhere (to a certain extend, still to be decided upon) to this model
2. Within the catalogue based on our model search options can be made available (filters/facets)
3. The HMD can/needs to be implemented in the Beacons (and/or other discovery tools).

## Overview and Diagram

In the diagram below, you can view the complete HMD.
Each box within the diagram comprises one of the classes of the model. Within each box, you find all concepts of the respective class.
Red boxes represent mandatory classes. The remaining classes (green boxes) are optional and usage of these classes depends on each case.
For example, for data of healthy subjects, the diagnosis class will not be used, but there always needs to be information about the Subject, Sample, Genotyping and Consent.

The connections between the classes indicate the relations between classes. For example, Subject is connected to the Sample class via the hasSample concept.

<img src="src/images/GDI_diagram-v2.0 UML Diagram 1+MG GDI.drawio.png" alt="UML diagram" width=1200>