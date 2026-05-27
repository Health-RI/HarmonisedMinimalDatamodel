## Data Provenance

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
            <td>Data Submitter</td>
            <td>Full name of the person responsible for submitting the data into the dataset. A string with the name can be provided, but a ORCID can be submitted as well (as a string).</td>
            <td>String</td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Data Submitter Email</td>
            <td>Email where the person responsible for the data submission can be reached at.</td>
            <td>String</td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Data Submitter Role</td>
            <td>Role of the Submitter (e.g. oncologist in charge of the patient, research project PI)</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Department of data submitter</td>
            <td>Refers to the Department of the Submitter</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Submitter Institution</td>
            <td>Identifies the Institution of the data submitter. A string with the name can be provided, but a ROR can be submitted as well (as a string).</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Country</td>
            <td>Country of Submission.</td>
            <td>GeoLocation class (or if we cannot implement input of only country and filling the mandatory items then stick to 2- or 3-lettercode from ISO 3166-1)</td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Data Collector</td>
            <td>Identifies the person responsible for Data Collection</td>
            <td>String</td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Data Production Department</td>
            <td>Refers to the Department in charge of Data Production</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Data Analysis Department</td>
            <td>Refers to the Department in charge of Data Analysis</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Projects/Trial/cohort/surveillance study</td>
            <td>Identifies projects which data are part of</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Research Consortia</td>
            <td>Identifies Research Consortia involved</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
    </tbody>
</table>