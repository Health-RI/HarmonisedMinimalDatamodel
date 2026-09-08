## Test

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
            <td>Test Description</td>
            <td>Name or description of the test.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Test Start Date</td>
            <td>Defined the date of when the test began.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>ISO 15189 accredited</td>
            <td>Indication whether the laboratory is accredited according to ISO 15189 (clinical) at the time of genotyping.</td>
            <td>Boolean</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>ISO 17025 accredited</td>
            <td>Indication whether the laboratory is accredited according to ISO 17025 (testing and calibration) at the time of genotyping.</td>
            <td>Boolean</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Protocol</td>
            <td>The protocol used for the test.</td>
            <td><a href="#protocol">Protocol class</a></td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Diagnosis</td>
            <td>Establishes the link between Test and Diagnosis class.</td>
            <td><a href="#diagnosis">Diagnosis class</a></td>
            <td>0..n</td>
        </tr>
    </tbody>
</table>