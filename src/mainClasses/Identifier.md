#### Identifier

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
            <td><a href="https://www.w3.org/TR/vocab-adms/#adms-schemaagency">Schema</a></td>
            <td>Name of the schema agency</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td><a href="https://www.w3.org/2009/08/skos-reference/skos.html#notation">Identifier</a></td>
            <td>Identifier from the corresponding schema for the target gene.</td>
            <td>String</td>
            <td>1..1</td>
        </tr>
        <tr>
            <td><a href="http://purl.org/dc/terms/conformsTo">Scheme URI</a></td>
            <td>URI of the scheme used to construct the identifier.</td>
            <td>String (with#anyURI) of either <a href="http://www.wikidata.org/entity/Q1646383">HGNC</a>, <a href="http://www.wikidata.org/entity/Q20641742">NCBI gene</a>, <a href="http://www.wikidata.org/entity/Q905695">UniProtID</a>, <a href="http://www.wikidata.org/entity/Q241953">OMIM</a>, <a href="http://www.wikidata.org/entity/Q17027854">HPO</a> or <a href="http://semanticscience.org/resource/SIO_001389">HGVS</a> for variants </td>
            <td>1..1</td>
        </tr>
    </tbody>
</table>