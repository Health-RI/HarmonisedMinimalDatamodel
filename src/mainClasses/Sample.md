## Sample

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
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C13717">Anatomical sample location</a></td>
            <td>Anatomic site from which the sample was taken.</td>
            <td>ICD-11 <a href="https://icd.who.int/browse/2024-01/mms/en#1154280071">Anatomy and topography</a></td>
            <td>1..1 (conditional)</td>
            <td>In use case cancer, the exact sample location is relevant; therefore the more detailed value list of ICD-O3 can be used (which is included in ICD-11)</td>
        </tr>
        <tr>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C19697">Pathological state</a></td>
            <td>The pathological condition of the sample.</td>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C162623">Tissue Normal</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C94480">Germline DNA</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C8509">Primary Tumor</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C3261">Tumor Metastasis</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C4798">Recurrent Tumor</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C172259">Organoid</a>, <a href="https://w3id.org/fair-genomes/resource/FG_0000124">Tumoroid</a></td>
            <td>1..1 (conditional)</td>
            <td>In cancer use case, the pathological state of the sample must be recorded; several instances of the sample class can be filled if matching samples of different pathological states (normal, primary tumor,...) are present.</td>
        </tr>
        <tr>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C25164">Date of Sampling</a></td>
            <td>Defines the date of sampling.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>ID</td>
            <td>Unique identifier for a collected specimen assigned by data provider.</td>
            <td>String</td>
            <td>1..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C14250">Organism</a></td>
            <td>A living entity.</td>
            <td>Children of <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C14250">NCIT Organism</a></td>
            <td>1..1</td>
            <td>If Organism is for example "Virus" then Biospecimen_Type should not be something like "tissue"</td>
        </tr>
        <tr>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C70713">Biospecimen Type</a></td>
            <td>The type of a material sample taken from a biological entity for testing, diagnostic, propagation, treatment or research purposes. This includes particular types of cellular molecules, cells, tissues, organs, body fluids, embryos, and body excretory substances.</td>
            <td><br><a href="http://purl.obolibrary.org/obo/NCIT_C17610">Blood</a>
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C84507">Buffy coat</a>
            <br><a href="http://purl.obolibrary.org/obo/NCIT_C20313">Cancer cell lines</a>
            <br><a href="https://snomedbrowser.org/?perspective=full&conceptId1=272625005&edition=MAIN&release=&languages=en">Entire body organ</a>
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
            <td>For Cancer use case, and for the Infectious disease use case, this field is mandatory, otherwise optional.</td>
        </tr>
        <tr>
            <td>Extraction Technique</td>
            <td>The technique of extraction of the sample.</td>
            <td><a href="#protocol">Protocol class</a></td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Storage Conditions</td>
            <td>Storage conditions of the sample.</td>
            <td><a href="https://github.com/fairgenomes/fairgenomes-semantic-model/blob/main/lookups/StorageConditions.txt"> FAIR Genomes Storage Conditions</a></td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Assayed Biological Macromolecule</td>
            <td>Macromolecule derived from the sample.</td>
            <td>Children of <a href="http://www.ebi.ac.uk/efo/EFO_0004446">EFO biological macromolecule</a></td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td><a href="https://ncit.nci.nih.gov/ncitbrowser/ConceptReport.jsp?dictionary=NCI_Thesaurus&version=24.06d&ns=ncit&code=C25725&key=645876995&b=1&n=null">Sampling Intent</a></td>
            <td>Describes the purpose for taking the sample.</td>
            <td>String</td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Sampling Place</td>
            <td>Defines the geographic location of sampling</td>
            <td><a href="#geolocation">GeoLocation class</a></td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Sample Diagnosis</td>
            <td>Diagnosis established based on sample.</td>
            <td><a href="#diagnosis">Diagnosis class</a></td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Sample Relation</td>
            <td>Establishes the relation with another sample.</td>
            <td><a href="#sample-relation">Sample Relation class</a></td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Sample TNM</td>
            <td>TNM classification of the sample.</td>
            <td><a href="#tnm">TNM class</a></td>
            <td>0..2(conditional)</td>
            <td>Recommended for Cancer use case.</td>
        </tr>
        <tr>
            <td>Sample Genotyping</td>
            <td>Establishes the relation with Genotyping class.</td>
            <td><a href="#genotyping">Genotyping class</a></td>
            <td>1..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Subject</td>
            <td>Establishes the relation with the subject.</td>
            <td><a href="#subject">Subject class</a></td>
            <td>1..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Sample Provenance</td>
            <td>Establishes the relation with provenance class.</td>
            <td><a href="#data-provenance">Data Provenance class</a></td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Test</td>
            <td>Establishes the relation with Test class.</td>
            <td><a href="#test">Test class</a></td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
    </tbody>
</table>