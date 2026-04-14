### Target Gene

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
            <td>URI</td>
            <td>URI identifying the targeted gene.</td>
            <td>URI to either <a href="https://www.genenames.org/">HGNC</a> <a href="https://www.ncbi.nlm.nih.gov/gene">NCBI gene</a>, <a href="https://www.omim.org/">OMIM</a>, <a href="https://hpo.jax.org/">HPO</a> or <a href="https://hgvs-nomenclature.org/stable/">HGVS</a> for variants.</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Label</td>
            <td>Label of the target gene, if no URI can be provided.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Description</td>
            <td>Description of target gene.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    </tbody>
</table>