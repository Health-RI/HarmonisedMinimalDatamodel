#### Protocol

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
            <td>Description</td>
            <td>Type of protocol</td>
            <td>String (e.g.library preparation, Genome extraction protocol, Sequencing protocol)</td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Available at</td>
            <td>Link to a protocol available at <a href="protocols.io">protocols.io</a></td>
            <td>URL to <a href="protocols.io">protocols.io</a></td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Kit number</td>
            <td>A number or sequence of characters that identifies a particular kit.</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Participated in proficiency testing</td>
            <td>Indication of what type of proficiency testing the laboratory had participated in.</td>
            <td>String (for example:
                external EQA, <br>
                national PT program, <br>
                international PT program, <br>
                internal PT, <br>
                interlaboratory comparison, <br>
                Include as well if PT is for a specific test or analysis)</td>
            <td>0..n</td>
        </tr>
    </tbody>
</table>