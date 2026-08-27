#### Target Gene

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
            <td>Identifier</td>
            <td>Schema and identifier of the target gene, expressed with an instance of adms:Identifier</td>
            <td><a href="#identifier">Identifier class</a></td>
            <td>1..1 (conditional)</td>
            <td>It is mandatory to provide either identifier or label.</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Label</td>
            <td>Label of the target gene, if no URI can be provided.</td>
            <td>String</td>
            <td>1..1 (conditional)</td>
            <td>It is mandatory to provide either identifier or label.</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Description</td>
            <td>Description of target gene.</td>
            <td>String</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
    </tbody>
</table>