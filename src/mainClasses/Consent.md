### Consent

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
            <td>Consent_scientificResearch</td>
            <td>Specify whether subject has given consent to secondary use of the data for scientific research for health purposes.</td>
            <td>Boolean</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Consent_policy</td>
            <td>Specify whether subject has given consent to secondary use of the data for policy development in health systems.</td>
            <td>Boolean</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Consent_qualityManagement</td>
            <td>Specify whether subject has given consent to secondary use of the data for quality management in healthcare.</td>
            <td>Boolean</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Consent_healthcare</td>
            <td>Specify whether subject has given consent to secondary use of the data in healthcare.</td>
            <td>Boolean</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td><a href="http://purl.obolibrary.org/obo/GENEPIO_0002032">Consent date</a></td>
            <td>Date on which consent was given.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>1..1 (conditional)</td>
            <td>Mandatory for Infection Diseases</td>
        </tr>
    </tbody>
</table>