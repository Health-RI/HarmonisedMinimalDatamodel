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
            <td>373808002 | Curative - procedure intent
            <br>373847000 | Neoadjuvant intent
            <br>373846009 | Adjuvant - intent
            <br>363676003 | Palliative - procedure intent
            <br>360271000 | Prophylaxis - procedure intent
            <br>243114000 | Support (regime/therapy)
            <br>129304002 | Excision - action 
            <br>261004008 | Diagnostic intent
            <br>129428001 | Preventive - intent
            <br>429892002 | Guidance intent
            <br>360156006 | Screening - procedure intent
            <br>447295008 | Forensic intent
            <br>Other - HL7 NULL flavor (OTH, UNK, NI, NA)</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Setting</td>
            <td>Indicate the treatment setting, which describes the treatment's purpose in relation to the primary treatment (Reference: NCIT C124308)</td>
            <td><a href="https://bioportal.bioontology.org/ontologies/NCIT?p=classes&conceptid=http%3A%2F%2Fncicb.nci.nih.gov%2Fxml%2Fowl%2FEVS%2FThesaurus.owl%23C15675">Adjuvant</a> <br> <a href="https://w3id.org/fair-genomes/resource/FG_0000760">Advanced/Metastatic</a><br> <a href="https://bioportal.bioontology.org/ontologies/NCIT?p=classes&conceptid=http%3A%2F%2Fncicb.nci.nih.gov%2Fxml%2Fowl%2FEVS%2FThesaurus.owl%23C15665">Neoadjuvant</a><br> <a href="https://terminology.hl7.org/5.1.0/CodeSystem-v3-NullFlavor.html#v3-NullFlavor-NA">Not applicable</a></td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Type</td>
            <td>Indicates the type of treatment regimen that the patient completed; coded values can be chosen, SNOMED may be chosen for "procedures".</td>
            <td>23719005 | Bone marrow transplant
            <br>367336001 | Chemotherapy
            <br>18629005 | Medication
            <br>423827005 | Endoscopic therapy
            <br>169413002 | Hormonal therapy
            <br>76334006 | Immunotherapy
            <br>257891001 | Photodynamic therapy
            <br>1287742003 | Radiation therapy
            <br>56305001 | Radionucleotide therapy
            <br>1269349006 | Stem cell transplant
            <br>387713003 | Surgery
            <br>394613000 | Gene therapy
            <br>310341009 or 373818007 | Watchful waiting
            <br>424313000 | Active follow-up
            <br>703423002 | Chemoradiotherapy
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
            <td>Treatment Code</td>
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
            <td>Subclass of <a href="http://purl.obolibrary.org/obo/NCIT_C13442">Anatomy qualifier</a></td>
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
            <td><a href="http://snomed.info/id/71388002">SNOMED Procedures</a></td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Surgical resection quality</td>
            <td>Evaluation of the surgical resection quality based on coded values.</td>
            <td>1222638005 |American Joint Committee on Cancer R0 (qualifier value)
            <br>1222639002 | American Joint Committee on Cancer R1 (qualifier value)
            <br>1222640000 | American Joint Committee on Cancer R2 (qualifier value)
            <br>1222641001 | American Joint Committee on Cancer RX (qualifier value)</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Treatment_Status</td>
            <td>Indicates the patient's outcome of the prescribed treatment (coded values, e.g. treatment not completed | because of toxicity).</td>
            <td>182992009 | Treatment completed (situation)
            <br>445528004 | Treatment changed (situation)
            <br>405613005 | Planned procedure (situation)
            <br>416406003 | Procedure discontinued (situation)</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Reason_for_incomplete_Treatment</td>
            <td>Reason for discontinuation of the treatment.</td>
            <td>419099009 | Dead (finding)
            <br>1296859006 | Procedure declined (situation)   
            <br>713247000 | Procedure discontinued by patient (situation)
            <br>713246009 | Procedure discontinued by healthcare professional (situation) 
            <br>266721009 | Absent response to treatment (situation)       
            <br>407563006 | Treatment not tolerated (situation) 
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
            <td>Children of <a href="https://bioportal.bioontology.org/ontologies/NCIT?p=classes&conceptid=http%3A%2F%2Fncicb.nci.nih.gov%2Fxml%2Fowl%2FEVS%2FThesaurus.owl%23C27990">Toxicity (NCIT)</a></td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Modality</td>
            <td>Indicates the method of radiation treatment or modality.</td>
            <td><a href="https://bioportal.bioontology.org/ontologies/NCIT/?p=classes&lang=en&conceptid=http%3A%2F%2Fncicb.nci.nih.gov%2Fxml%2Fowl%2FEVS%2FThesaurus.owl%23C15650&jump_to_nav=true">Electron</a> <br> <a href="https://bioportal.bioontology.org/ontologies/NCIT/?p=classes&lang=en&conceptid=http%3A%2F%2Fncicb.nci.nih.gov%2Fxml%2Fowl%2FEVS%2FThesaurus.owl%23C15458&jump_to_nav=true">Heavy Ions</a> <br> <a href="https://bioportal.bioontology.org/ontologies/NCIT?p=classes&conceptid=http%3A%2F%2Fncicb.nci.nih.gov%2Fxml%2Fowl%2FEVS%2FThesaurus.owl%23C93337">Photon</a> <br> <a href="https://bioportal.bioontology.org/ontologies/NCIT/?p=classes&lang=en&conceptid=http%3A%2F%2Fncicb.nci.nih.gov%2Fxml%2Fowl%2FEVS%2FThesaurus.owl%23C66897&jump_to_nav=true">Proton</a></td>
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
            <td>Children concepts of <a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=91723000&edition=MAIN&release=&languages=en">Anatomical Structure (body structure)</a></td>
            <td>0..n</td>
        </tr>
    </tbody>
</table>