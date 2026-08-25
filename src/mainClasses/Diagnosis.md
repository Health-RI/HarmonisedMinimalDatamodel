## Diagnosis

<table>
    <thead>
        <tr>
            <th>Item</th>
            <th>Definition</th>
            <th>Value</th>
            <th>Cardinality</th>
            <th>Condition</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C164339">Date of Diagnosis</a></td>
            <td>Date at which diagnosis was made.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td><a href="https://snomedbrowser.org/?perspective=full&conceptId1=298059007&edition=MAIN&release=&languages=en">Date of Onset</a></td>
            <td>Date of onset.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C2991">Diagnosis</a></td>
            <td>Any abnormal condition of the body or mind that causes discomfort, dysfunction, or distress to the affected person.</td>
            <td>Children of SNOMED-CT <a href="http://purl.bioontology.org/ontology/SNOMEDCT/64572001">Disease (Disorder)</a></td>
            <td>1..1 (conditional)</td>
            <td>It is mandatory to provide either Diagnosis or Provisional Diagnosis</td>
        </tr>
        <tr>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C200660">Provisional diagnosis / clinical diagnosis</a></td>
            <td>An initial diagnosis that is subject to change as new information becomes available.</td>
            <td>Children of SNOMED-CT <a href="http://purl.bioontology.org/ontology/SNOMEDCT/64572001">Disease (Disorder)</a></td>
            <td>1..1 (conditional)</td>
            <td>It is mandatory to provide either Diagnosis or Provisional Diagnosis</td>
        </tr>
        <tr>
            <td>Diagnosis_InfectiousDisease</td>
            <td>For infectious diseases, some specific diagnoses are not available in SNOMED. For these cases, the Diagnosis_InfectiousDisease item may be used.</td>
            <td><a href="https://www.ebi.ac.uk/ols4/ontologies/genepio">Genepio (epidemiology)</a></td>
            <td>0..1 (conditional)</td>
            <td>If infectious disease and specific SNOMED term is not available, Genepio may be used. May not be used if a SNOMED code is available.</td>
        </tr>
        <tr>
            <td>Provisional/clinical Diagnosis_InfectiousDisease</td>
            <td>For infectious diseases, some specific diagnoses are not available in SNOMED. For these cases, the Provisional/clinical Diagnosis_InfectiousDisease item may be used.</td>
            <td><a href="https://www.ebi.ac.uk/ols4/ontologies/genepio">Genepio (epidemiology)</a></td>
            <td>0..1 (conditional)</td>
            <td>If infectious disease and specific SNOMED term is not available, Genepio may be used. May not be used if a SNOMED code is available.</td>
        </tr>
        <tr>
            <td><a href="https://loinc.org/8656-1/">Date of hospitalization</a></td>
            <td>Date at which subject was hopitalised </td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1 (conditional)</td>
            <td>Optional for Infectious Disease</td>
        </tr>
        <tr>
            <td><a href="https://snomedbrowser.org/?perspective=full&conceptId1=284548004&edition=MAIN/2026-08-01&release=&languages=en">Clinical Department</a></td>
            <td>Refers to the Clinical Department in charge of the patient</td>
            <td>String</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Institution Clinical</td>
            <td>Institution of the clinical department in charge of the patient.</td>
            <td>String</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td><a href="https://snomedbrowser.org/?perspective=full&conceptId1=272141005&edition=MAIN&release=&languages=en">Severity Grading</a></td>
            <td>Classification scale used for severity grading</td>
            <td><a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=442452003&edition=MAIN/2025-11-01&release=&languages=en">442452003 | Life threatening severity</a> <br>
            <a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=255604002&edition=MAIN/2025-11-01&release=&languages=en">255604002 | Mild</a> <br>
            <a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=371923003&edition=MAIN/2025-11-01&release=&languages=en">371923003 | Mild to moderate</a> <br>
            <a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=6736007&edition=MAIN/2025-11-01&release=&languages=en">6736007 | Moderate</a> <br>
            <a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=371924009&edition=MAIN/2025-11-01&release=&languages=en">371924009 | Moderate to severe</a> <br>
            <a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=24484000&edition=MAIN/2025-11-01&release=&languages=en">24484000 | Severe</a> <br></td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td><a href="https://loinc.org/95367-9/">Date of transfer to an Intensive Care Unit (ICU)</a></td>
            <td>Date at which subject was transfered to an Intensive care unit. </td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1 (conditional)</td>
            <td>Recommended for Infectious Disease</td>
        </tr>
        <tr>
            <td>Date Declared Cured</td>
            <td>Date at which subject was called "cured" from the disease.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Clinical Status</td>
            <td>Indicates the status of the condition.</td>
            <td>Active<br>
                Inactive<br>
                Recurring<br>
                Remission<br>
                Relapsed</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Has Comorbidity</td>
            <td>Points to another diagnosis that acts as a comorbidity to the current diagnosis.</td>
            <td>Diagnosis class</td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Topology</td>
            <td>Describes the anatomical location of (the origin of) the disease.</td>
            <td>String</td>
            <td>1..1 (conditional)</td>
            <td>Mandatory for Infectious Disease</td>
        </tr>
        <tr>
            <td>Morphology</td>
            <td>Describes the cell type and biological activity.</td>
            <td>String</td>
            <td>1..1 (conditional)</td>
            <td>Mandatory for Infectious Disease</td>
        </tr>
    </tbody>
</table>