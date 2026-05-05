## Genotyping

The Genotyping class is a subclass of the Test class. This means that it adopts all items from the Test class, and adds some Genotyping-specific items.
The Biomarker class is another subclass from the Test class. Any reference from another class to a Test can be either a generic Test (in that case, the Test class is used), or an instance of the Genotyping or Biomarker class. If a reference from a class is established directly to Genotyping, that class has to be used.

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
            <td>Technology</td>
            <td>Genotyping technology used.</td>
            <td>whole genome (3gb, 3m variants) - short read, <br>
                whole genome (3gb, 3m variants) - long read, <br>
                whole exome ( ~45Mb, 40k variants) - short read, <br>
                whole exome ( ~45Mb, 40k variants) - long read, <br>
                optical genome mapping, <br>
                genotyping array (~1Mb, 200k variants), <br>
                arrays + imputation (~1Mb, 1m variants), <br>
                gene panel (~45kb, ~50 variants), <br>
                single gene (2kb, 3 variants), <br>
                single exon (200 nt, 0-1 variants), <br>
                single variant (1nt, 0-1 variants)</td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>IVDR_passed</td>
            <td>Indicate whether the methodology (including chemistry and genotyping standards) used for genotyping follows the In vitro diagnostic medical devices (IVDR) regulation passed by the EU in April 2017.</td>
            <td>boolean</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Platform</td>
            <td>The used sequencing platform (i.e. brand, name of a company that produces sequencer equipment).</td>
            <td>**Sequencing:**<a href="https://github.com/fairgenomes/fairgenomes-semantic-model/blob/main/lookups/SequencingInstrumentModels.txt">FAIR Genomes</a> or <a href="https://bioportal.bioontology.org/ontologies/EFO/?p=classes&conceptid=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FOBI_0400103">EFO list</a> <br>
               **Microarrays:** <br>
                Illumina Exome V1.1, <br>
                Illumina Immuno V2, <br>
                Illumina Cyto12, <br>
                Illumina Core, <br>
                Illumina  DrugDev, <br>
                Illumina Onco, <br>
                Illumina PsychArray, <br>
                Affymetrix Axiom_GW_ASI, <br>
                Illumina 660w-Quad, <br>
                Affymetrix Axiom_GW_CHB, <br>
                Affymetrix Axiom_NL, <br>
                Affymetrix Axiom_GW_EUR, <br>
                Illumina OmniExpress, <br>
                Illumina GSAv1, <br>
                Illumina GSAv3, <br>
                Affymetrix Axiom_LAT, <br>
                Affymetrix Axiom_UKB, <br>
                Illumina CytoSNP850K, <br>
                Illumina OmniZhongHua, <br>
                Affymetrix PMRA, <br>
                Affymetrix PMDA, <br>
                Affymetrix Affy6.0, <br>
                Illumina MultiEthnic-AMR/AFR, <br>
                Illumina MultiEthnic-EUR/ASN, <br>
                Illumina MultiEthnic-Global, <br>
                Affymetrix Axiom_GW_PanAFR, <br>
                Illumina Omni2.5, <br>
                Illumina Omni5, <br>
               **OTHER (String)**</td>
            <td>1..n</td>
        </tr>
        <tr>
            <td>Targeted_Gene</td>
            <td>In case of targeted sequencing, specify which gene is being targeted. This item points to another class: Target_Gene</td>
            <td>Class Target_Gene</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Target Other</td>
            <td>Any other targeted genomic region.</td>
            <td>Children of <a href="http://www.sequenceontology.org/browser/current_release/term/SO:0000001">SIO region</a> <br> NULL flavors</td>
            <td>0..n</td>
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
            <td>0..1</td>
        </tr>
        <tr>
            <td>Average depth of coverage</td>
            <td>Mean coverage for whole genome sequencing, or mean target coverage for whole exome and targeted sequencing (eg 60x, average number of times each target base has been ‘read’ by sequencer). (Observed)</td>
            <td>Float</td>
            <td>1..1 (conditional)</td>
        </tr>
        <tr>
            <td>Breadth of coverage</td>
            <td>A data item which is the amount of a reference sequence covered by a sequence of interest. (Observed) <br>
            Example of usage: <br>
            Eighty percent of the reference genome was covered by sequence fragments with a coverage depth of 4X; therefore, the breadth of coverage was 80% (4:5).</td>
            <td>Float</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Additional NGS quality control metrics</td>
            <td>Statement of any additional NGS quality control metrics.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Initial_input_file_format</td>
            <td>Identification of the genomic file format of the initial input file (eg. fastq, bam, cram).</td>
            <td><a href="http://edamontology.org/format_1921">EDAM's file types and formats</a></td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Final_output_file_format</td>
            <td>Identification of the genomic file format of the final output file (eg. vcf, gvcf).</td>
            <td><a href="http://edamontology.org/format_1921">EDAM's file types and formats</a></td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Final_output_file_format_version</td>
            <td>Identification of the version of genomic file format of the final output file (eg. VCF version 4.3).</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Alignment_software</td>
            <td>Identification of the software used for alignment.</td>
            <td>--> Digital Resource class</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Alignment_Genome</td>
            <td>The specific build of the human genome used as reference for sequence alignment and variant calling.</td>
            <td>--> Digital Resource class</td>
            <td>1..n</td>
        </tr>
        <tr>
            <td>Specific_Settings_Alignment_Genome</td>
            <td> Any specific settings regarding alternative contigs or decoys.</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Variant</td>
            <td>A detected and reported variant.</td>
            <td>--> Variant class</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Variant_calling</td>
            <td>Identification of the software used for variant calling.</td>
            <td>--> Digital Resource class</td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Variant_calling_date</td>
            <td>Defines the date of variant calling.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
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
            <td>0..n</td>
        </tr>
    </tbody>
</table>