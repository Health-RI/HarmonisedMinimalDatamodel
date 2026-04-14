## Diagnosis

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
            <td>Date of Diagnosis</td>
            <td>Date at which diagnosis was made.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Diagnosis</td>
            <td>The investigation, analysis and recognition of the presence and nature of disease, condition, or injury from expressed signs and symptoms; also, the scientific determination of any kind; the concise results of such an investigation.</td>
            <td>Children of SNOMED-CT <a href="http://purl.bioontology.org/ontology/SNOMEDCT/64572001">Disease (Disorder)</a></td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Provisional diagnosis / clinical diagnosis</td>
            <td>An initial diagnosis that is subject to change as new information becomes available.</td>
            <td>Children of SNOMED-CT <a href="http://purl.bioontology.org/ontology/SNOMEDCT/64572001">Disease (Disorder)</a></td>
            <td>0..n</td>
        </tr>
    </tbody>
</table>