### TNM

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
            <td>Tumor_size</td>
            <td>Indicates the size of the primary tumor.</td>
            <td>Double</td>
            <td>0..1</td>
        </tr>
    <tbody>
        <tr>
            <td>Tumor_size_unit</td>
            <td>Indicates the unit in which tumor size is stated.</td>
            <td><a href="https://ucum.org/">UCUM</a></td>
            <td>0..1</td>
        </tr>
    <tbody>
        <tr>
            <td>Lymph_Node_Status</td>
            <td>Indicates lymph node involvement according to the international TNM classification for solid tumors.</td>
            <td>Children of <a href="http://purl.bioontology.org/ontology/SNOMEDCT/1279504008">SCTID: 1279504008</a>  | American Joint Committee on Cancer ycN category allowable value (qualifier value)</td>
            <td>0..1</td>
        </tr>
    <tbody>
        <tr>
            <td>Metastases</td>
            <td>Indicates presence or absence of metastasis according to the international TNM classification for solid tumors.</td>
            <td>Children of <a href="http://purl.bioontology.org/ontology/SNOMEDCT/1222587001">SCTID: 1222587001 </a> | American Joint Committee on Cancer pathological M category allowable value (qualifier value), <br> or <br> Children of <a href="http://purl.bioontology.org/ontology/SNOMEDCT/1222591006">SCTID: 1222591006 </a> | American Joint Committee on Cancer clinical M category allowable value (qualifier value), <br> or HL7 NULL flavor in case not determined.</td>
            <td>0..1</td>
        </tr>
    <tbody>
        <tr>
            <td>Version</td>
            <td>Version of the TNM classification.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    <tbody>
        <tr>
            <td>Stage</td>
            <td>The extent of a cancer in the body. Staging is usually based on the size of the tumor, whether lymph nodes contain cancer, and whether the cancer has spread from the original site to other parts of the body.</td>
            <td>Children of
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/1222592004">SCTID: 1222592004</a> |  American Joint Committee on Cancer clinical stage group allowable value (qualifier value), <br> or <br>
            <a href="http://purl.bioontology.org/ontology/SNOMEDCT/1222593009">SCTID: 1222593009</a> | American Joint Committee on Cancer pathological stage group allowable value (qualifier value),<br> or
            <br> <a href="http://purl.bioontology.org/ontology/SNOMEDCT/1222594003">SCTID: 1222594003</a> |  American Joint Committee on Cancer yp stage group allowable value (qualifier value),<br> or
            <br> UICC values (to be added to SNOMED in 2025) </td>
            <td>0..1</td>
        </tr>
    <tbody>
        <tr>
            <td>Pathology_Clinical</td>
            <td>Indication whether TNM classification is based on clinical or pathological evaluation. If pathological is available, this always goes before clinical.</td>
            <td>Clinical or pathological</td>
            <td>1..1</td>
        </tr>
    <tbody>
        <tr>
            <td>Date of evaluation</td>
            <td>Date of the clinical/pathological evaluation.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>                     
    </tbody>
</table>