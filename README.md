# README

## Data for:
**From Lagging to Leading: Increased Phenological Asynchrony in a Batesian Mimicry Complex**  
**DOI:** [https://doi.org/10.5061/dryad.jwstqjqjw](https://doi.org/10.5061/dryad.jwstqjqjw)

---

## DATA FILES

### 1) ModelMimics_raw data

**Description:**  
This Excel spreadsheet contains raw observational data on flight times of model bumblebees and their hoverfly mimics, extracted on 21 June 2023 from two online citizen science and museum specimen databases:  
- [Norwegian Artsdatabanken](https://www.artsdatabanken.no/)  
- [Swedish Artportalen](https://www.artportalen.se/)

Data were downloaded, translated where necessary (from Norwegian and Swedish), and cleaned for use in this study.  
Please refer to the Methods section of the accompanying paper for detailed data collection and cleaning protocols.

---

### Spreadsheet Tabs:

#### a) Artsdatabanken_mimic 21.06.2023
- **Content:** Raw records of mimic hoverflies from Norway.
- **Notes:** Column headings provided in both Norwegian and English.

**Variables:**  
| Column Name (English) | Original (Norwegian) | Description |
|:----------------------|:---------------------|:------------|
| institution | institusjon | Hosting institution (e.g., museum, database source) |
| collection | samling | Name of the collection within the institution |
| IUCN status | Kategori | Conservation status (e.g., Least Concern, Vulnerable) |
| validScientificName | Vitenskapelig navn | Validated scientific name |
| taxonGroupName | taksongruppenavn | Taxonomic group (e.g., Syrphidae, Bombus) |
| Finder/Collector | Finner/Samler | Person who found/collected the specimen |
| Date | Funndato | Date of observation or collection (DD.MM.YYYY) |
| locality | Lokalitet | Specific site of observation |
| coordinate Precision | Presisjon | Precision of coordinates |
| municipality | Kommune | Municipality |
| county | Fylke | County/region |
| individualCount | Antall | Number of individuals observed |
| basisOfRecord | Funnegenskaper | Type of record (e.g., observation, specimen) |
| identifiedBy | Artsbestemt av | Identifier of the species |
| validated (Yes/No) | Validert (Ja/Nei) | Validation status |
| catalogNumber | Katalognummer | Catalog number |
| latitude | Breddegrad | Latitude (decimal degrees) |
| longitude | Lengdegrad | Longitude (decimal degrees) |
| øst | øst | Eastern UTM coordinate |
| nord | nord | Northern UTM coordinate |
| geometry | geometri | Geospatial data field |
| behavior | Aktivitet | Behavior observed |
| Photo documentation | Bildedokumentasjon | Presence of photographs |
| dateLastModified | - | Last modification date |
| dateLastIdentified | - | Last identified date |
| occurrenceId | forekomst-ID | Unique occurrence ID |
| datasetName | datasettnavn | Dataset name |
| notes | notater | Additional notes |
| habitat | habitat | Habitat description |
| Sex | Kjønn | Sex of individual (M=male, F=female, u=worker, dronning=queen) |
| otherCatalogNumbers | Andre Katalognummer | Additional catalog numbers |
| recordNumber | rekordnummer | Record number |
| fieldNumber | felt id | Field-specific ID |
| Preparation method | Prepareringsmetode | Specimen preparation method |
| dynamicProperties | dynamiske egenskaper | Additional dynamic properties |
| nodeId | node-ID | Database node ID |
| Institutional code | Institusjonskode | Institution code |
| collectionCode | samlingskode | Collection code |

---

#### b) Artsdatabanken_model 21.06.2023
- **Content:** Raw records of model bumblebees from Norway.
- **Notes:** Same format and structure as tab (a).

---

#### c) Artportalen_mimic 21.06.2023
- **Content:** Raw records of mimic hoverflies from Sweden.
- **Notes:** Swedish headings translated into English.

**Key Variables:**  
- **Id**: Unique record ID  
- **Taxon Sort Order**: Taxonomic display order  
- **Validation status**: Validation review status  
- **Red list**: Conservation status (Swedish red list)  
- **Taxon id**: Internal taxon identifier  
- **Taxon Name**: Common name (Swedish)  
- **Scientific Taxon Name**: Full scientific name  
- **Auctor**: Author of species description  
- **Quantity**: Number of individuals observed  
- **Unit**: Unit of measure  
- **Stage**: Life stage (adult, larva)  
- **Gender**: Sex (if known)  
- **Activity**: Observed behavior  
- **Discovery method**: Method of observation  
- **Parent Site**: Broader site group  
- **Site name**: Specific observation site  
- **Longitude / Latitude**: Coordinates (decimal degrees)  
- **Accuracy / Diffusion**: Precision of spatial data  
- **County / Municipality / County2 / Parrish**: Administrative regions  
- **Start date/time, End date/time**: Observation timepoints  
- **Public/Private comment**: Comments  
- **Not recovered, Uncertain determination**: Uncertainty flags  
- **Determination method, Biotope, Biotope description**: Habitat and ID details  
- **Determiner, Confirmator**: Identifiers and verifiers  
- **Owner, Submitted by, Observers**: Dataset and observer metadata  
- **Link to BOLD/GenBank**: Genetic data links  
- **Project name**: Associated project

---

#### d) Artportalen_model 21.06.2023
- **Content:** Raw records of model bumblebees from Sweden.
- **Notes:** Follows the same format as (c).

---

#### e) NorSwe_usable data
- **Content:**  
  Cleaned and merged dataset combining usable records from Norway and Sweden for both models and mimics, after filtering queried records.
- **Variables:**  
  Same as described above.

---

### Notes on Missing Data
- Cells marked as **N/A** indicate that no data was available from the original databases.
- These missing values reflect real gaps in source databases, not errors in processing.

---

## 2) ModelMimics_raw

**Description:**  
Contains the merged and cleaned records used for all statistical analyses in the accompanying R-code file.

- **File Format:** CSV

**Key Columns:**  
- **Species**: Name of the species  
- **Taxon**: "Tovinger" (hoverfly mimic) or "Veps" (bumblebee model)  
- **Longitude**: Decimal degrees  
- **Latitude**: Decimal degrees  
- **Precision**: Accuracy of spatial coordinates  
- **count**: Number of individuals observed  
- **elevation**: Elevation (meters)  
- **ordinal**: Julian day of the year  
- **date**: Calendar date of observation  
- **year**: Year of observation  

---

### Note to Users
We recommend using the **ModelMimics_raw** dataset for analyses, as it contains cleaned and harmonized data.  
For raw, unprocessed records, refer to tabs in the **ModelMimics_raw data** Excel spreadsheet.

---
