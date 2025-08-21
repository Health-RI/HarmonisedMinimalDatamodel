## Sample

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
            <td>Anatomical sample location</td>
            <td>Anatomic site from which the sample was taken.</td>
            <td><a href="https://icd.who.int/browse/2024-01/mms/en#1154280071">ICD-11 Anatomy and topography</a></td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Pathological state</td>
            <td>The pathological condition of the sample.</td>
            <td><a href="https://ncithesaurus.nci.nih.gov/ncitbrowser/ConceptReport.jsp?dictionary=NCI_Thesaurus&ns=ncit&code=C162623">Tissue Normal</a>, Germline Normal, <a href="https://ncithesaurus.nci.nih.gov/ncitbrowser/ConceptReport.jsp?dictionary=NCI_Thesaurus&version=24.03d&ns=ncit&code=C8509">Primary Tumor</a>, <a href="https://ncithesaurus.nci.nih.gov/ncitbrowser/ConceptReport.jsp?dictionary=NCI_Thesaurus&version=24.03d&ns=ncit&code=C3261">Tumor Metastasis</a>, <a href="https://ncit.nci.nih.gov/ncitbrowser/ConceptReport.jsp?dictionary=NCI_Thesaurus&ns=ncit&code=C4798">Recurrent Tumor</a>, <a href="http://purl.obolibrary.org/obo/NCIT_C172259">Organoid</a>, <a href="https://w3id.org/fair-genomes/resource/FG_0000124">Tumoroid</a></td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Date</td>
            <td>Defines the date of sampling.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>ID</td>
            <td>Unique identifier for a collected specimen assigned by data provider.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Organism</td>
            <td>A living entity.</td>
            <td>Children of <a href="https://purl.bioontology.org/ontology/NCIT?conceptid=http%3A%2F%2Fncicb.nci.nih.gov%2Fxml%2Fowl%2FEVS%2FThesaurus.owl%23C14250">NCIT Organism</a></td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Biospecimen_Type</td>
            <td>The type of a material sample taken from a biological entity for testing, diagnostic, propagation, treatment or research purposes. This includes particular types of cellular molecules, cells, tissues, organs, body fluids, embryos, and body excretory substances.</td>
            <td>Value from type of Sample table in <a href="https://cdn.ymaws.com/www.isber.org/resource/resmgr/isber_2019/pdf/standard_preanalytical_code_.pdf">SPREC Codes v3.0 </a>:
            <br>ASC - Ascites fluid
            <br> AMN - Amniotic fluid
            <br> BAL - Bronchoalveolar lavage
            <br> BLD - Blood (whole)
            <br> BMA - Bone marrow aspirate
            <br> BMK - Breast milk
            <br> BUC - Buccal cells
            <br> BUF - Unficolled buffy coat, viable
            <br> CEL - Ficoll mononuclear cells, viable
            <br> CEN - Fresh cells from non blood specimen type
            <br> CLN - Cells from nonblood specimen type (e.g., disrupted tissue), viable
            <br> CRD - Cord blood
            <br> CSF - Cerebrospinal fluid
            <br> NAS - Nasal washing
            <br> PEL - Ficoll mononuclear cells, nonviable
            <br> PEN - Cells from nonblood specimen type (e.g., disrupted tissue), nonviable
            <br> PFL - Pleural fluid
            <br> PL1 - Plasma, single spun
            <br> PL2 - Plasma, double spun
            <br> SAL - Saliva
            <br> SEM - Semen
            <br> SER - Serum
            <br> SPT - Sputum
            <br> STL - Stool
            <br> SYN - Synovial fluid
            <br> TER - Tears
            <br> U24 - 24-h urine
            <br> URN - Urine
            <br> ZZZ Other </td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Extraction_Technique</td>
            <td>The technique of extraction of the sample.</td>
            <td>Values within <a href="https://bioportal.bioontology.org/ontologies/MESH/?p=classes&conceptid=http%3A%2F%2Fpurl.bioontology.org%2Fontology%2FMESH%2FD013048">MESH Specimen Handling</a></td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Storage_Conditions</td>
            <td>Storage conditions of the sample.</td>
            <td><a href="https://github.com/fairgenomes/fairgenomes-semantic-model/blob/main/lookups/StorageConditions.txt"> FAIR Genomes Storage Conditions</a> or <a href="https://cdn.ymaws.com/www.isber.org/resource/resmgr/isber_2019/pdf/standard_preanalytical_code_.pdf"> SPREC Codes v3.0</a></td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Assayed_Biological_Macromolecule</td>
            <td>Macromolecule derived from the sample.</td>
            <td>Children of <a href="https://www.ebi.ac.uk/ols4/ontologies/efo/classes?short_form=EFO_0004446">EFO biological macromolecule</a></td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Sampling_Intent</td>
            <td>Describes the purpose for taking the sample.</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
    </tbody>
</table>