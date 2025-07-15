# Matches # {#matches}

Different countries use different standards or vocabularies for their data. For example, in the harmonized minimal data model we mostly use terms from SNOMED CT and NCIT, but some countries only use ICD-10, and it’s difficult for them to convert everything to SNOMED.
To make things easier, we decided to focus on matches between terms from different systems. This way, a dataset using ICD-10 can still be included in the GDI Catalogue, as long as we can clearly show how its terms connect to SNOMED or other terms.

For example:
- One dataset might use a SNOMED term to describe a disease.
- Another dataset might describe the same disease using an ICD-10 term.
- Without a match between them, our system would think they are two different things.
- If we add an exact match, the system will understand that they are the same, just described with different vocabularies.

This will make data both human and machine readable.

## How To Use Matches

We started by adding different types of matches to all items and values in the model. The types of matches (match attribute), their definitions and examples can be found in the table below.

<table>
    <thead>
        <tr>
            <th>Match Attribute</th>
            <th>Definition</th>
            <th>comExamplement</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><a href="https://www.w3.org/2009/08/skos-reference/skos.html#exactMatch">skos:exactMatch</a></td>
            <td>Two concepts have the same meaning and can be used interchangeably in all contexts. This link is transitive, meaning if A is an exact match to B, and B is an exact match to C, then A is also an exact match to C.</td>
            <td><a href="https://browser.ihtsdotools.org/?perspective=full&amp;conceptId1=184099003&amp;edition=MAIN&amp;release=&amp;languages=en">SNOMED Date of birth</a> has an exact match to <a href="https://browser.ihtsdotools.org/?perspective=full&amp;conceptId1=184099003&amp;edition=MAIN&amp;release=&amp;languages=en">EFO Date of birth</a>. Both refer to the same concept with no variation in meaning.</td>
        </tr>
        <tr>
            <td><a href="https://www.w3.org/2009/08/skos-reference/skos.html#closeMatch">skos:closeMatch</a></td>
            <td>Two concepts are sufficiently similar that they can be used interchangeably in many applications and schemes, but they are not strictly identical. This link is not meant to be transitive.</td>
            <td><a href="https://browser.ihtsdotools.org/?perspective=full&amp;conceptId1=116154003&amp;edition=MAIN&amp;release=&amp;languages=en">SNOMED Patient</a> has a close match to <a href="https://evsexplore.semantics.cancer.gov/evsexplore/concept/ncit/C142710">NCIT Study Participant</a>. <br> A patient is an individual receiving medical care, while a study participant is someone enrolled in a research study. In some cases, these terms can be used interchangeably (e.g., in clinical trials involving patients), but not all study participants are patients—some might be healthy controls.</td>
        </tr>
        <tr>
            <td><a href="https://www.w3.org/2009/08/skos-reference/skos.html#relatedMatch">skos:relatedMatch</a></td>
            <td>Two concepts are associated but not similar enough to be considered exact or close matches.</td>
            <td>   The concept <a href="https://identifiers.org/hgnc:1100">HGNC BRCA1</a> and 
            <a href="http://purl.obolibrary.org/obo/NCIT_C4872">NCIT Breast Carcinoma</a> 
            have a skos:relatedMatch relationship because they are strongly associated but not identical. 
            BRCA1 is a gene mutation, while breast cancer is a disease that may develop as a result of certain BRCA1 mutations. 
            However, not all BRCA1 mutations lead to breast cancer, and not all cases of breast cancer are caused by BRCA1 mutations, making them related but not broader/narrower concepts.</td>
        </tr>
        <tr>
            <td><a href="https://www.w3.org/2009/08/skos-reference/skos.html#broadMatch">skos:broadMatch</a></td>
            <td>The concept represented by the external entity is broader than the item. This is a reverse property of skos:narrowMatch.</td>
            <td>The concept <a href="https://ontobee.org/ontology/NCIT?iri=http://purl.obolibrary.org/obo/NCIT_C4872">NCIT Breast Carcinoma</a> has a skos:broadMatch relationship to <a href="https://browser.ihtsdotools.org/?perspective=full&amp;conceptId1=363346000&amp;edition=MAIN&amp;release=&amp;languages=en">SNOMED Cancer</a>. This means that Cancer is the broader concept because it represents a general category that includes multiple types of cancer, one of which is Breast Cancer.</td>
        </tr>
        <tr>
            <td><a href="https://www.w3.org/2009/08/skos-reference/skos.html#narrowMatch">skos:narrowMatch</a></td>
            <td>The concept represented by the external entity is narrower than the item. This is a reverse property of skos:broadMatch.</td>
            <td>The concept <a href="https://browser.ihtsdotools.org/?perspective=full&amp;conceptId1=363346000&amp;edition=MAIN&amp;release=&amp;languages=en">SNOMED Cancer</a> has a skos:narrowMatch relationship to <a href="https://ontobee.org/ontology/NCIT?iri=http://purl.obolibrary.org/obo/NCIT_C4872">NCIT Breast Carcinoma</a>. This means that Breast Cancer is a specific subtype of Cancer.</td>
        </tr>
    </tbody>
</table>

Next to the matches, we also record what is the source of the match. If the mapping has already been done, for example SNOMED to ICD-10 in the SNOMED browser, or in the T-Rex browser, we include this information with the match in the spreadsheet.

## Using SSSSOM
From now on, we decided to follow the [SSSOM (Simple Standard for Sharing Ontological Mappings)](https://mapping-commons.github.io/sssom/) method. This is a standard format for describing matches between terms. We will:
- Add all required [SSSOM elements](https://mapping-commons.github.io/sssom/linkml-index/).
- Include recommended and optional elements if they are useful.
- Make sure our matches follow the SSSOM rules.
 
Using this model and the SSSOM standard will help us:
- Make it easier for teams using different vocabularies to share their data.
- Let people and software search and analyze the data more effectively.
- Support more countries and teams to join the GDI Catalogue without needing to change everything.








