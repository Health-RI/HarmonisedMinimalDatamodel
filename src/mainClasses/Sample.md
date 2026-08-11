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
            <td>ICD-11 <a href="https://icd.who.int/browse/2024-01/mms/en#1154280071">Anatomy and topography</a></td>
            <td>1..1 (conditional)</td>
        </tr>
        <tr>
            <td>Pathological state</td>
            <td>The pathological condition of the sample.</td>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C162623">Tissue Normal</a>, Germline Normal, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C8509">Primary Tumor</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C3261">Tumor Metastasis</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C4798">Recurrent Tumor</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C172259">Organoid</a>, <a href="https://w3id.org/fair-genomes/resource/FG_0000124">Tumoroid</a></td>
            <td>1..1 (conditional)</td>
        </tr>
        <tr>
            <td>Date of Sampling</td>
            <td>Defines the date of sampling.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>ID</td>
            <td>Unique identifier for a collected specimen assigned by data provider.</td>
            <td>String</td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Organism</td>
            <td>A living entity.</td>
            <td>Children of <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C14250">NCIT Organism</a></td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Biospecimen_Type</td>
            <td>The type of a material sample taken from a biological entity for testing, diagnostic, propagation, treatment or research purposes. This includes particular types of cellular molecules, cells, tissues, organs, body fluids, embryos, and body excretory substances.</td>
            <td><br><a href="http://purl.obolibrary.org/obo/NCIT_C17610">Blood</a>
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C84507">Buffy coat</a>
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C20313">Cancer cell lines</a>
            <br> Entire body organ
            <br><a href="http://purl.obolibrary.org/obo/OMIABIS_0001076">Faeces</a>
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C17730">Embryo or fetal tissue</a>
            <br> Immortalized cell lines
            <br> Isolated microbes
            <br> Other body fluid
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C185204">Plasma</a>
            <br> Primary cells
            <br><a href="http://purl.obolibrary.org/obo/OBI_0000902">Post-mortem tissue</a>
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C174119">Saliva</a>
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C178987">Serum</a>
            <br><a href="http://purl.obolibrary.org/obo/OBI_0600012">Specimen from environment or food: environmental collection</a>
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C150895">Swab</a>
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C158417">Tissue (Frozen)</a>
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C172265">Tissue (FFPE)</a>
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C189126">Urine</a>
            <br><a href="https://terminology.hl7.org/en/CodeSystem-v3-NullFlavor.html#v3-NullFlavor-OTHOther">Other</a></td>
            <td>1..1 (conditional)</td>
        </tr>
        <tr>
            <td>Extraction_Technique</td>
            <td>The technique of extraction of the sample.</td>
            <td>Protocol class</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Storage_Conditions</td>
            <td>Storage conditions of the sample.</td>
            <td><a href="https://github.com/fairgenomes/fairgenomes-semantic-model/blob/main/lookups/StorageConditions.txt"> FAIR Genomes Storage Conditions</a></td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Assayed_Biological_Macromolecule</td>
            <td>Macromolecule derived from the sample.</td>
            <td>Children of <a href="http://www.ebi.ac.uk/efo/EFO_0004446">EFO biological macromolecule</a></td>
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