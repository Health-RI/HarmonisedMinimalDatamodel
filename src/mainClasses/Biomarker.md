## Biomarker

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
            <td>Purpose</td>
            <td>Necessary information to indicate the objective of the biomarker used  (coded value, e.g. diagnostic, prognostic,…).</td>
            <td><a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C201361">Diagnosis</a> <br>
            <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C201363">Prognosis</a> <br>
            <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C201364">Prediction</a> <br>
            <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C201362">Monitoring</a></td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Type</td>
            <td>What type is the biomarker classified as.</td>
            <td>Molecular
            <br>Imaging
            <br>Anthropometric
            <br>Cellular
            <br>Physiological</td>
            <td>1..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Subtype</td>
            <td>Subtype of the biomarker as classified in the type.</td>
            <td>If Type ==
            <br>- <b>Molecular</b>: Genetics/Genomics,
            Epigenetics/Epigenomics,
            Transcription/Transcriptomics,
            Metabolites/Metabolomics,
            Proteins/Proteomics,
            Microbiomics/Microbiology,
            Biochemistry (biochemical),
            Other molecular biomarker,
            N/P
            <br>- <b>Imaging</b>: X-Rays,
            Ultrasound (echography, etc),
            CT Scan,
            PET/SPECT,
            Spectrometry,
            MRI,
            Scintigraphy (Gamma),
            Mammography,
            Other image biomarker,
            N/P
            <br>- <b>Anthropometric</b>: BMI,
            Body perimeters (circumference),
            Other anthropometric biomarker,
            N/P
            <br>- <b>Cellular</b>: Histology (tissue abnormalities),
            Cytology (cell types),
            Other cellular biomarker,
            N/P
            <br>- <b>Physiological</b>: Blood Pressure,
            Ankle-brachial Index,
            ECG,
            EEG,
            Electromyography,
            Other physiological biomarker,
            N/P</td>
            <td>1..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Name</td>
            <td>Biomarker name.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    </tbody>    
    <tbody>
        <tr>
            <td>Code</td>
            <td>Code of the biomarker.</td>
            <td>String</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Code System</td>
            <td>Code System of the Biomarker Code.</td>
            <td>String or URI</td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Date</td>
            <td>The date of the biomarker being obtained.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>
    </tbody>        
</table>