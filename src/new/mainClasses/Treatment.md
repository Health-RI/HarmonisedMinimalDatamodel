## Treatment

<table>
    <thead>
        <tr>
            <th>Item</th>
            <th>Definition</th>
            <th>Value</th>
            <th>Cardinality</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Intention_to_Treat</td>
            <td>Indicate the intended disease outcome for which the treatment is given, may be coded as SNOMED-CT.</td>
            <td><a href="http://purl.bioontology.org/ontology/SNOMEDCT/373808002">SCTID: 373808002</a> | Curative - procedure intent
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/373847000">SCTID: 373847000</a> | Neoadjuvant intent
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/373846009">SCTID: 373846009</a> | Adjuvant - intent
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/363676003">SCTID: 363676003</a> | Palliative - procedure intent
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/360271000">SCTID: 360271000</a> | Prophylaxis - procedure intent
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/243114000">SCTID: 243114000</a> | Support (regime/therapy)
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/129304002">SCTID: 129304002</a> | Excision - action 
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/261004008">SCTID: 261004008</a> | Diagnostic intent
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/129428001">SCTID: 129428001</a> | Preventive - intent
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/429892002">SCTID: 429892002</a> | Guidance intent
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/360156006">SCTID: 360156006</a> | Screening - procedure intent
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/447295008">SCTID: 447295008</a> | Forensic intent
            <br>Other - HL7 NULL flavor (OTH, UNK, NI, NA)</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Setting</td>
            <td>Indicate the treatment setting, which describes the treatment's purpose in relation to the primary treatment (Reference: NCIT C124308)</td>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C15675">Adjuvant</a> <br> <a href="https://w3id.org/fair-genomes/resource/FG_0000760">Advanced/Metastatic</a><br> <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C15665">Neoadjuvant</a><br> <a href="https://terminology.hl7.org/5.1.0/CodeSystem-v3-NullFlavor.html#v3-NullFlavor-NA">Not applicable</a></td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Type</td>
            <td>Indicates the type of treatment regimen that the patient completed; coded values can be chosen, SNOMED may be chosen for "procedures".</td>
            <td><a href="http://purl.bioontology.org/ontology/SNOMEDCT/23719005">SCTID: 23719005</a> | Bone marrow transplant
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/367336001">SCTID: 367336001</a> | Chemotherapy
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/18629005">SCTID: 18629005</a> | Medication
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/423827005">SCTID: 423827005</a> | Endoscopic therapy
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/169413002">SCTID: 169413002</a> | Hormonal therapy
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/76334006">SCTID: 76334006</a> | Immunotherapy
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/257891001">SCTID: 257891001</a> | Photodynamic therapy
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/1287742003">SCTID: 1287742003</a> | Radiation therapy
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/56305001">SCTID: 56305001</a> | Radionucleotide therapy
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/1269349006">SCTID: 1269349006</a> | Stem cell transplant
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/387713003">SCTID: 387713003</a> | Surgery
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/394613000">SCTID: 394613000</a> | Gene therapy
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/310341009">SCTID: 310341009</a> or 373818007 | Watchful waiting
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/424313000">SCTID: 424313000</a> | Active follow-up
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/703423002">SCTID: 703423002</a> | Chemoradiotherapy
            <br>HL7 NULL flavor (NI, NA, OTH) | Other</td>
            <td>1..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Subtype</td>
            <td>Detailed specification of the treatment type.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Line</td>
            <td>Indicate if the treatment was the primary treatment following the initial diagnosis or 2nd, 3rd, …</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>treatmentCode</td>
            <td>A drug product that contains one or more active and/or inactive ingredients used by the patient intended to treat, prevent or alleviate the symptoms of disease. Any hormone therapies, gender-related or otherwise, should also be recorded here.</td>
            <td><a href="https://raw.githubusercontent.com/fairgenomes/fairgenomes-semantic-model/main/lookups/Drugs.txt">ATC codes</a>, IDMP when available. <br> In case of Cancer: <a href="https://hemonc.org/wiki/Main_Page">HEMONC</a>, <a href="https://mor.nlm.nih.gov/RxClass/">RxNorm</a></td>
            <td>1..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Date_start_overall</td>
            <td>The date and time of (the start of) the treatment.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Date_end_overall</td>
            <td>The date and time of the end of the overall treatment.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Intended Duration</td>
            <td>The duration of treatment regimen, in days.</td>
            <td>Integer</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>DoseUnits</td>
            <td>Indicates the total dose given in units (e.g. of Gray (Gy) when radiation, Millimeters/24hours for medication).</td>
            <td>Choicelist with most common DoseUnits, like Gray, Milligrams/24 hours: make use of <a href="https://ucum.org/">UCUM</a>.</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>cumulativeDose</td>
            <td>The amount of any substance administered over a specific period of time.</td>
            <td>Float</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>doseIntervals</td>
            <td>The number of times a substance is administered within a specific time period.</td>
            <td>ISO8601 Period</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>routeOfAdministration</td>
            <td>Designation of the part of the body through which or into which, or the way in which, the medicinal product is intended to be introduced. In some cases a medicinal product can be intended for more than one route and/or method of administration.</td>
            <td>Subclass of <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C13442">Anatomy qualifier</a></td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Pre-Treated</td>
            <td>Indicates if disease has been pre-treated or is in course of treatment.</td>
            <td>Boolean</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Procedures</td>
            <td>Indicates the type of treatment regimen that the patient completed; coded values can be chosen, SNOMED may be chosen for "procedures".</td>
            <td><a href="http://purl.bioontology.org/ontology/SNOMEDCT/71388002">SNOMED Procedure</a></td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Surgical resection quality</td>
            <td>Evaluation of the surgical resection quality based on coded values.</td>
            <td><a href="http://purl.bioontology.org/ontology/SNOMEDCT/1222638005">SCTID: 1222638005</a> |American Joint Committee on Cancer R0 (qualifier value)
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/1222639002">SCTID: 1222639002</a> | American Joint Committee on Cancer R1 (qualifier value)
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/1222640000">SCTID: 1222640000</a> | American Joint Committee on Cancer R2 (qualifier value)
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/1222641001">SCTID: 1222641001</a> | American Joint Committee on Cancer RX (qualifier value)</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Treatment_Status</td>
            <td>Indicates the patient's outcome of the prescribed treatment (coded values, e.g. treatment not completed | because of toxicity).</td>
            <td><a href="http://purl.bioontology.org/ontology/SNOMEDCT/182992009">SCTID: 182992009</a> | Treatment completed (situation)
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/445528004">SCTID: 445528004</a> | Treatment changed (situation)
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/405613005">SCTID: 405613005</a> | Planned procedure (situation)
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/416406003">SCTID: 416406003</a> | Procedure discontinued (situation)</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Reason_for_incomplete_Treatment</td>
            <td>Reason for discontinuation of the treatment.</td>
            <td><a href="http://purl.bioontology.org/ontology/SNOMEDCT/419099009">SCTID: 419099009</a> | Dead (finding)
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/1296859006">SCTID: 1296859006</a> | Procedure declined (situation)   
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/713247000">SCTID: 713247000</a> | Procedure discontinued by patient (situation)
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/713246009">SCTID: 713246009</a> | Procedure discontinued by healthcare professional (situation) 
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/266721009">SCTID: 266721009</a> | Absent response to treatment (situation)       
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/407563006">SCTID: 407563006</a> | Treatment not tolerated (situation) 
            <br>technical or organizational problems | to be added, or use OTH 
            <br>Other | HL7 null flavour OTH      
            <br>Not applicable | HL7 null flavour, NA
            <br>No information | HL7 null flavour, NI</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Response_to_Treatment</td>
            <td>The patients' response to the applied treatment regimen. (Source: RECIST).</td>
            <td><a href="https://w3id.org/fair-genomes/resource/FG_0000761">Complete Response</a> <br>
            <a href="https://w3id.org/fair-genomes/resource/FG_0000762">Disease progression</a> <br>
            <a href="https://w3id.org/fair-genomes/resource/FG_0000763">NED</a> <br>
            <a href="https://w3id.org/fair-genomes/resource/FG_0000764">Partial Response</a> <br>
            <a href="https://w3id.org/fair-genomes/resource/FG_0000765">Stable Disease</a></td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Adverse_Events</td>
            <td>Reports any treatment related adverse events. (Codelist reference: NCI-CTCAE (v5.0))</td>
            <td><a href="https://ctep.cancer.gov/protocoldevelopment/electronic_applications/docs/CTCAE_v5_Quick_Reference_5x7.pdf">CTCAE Codes</a></td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Toxicity_Type</td>
            <td>If the treatment was terminated early due to acute toxicity, indicates the type of toxicity that caused early termination of treatment.</td>
            <td>Children of <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C27990">Toxicity (NCIT)</a></td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Modality</td>
            <td>Indicates the method of radiation treatment or modality.</td>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C15650">Electron</a> <br> <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C15458">Heavy Ions</a> <br> <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C93337">Photon</a> <br> <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C66897">Proton</a></td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Fractions</td>
            <td>Indicates the total number of fractions delivered as part of radiation treatment.</td>
            <td>Integer</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Site</td>
            <td>Indicates the body region where radiation therapy was administered.</td>
            <td>Children concepts of <a href="http://purl.bioontology.org/ontology/SNOMEDCT/91723000">Anatomical Structure (body structure)</a></td>
            <td>0..n</td>
        </tr>
    </tbody>
</table>