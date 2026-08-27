## [Subject](https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C48910)

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
            <td>Birth Date</td>
            <td>The calendar date on which a person was born.</td>
            <td>Complete date, without time, following the ISO 8601. If only year or year-month is available, use that. xsd:date or xsd:gYearMonth or xsd:gYear</td>
            <td>1..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Administrative Gender</td>
            <td>The gender of a person used for administrative purposes.</td>
            <td><a href="https://build.fhir.org/valueset-administrative-gender.html">HL7 Administrative Gender</a></td>
            <td>1..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Genetic determined sex</td>
            <td>The sex of a person at birth as genetically proven.</td>
            <td><a href="https://www.hl7.org/fhir/us/core/ValueSet-birthsex.html">HL7 ValueSet: Birth Sex</a></td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Date of Last Follow-up</td>
            <td>Date of last follow-up, partial date with month and year.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>1..1 (conditional)</td>
            <td>Mandatory item in cancer use case</td>
        </tr>
        <tr>
            <td>Status at Last Follow-up</td>
            <td>Status of the subject at last follow-up.</td>
            <td>Alive, <br>
                Alive with disease, <br>
                Alive without disease, <br>
                Dead, <br>
                Dead with disease, <br>
                Dead due to other causes, <br>
                Lost to follow-up, <br>
                Unknown</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Country of birth</td>
            <td>Country which a person was born in.</td>
            <td>
            2- or 3-lettercode from <a href="https://www.iso.org/obp/ui/#iso:std:iso:3166:-1:ed-4:v1:en">ISO 3166-1</a> if only a country code is provided. <br>If a country-subdivision then a value from the ISO <a href="https://www.iso.org/obp/ui/#iso:std:iso:3166:-2:ed-4:v1:en">ISO 3166-2</a></td>
            <td>1..1 (conditional)</td>
            <td>Mandatory item in GoE & complex and common disease use cases</td>
        </tr>
        <tr>
            <td>Subject ID</td>
            <td>A sequence of characters used to identify, name, or characterize a trial or study subject.</td>
            <td>String</td>
            <td>1..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Socioeconomic status</td>
            <td>An individual's relative social and economic position in a society based on a combination of education, income, employment, and wealth.</td>
            <td>String</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Consent</td>
            <td>Consent to proceed to personal data analysis.</td>
            <td><a href="#consent">Consent class</a></td>
            <td>1..1 (conditional)</td>
            <td>Mandatory for Infectious Diseases.</td>
        </tr>
        <tr>
            <td>Environmental exposure</td>
            <td>Establishes a link between Subject and Environmental exposure class.</td>
            <td><a href="#environmental-exposure">Environmental Exposure class</a></td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>has Sample</td>
            <td>Establishes a link between Subject and Sample class.</td>
            <td><a href="#sample">Sample class</a></td>
            <td>1..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>has Treatment</td>
            <td>Establishes a link between Subject and Treatment class.</td>
            <td><a href="#treatment">Treatment class</a></td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Subject Diagnosis</td>
            <td>Establishes a link between Subject and Diagnosis class.</td>
            <td><a href="#diagnosis">Diagnosis class</a></td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Test</td>
            <td>Establishes a link between Subject and Test class.</td>
            <td><a href="#test">Test class</a></td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
    </tbody>
</table>