### Digital Resource

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
            <td>Name</td>
            <td>The name of the tool/software/database used.</td>
            <td>String</td>
            <td>1..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Website</td>
            <td>Link to the website or repository (like GitHub) of the tool/software/database.</td>
            <td>URL</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Identifier</td>
            <td>bio.tools identifier for the digital resource.</td>
            <td><a href="https://bio.tools/">bio.tools</a> identifier</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Version</td>
            <td>The version of the tool/software/database used.</td>
            <td>double</td>
            <td>1..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Date used</td>
            <td>The date when the tool/software/database was last used.</td>
            <td>xsd:dateTime</td>
            <td>1..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Settings</td>
            <td>Free text account of the settings used in the tool/software/database.</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Parameters</td>
            <td>Description of parameters used with the specified software. Copy the complete command line (all lines executed) used.</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
    </tbody>
</table>