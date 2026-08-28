## GeoLocation

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
            <td>Location Name</td>
            <td>Human readable name of the location</td>
            <td>String or <a href="geonames.org">Geonames.org</a> Ontology IRI (https://sws.geonames.org/xyz)</td>
            <td>1..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Location Type</td>
            <td>Type of location (e.g. residence, infection site, event, facility, hospital)</td>
            <td>Children of <a href="https://snomedbrowser.org/?perspective=full&conceptId1=276339004&edition=MAIN/2026-08-01&release=&languages=en">SNOMED 276339004 | Environment (environment)</a></td>
            <td>1..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Geometry</td>
            <td>Geospatial shape (point, polygon, etc.)</td>
            <td>GeoJSON or WKT (Well Known Text)</td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Country</td>
            <td>Country code</td>
            <td>2- or 3-lettercode from ISO 3166-1</td>
            <td>0..1 (conditional)</td>
            <td>If geometry is provided then country, region and city are more or less obsolete</td>
        </tr>
        <tr>
            <td><a href="http://purl.obolibrary.org/obo/ENVO_00000004">Region</a></td>
            <td>Administrative region</td>
            <td><a href="geonames.org">Geonames.org</a></td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>City</td>
            <td>City or municipality</td>
            <td>rdfs:Literal (xsd:anyURI or xsd:string) where URI is from <a href="geonames.org">Geonames.org</a> (e.g https://www.geonames.org/2759794 is Amsterdam)</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Source</td>
            <td>Source of the location data (e.g. self-reported, registry, sensor).</td>
            <td>rdfs:Literal (xsd:anyURI or xsd:string)</td>
            <td>0..n</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Valid From</td>
            <td>Temporal validity of location (when applicable)</td>
            <td>DateTime (YYYY-MM-DD'T'HH:MM:SS), ISO 8601 format</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
        <tr>
            <td>Valid To</td>
            <td>Temporal validity of location (when applicable)</td>
            <td>DateTime (YYYY-MM-DD'T'HH:MM:SS), ISO 8601 format</td>
            <td>0..1</td>
            <td>NA</td>
        </tr>
    </tbody>
</table>