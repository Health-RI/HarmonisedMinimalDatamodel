### Variant

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
            <td>Variant_Type</td>
            <td>The category or type of variation or abnormality present in an amino acid or nucleic acid sequence.</td>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C164674">SNVs</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C99752">indels</a>, SVs, CNVs, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C20195">gene fusions</a>, ... (to be extended).</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Variant_Origin</td>
            <td>A quality inhering in a variant by virtue of its origin.</td>
            <td><a href="http://purl.obolibrary.org/obo/SO_0001777">somatic</a>, <a href="http://purl.obolibrary.org/obo/SO_0001778">germline</a>, <a href="http://purl.obolibrary.org/obo/SO_0001775">maternal</a>, <a href="http://purl.obolibrary.org/obo/SO_0001776">paternal</a>, <a href="http://purl.obolibrary.org/obo/SO_0001779">pedigree specific</a>, <a href="http://purl.obolibrary.org/obo/SO_0001780">population specific</a>, <a href="http://purl.obolibrary.org/obo/SO_0001781">de novo</a>.</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Variant_representation</td>
            <td>The representation of the variant using HGVS nomenclature.</td>
            <td>String following <a href="https://hgvs-nomenclature.org/stable/">HGVS nomenclature</a></td>
            <td>1..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Clinical_Variant_Interpretation_criteria</td>
            <td>Internationally (e.g. ACMG, ESMO-ESCAT) criteria met for variant interpretation</td>
            <td>List of versions of ACMG, ESMO-ESCAT, others??</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Clinical_Variant_Interpretation_result</td>
            <td>Indicates result of clinical variant interpretation.</td>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C168802">benign</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C168801">likely benign</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C94187">VUS</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C168800">likely pathogenic</a>, <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C168799">pathogenic</a>.</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Clinical_expert_panel_decision</td>
            <td>Decision by clinical expert panel concerning the variant interpretation</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Applied_Criteria_of_Evidence</td>
            <td>A category which fits with categories provided by Expert panels or tools accepted in Clincial Practice. If such recommendations are not available the weighted categories provided by freely available tools would be acceptable.</td>
            <td>As listed in tables 3 and 4 in <a href="https://doi.org/10.1038/gim.2015.30">Standards and guidelines for the interpretation of sequence variants: a joint consensus recommendation of the American College of Medical Genetics and Genomics and the Association for Molecular Pathology</a></td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Clinical_Interpretation_Tool</td>
            <td>Identification of the tool used for clinical interpretation</td>
            <td>--> Digital Resource class</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Variant_calling_software_deviation</td>
            <td>Identification of the software used for variant calling, if different from software stated in Sequence class.</td>
            <td>--> Digital Resource class</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Variant_Annotation_tools_deviation</td>
            <td>Identification of the software used for variant annotation, if different from software stated in Sequence class. </td>
            <td>--> Digital Resource class</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Variant_Annotation_database_deviation</td>
            <td>Database and version used for variant annotation, if different from software stated in Sequence class.</td>
            <td>--> Digital Resource class</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Reported_to_patient</td>
            <td>Indication if the variant has been reported back to the patient, if different from software stated in Sequence class.</td>
            <td>Boolean</td>
            <td>0..1</td>
        </tr>
    </tbody>
</table>