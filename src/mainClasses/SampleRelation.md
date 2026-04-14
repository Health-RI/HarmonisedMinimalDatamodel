### Sample Relation

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
            <td>Related_Sample</td>
            <td>Points to a related sample.</td>
            <td>Sample ID</td>
            <td>1..n</td>
        </tr>
    <tbody>
        <tr>
            <td>Relation_Type</td>
            <td>Describes the relationship type between the two connected samples.</td>
            <td>List to be defined/extended:
            <br>New sample
            <br>Derived
            <br>Aliquot
            <br>Control (experiment)
            <br>Disease versus Control
            <br>Matched
            <br>Longitudinal
            <br>Paired
            <br>Familial
            <br>Spatial</td>
            <td>1..1</td>
        </tr>
    <tbody>
        <tr>
            <td>Relation_Description</td>
            <td>Free text describing the Relation Type of two samples.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    </tbody>
</table>