# Main Classes # {#main-classes}
In the Harmonized Minimal Dataset, we defined 12 different classes.

## Subject

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
            <td>Birth Date</td>
            <td>The calendar date on which a person was born.</td>
            <td>Complete date, without time, following the ISO 8601. If only year or year-month is available, use that. xsd:date or xsd:gYearMonth or xsd:gYear</td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Administrative Gender</td>
            <td>The gender of a person used for administrative purposes.</td>
            <td><a href="https://build.fhir.org/valueset-administrative-gender.html">HL7 Administrative Gender</a></td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Biological Sex at Birth</td>
            <td>The sex of a person at birth as molecular proven.</td>
            <td><a href="https://www.hl7.org/fhir/us/core/ValueSet-birthsex.html">HL7 ValueSet: Birth Sex</a></td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Date of Last Follow-up</td>
            <td>Date of last follow-up, partial date with month and year.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Country of Origin</td>
            <td>A person's descent or lineage, from a person or from a population.</td>
            <td>2- or 3-lettercode from <a href="https://www.iso.org/obp/ui/#iso:std:iso:3166:-1:ed-4:v1:en">ISO 3166-1</a> if only a country code is provided. If a country-subdivision then a value from the <a href="https://www.iso.org/obp/ui/#iso:std:iso:3166:-2:ed-4:v1:en">ISO 3166-2</a></td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Subject ID</td>
            <td>A sequence of characters used to identify, name, or characterize a trial or study subject.</td>
            <td>String</td>
            <td>1..1</td>
        </tr>
    </tbody>
</table>

## Sample

## Sequence

## Sample Relation

## Diagnosis

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
            <td>Date of Diagnosis</td>
            <td>Date at which diagnosis was made.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Administrative Gender</td>
            <td>The gender of a person used for administrative purposes.</td>
            <td><a href="https://build.fhir.org/valueset-administrative-gender.html">HL7 Administrative Gender</a></td>
            <td>1..1</td>
        </tr>
        <tr>
            <td>Diagnosis</td>
            <td>The investigation, analysis and recognition of the presence and nature of disease, condition, or injury from expressed signs and symptoms; also, the scientific determination of any kind; the concise results of such an investigation.</td>
            <td><a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=64572001&edition=MAIN/2024-10-01&release=&languages=en&latestRedirect=false">Children of Disease (Disorder) in SNOMED</a></td>
            <td>0..n</td>
        </tr>
        <tr>
            <td>Provisional diagnosis / clinical diagnosis</td>
            <td>An initial diagnosis that is subject to change as new information becomes available.</td>
            <td><a href="https://browser.ihtsdotools.org/?perspective=full&conceptId1=64572001&edition=MAIN/2024-10-01&release=&languages=en&latestRedirect=false">Children of Disease (Disorder) in SNOMED</a></td>
            <td>0..n</td>
        </tr>
    </tbody>
</table>

## Treatment

## Environmental Exposure

## Biomarker

## TNM

## Variant

## Target Gene

## Digital Resource
