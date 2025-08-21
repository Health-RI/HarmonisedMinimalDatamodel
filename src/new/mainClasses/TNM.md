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
            <td>Children of <a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=1279504008&edition=MAIN/2024-11-01&release=&languages=en&latestRedirect=false">1279504008 | American Joint Committee on Cancer ycN category allowable value (qualifier value)</a></td>
            <td>0..1</td>
        </tr>
    <tbody>
        <tr>
            <td>Metastases</td>
            <td>Indicates presence or absence of metastasis according to the international TNM classification for solid tumors.</td>
            <td>Children of <a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=1222587001&edition=MAIN&release=&languages=en">American Joint Committee on Cancer pathological M category allowable value (qualifier value)</a> <br> or <br> Children of <a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=1222591006&edition=MAIN&release=&languages=en"> American Joint Committee on Cancer clinical M category allowable value (qualifier value)</a>  <br> and HL7 NULL flavor in case not determined.</td>
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
            <td><a href=""></a> <br> or <br>
            <a href=""></a> <br> or
            <br> <a href=""></a> <br> or
            <br> <a href=""></a></td>
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