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
            <td>biological sex at birth</td>
            <td>The sex of a person at birth as molecular proven.</td>
            <td><a href="https://www.hl7.org/fhir/us/core/ValueSet-birthsex.html">HL7 ValueSet: Birth Sex</a></td>
            <td>0..1</td>
        </tr>
        <tr>
            <td>Date_of_Last_Follow_up</td>
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