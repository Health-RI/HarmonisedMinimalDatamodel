#### Variant Calling

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
            <td>Variant_calling_software</td>
            <td>Identification of the software used for variant calling.</td>
            <td>--> Digital Resource class</td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Variant_Annotation</td>
            <td>Identification of the software used for variant annotation.</td>
            <td>--> Digital Resource class</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Variant_Annotation_database</td>
            <td>Database and version used for variant annotation.</td>
            <td>--> Digital Resource class</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Panel_of_Normals_Included</td>
            <td>Indicate whether a panel of normals is included during variant calling.</td>
            <td>Boolean</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Panel_of_Normals_Description</td>
            <td>Free text description of panel of normals, if applicable.</td>
            <td>String</td>
            <td>0..1 (conditional)</td>
        </tr>
    </tbody>
</table>