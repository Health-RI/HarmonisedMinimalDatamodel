#### Variant Calling

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
            <td>Variant Calling Software</td>
            <td>Identification of the software used for variant calling.</td>
            <td><a href="#digital-resource">Digital Resource class</a></td>
            <td>1..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Variant Annotation</td>
            <td>Identification of the software used for variant annotation.</td>
            <td><a href="#digital-resource">Digital Resource class</a></td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Variant Annotation Database</td>
            <td>Database and version used for variant annotation.</td>
            <td><a href="#digital-resource">Digital Resource class</a></td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Panel of Normals Included</td>
            <td>Indicate whether a panel of normals is included during variant calling.</td>
            <td>Boolean</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Panel of Normals Description</td>
            <td>Free text description of panel of normals, if applicable.</td>
            <td>String</td>
            <td>0..1 (conditional)</td>
            <td>If panel of normals == TRUE</td>
        </tr>
    </tbody>
</table>