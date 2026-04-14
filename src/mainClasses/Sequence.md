## Sequence

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
            <td>Target</td>
            <td>Identification of the sequenced target.</td>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C101294">Whole Genome Sequencing (WGS)</a> <br> <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C101295">Whole Exome Sequencing (WES)</a> <br> <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C198412">Multi-gene panel sequencing</a> <br>array <br> OTH </td>
            <td>1..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Sequencing_Date</td>
            <td>Defines the date of sequencing.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>ISO 15189 accredited</td>
            <td>Indication whether the laboratory is accredited according to ISO 15189 (clinical).</td>
            <td>Boolean</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>ISO 17025 accredited</td>
            <td>Indication whether the laboratory is accredited according to ISO 17025 (research).</td>
            <td>Boolean</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td> <b>WIP</b>  <br> Wet lab protocol</td>
            <td></td>
            <td>String or <a href="https://www.protocols.io">https://www.protocols.io</a> URL</td>
            <td></td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Participated in proficiency testing</td>
            <td>Indication whether the laboratory had participated in any proficiency testing, such as interlaboratory comparison.</td>
            <td>Boolean</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>IVDR_passed</td>
            <td>Indicate whether the methodology (including chemistry and sequencing standards) used for sequencing follows the In vitro diagnostic medical devices (IVDR) regulation passed by the EU in April 2017.</td>
            <td>Boolean</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Sequencing Platform</td>
            <td>The used sequencing platform (i.e. brand, name of a company that produces sequencer equipment).</td>
            <td><a href="https://github.com/fairgenomes/fairgenomes-semantic-model/blob/main/lookups/SequencingInstrumentModels.txt">FAIR Genomes</a> or <a href="http://purl.obolibrary.org/obo/OBI_0400103">EFO</a> list</td>
            <td>1..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Average depth of coverage</td>
            <td>Mean coverage for whole genome sequencing, or mean target coverage for whole exome and targeted sequencing (eg 60x, average number of times each target base has been ‘read’ by sequencer).</td>
            <td>Integer</td>
            <td>1..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Breadth of coverage</td>
            <td>Breadth of coverage (or evenness) is the proportion or percentage of a reads that has been sequenced at a the provided average depth of coverage. (E.g. if for Average depth of coverage, the value is 60, and the Evenness is 50% at 60x, the value here will be 50).</td>
            <td>Integer</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Additional NGS quality control metrics</td>
            <td>Statement of any additional NGS quality control metrics.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Initial_input_file_format</td>
            <td>Identification of the genomic file format of the initial input file (eg. fastq, bam, cram).</td>
            <td><a href="http://edamontology.org/format_1921">EDAM's file types and formats</a></td>
            <td>1..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Final_output_file_format</td>
            <td>Identification of the genomic file format of the final output file (eg. vcf, gvcf).</td>
            <td><a href="http://edamontology.org/format_1921">EDAM's file types and formats</a></td>
            <td>1..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Final_output_file_format_version</td>
            <td>Identification of the version of genomic file format of the final output file (eg. vcf, gvcf).</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Alignment_software</td>
            <td>Identification of the software used for alignment.</td>
            <td>--> Digital Resource class</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Alignment_Genome</td>
            <td>The specific build of the human genome used as reference for sequence alignment and variant calling.</td>
            <td>--> Digital Resource class</td>
            <td>1..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Specific_Settings_Alignment_Genome</td>
            <td> Any specific settings regarding alternative contigs or decoys.</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Target Gene</td>
            <td>In case of targeted sequencing, specify which gene is being targeted. This item points to another class: Target_Gene.</td>
            <td>--> Target Gene class</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Target Other</td>
            <td>Any other targeted genomic region.</td>
            <td>Children of <a href="http://www.sequenceontology.org/browser/current_release/term/SO:0000001">SIO region</a> <br> NULL flavors</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Panel_of_Normals_Included</td>
            <td>Indicate whether a panel of normals is included during variant calling.</td>
            <td>Boolean</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Panel_of_Normals_Description</td>
            <td>Free text description of panel of normals, if applicable.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Variant</td>
            <td>A detected and reported variant.</td>
            <td>--> Variant class</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Variant_calling</td>
            <td>Identification of the software used for variant calling.</td>
            <td>--> Digital Resource class</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Variant_calling_date</td>
            <td>Defines the date of variant calling.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Variant_Annotation</td>
            <td>Identification of the software used for variant annotation.</td>
            <td>--> Digital Resource class</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Variant_Annotation_database</td>
            <td>Database and version used for variant annotation.</td>
            <td>--> Digital Resource class</td>
            <td>0..n</td>
        </tr>
    </tbody>
</table>