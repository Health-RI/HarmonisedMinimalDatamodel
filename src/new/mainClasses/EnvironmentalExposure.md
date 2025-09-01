## Environmental Exposure

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
            <td>Tobacco Use Status</td>
            <td>The status of the patient’s tobacco use.</td>
            <td><a href="http://purl.bioontology.org/ontology/SNOMEDCT/449868002">SCTID:449868002</a> | Smokes tobacco daily
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/428041000124106">SCTID:428041000124106</a> | Occasional tobacco smoker
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/43381005">SCTID:43381005</a> | Passive smoker
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/8517006">SCTID:8517006</a> | Ex-smoker
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/405746006">SCTID:405746006</a> | Current non smoker but past smoking history unknown
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/266919005">SCTID:266919005</a> | Never smoked tobacco
            <br>NullFlavor <a href="https://terminology.hl7.org/1.0.0/CodeSystem-v3-NullFlavor.html#v3-NullFlavor-OTH">OTH</a> </td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Type Of Tobacco Used</td>
            <td>Type of tobacco the patient uses.</td>
            <td>Children of <a href="https://addictovocab.org/ADDICTO_0000311">tobacco product</a> combined with childred of <a href="https://addictovocab.org/ADDICTO_0000316">vaporizer</a>, or
            <br> <a href="https://terminology.hl7.org/1.0.0/CodeSystem-v3-NullFlavor.html">HL7 NULL flavors</a></td>
            <td>1..n (conditional)</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Smoking amount</td>
            <td>The number of cigarettes, cigars or grams of rolling tobacco consumed per day, week, month or year.</td>
            <td>amount/day | amount/week | amount/month | amount/year</td>
            <td>1..1 (conditional)</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Pack years</td>
            <td>The unit indicating the smoker’s total exposure to tobacco smoke. For cigarettes, this is calculated using the number of smoked packs of cigarettes per day (one pack = 20 cigarettes) times the number of years of smoking. For other forms of tobacco, this is usually converted to an equivalent cigarette consumption. Often, only the number of pack years is estimated.</td>
            <td>Integer </td>
            <td>1..1 (conditional)</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Alcohol use status</td>
            <td>The status of the patient’s alcohol use.</td>
            <td><a href="http://purl.bioontology.org/ontology/SNOMEDCT/219006">SCTID:219006</a> | Current drinker
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/105542008">SCTID:105542008</a> | Non - drinker
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/82581004">SCTID:82581004</a> | Ex-drinker
            <br><a href="http://purl.bioontology.org/ontology/SNOMEDCT/783261004">SCTID:783261004</a> | Lifetime non-drinker of alcohol
            <br>NullFlavor <a href="https://terminology.hl7.org/1.0.0/CodeSystem-v3-NullFlavor.html#v3-NullFlavor-OTH">OTH</a> </td>
            <td>0..1</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Alcohol amount</td>
            <td>The extent of the patient’s alcohol use in units of alcohol per time period (day/week/year).</td>
            <td>AU per (day/week/year). 1 A.U.= 
            <br>125 ml of wine, 
            <br>330 ml of beer, 
            <br>80 ml of drink, 
            <br>40 ml liquor</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Other Type of Exposure</td>
            <td>Indicates other exposures other than tabacco/smoking and alcohol use, for example asbestos. This exposure can include direct physical contact, inhalation, ingestion, or residing in close proximity to the source.</td>
            <td>- Inadequate water (quantity and quality), sanitation and solid waste disposal, improper hygein (handwashing)
            <br>- Improper water resource managment, uncluding poor drainage,
            <br>- Crowded housing and poor ventialtion of smoke
            <br>- Exposures to vehicular and industrial air pollution
            <br>- Population movement and encroachment and construction, which affect feeding and breeding grounds of vectors, such as mosquitoes,
            <br>- Exposure to naturally ocurring toxic substances
            <br>- Natural resources degradation (for example, landslides, poor drainage, erosion)
            <br>- Climate change, partly from combustion of fossil fuel and release of greenhouse gases in transportation, industry, and poor energy conservation in housing, fuel, commerce, and industry
            <br>- Ozone depletion from industrial and commercial actvitiy
            <br><b>Biological hazard</b> (Bacteria, Fungi, Parasitic worms, Protozoa, Viruses, Prions)
            <br><b>Chemical hazards</b> (Air pollutant, Heavy metal (Arsenice, Mercury, Lead), Pesticides, Other ( Formaldehyde, Asbestos, PFAS, PCBs, BPA, Phthalates, Radon, DDT)
            <br><b>Physical environmental hazard</b> (Radiation, Natural disaster (narrow matches: exposure to earthquake, exposure to flooding, exposure to tsunami etc.), Extreme weather, Human activities (eg. traffic accident))
            <br><a href="https://terminology.hl7.org/1.0.0/CodeSystem-v3-NullFlavor.html">HL7 NULL flavors</a></td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Other_Other Type of Exposure</td>
            <td>Provide the option to if "Other" option is choosen from List of other exposures, type a free text field.</td>
            <td>String</td>
            <td>1..1 (conditional)</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Travel History</td>
            <td>Description of any travel within 4 weeks before the diagnosis.</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Travel History_start_date</td>
            <td>Start date of relevant travel history.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Travel History_end_date</td>
            <td>End date of relevant travel history.</td>
            <td>Date (YYYY-MM-DD), ISO 8601 format</td>
            <td>0..n</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td>Residential area at risk</td>
            <td>Description of the area of ​​known environmental exposure conditions where the subject/patient resides.</td>
            <td>String</td>
            <td>0..n</td>
        </tr>
    </tbody>
</table>