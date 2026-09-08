#### Protocol

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
            <td>Description</td>
            <td>Type of protocol</td>
            <td>String (e.g.library preparation, Genome extraction protocol, Sequencing protocol)</td>
            <td>1..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Available at</td>
            <td>Link to a protocol available at <a href="protocols.io">protocols.io</a></td>
            <td>URL to <a href="protocols.io">protocols.io</a></td>
            <td>1..1 (conditional)</td>
            <td>Mandatory to provide either "Available at" or "Kit number"</td>
        </tr>
        <tr>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C87822">Kit number</a></td>
            <td>A number or sequence of characters that identifies a particular kit.</td>
            <td>String</td>
            <td>1..n (conditional)</td>
            <td>Mandatory to provide either "Available at" or "Kit number"</td>
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
            <td>NA</td>
        </tr>
    </tbody>
</table>