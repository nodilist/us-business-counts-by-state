# US Business Counts by State (17 CSVs)

This dataset combines 17 CSVs of US business and organization counts, mainly by state, with per-100,000 rates, shares and ranks where available. Nodilist builds these counts from public registers and open map data. The dental files also include estimates of practicing dentists and national candidate-group summaries; the 17 files are not 17 distinct industries. These are aggregate counts only: no business or person names, emails or phones. Contact lists are sold separately at https://nodilist.com/.

Version: 2026-10. Packaged 2026-10-12. Source vintages differ and are described below.

## Files

| File | What one row counts | US total from US row | Source | Release/file date | Nodilist page |
| --- | --- | --- | --- | --- | --- |
| chiropractors-register-2026-10.csv | Registered practice addresses | 105,507 | CMS NPPES Data Dissemination V.2; NUCC provider taxonomy; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/chiropractors/ |
| churches-register-2026-10.csv | Church map listings | 441,834 | Overture Maps Foundation, places theme; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-03 | https://nodilist.com/churches/how-many-churches/ |
| dental-offices-2026-09.csv | Estimated dental offices | 137,112 | BLS QCEW 2025 Q4, private offices of dentists; Census County Business Patterns 2023 (retrieved via Internet Archive); Census Nonemployer Statistics 2024 (context only; retrieved via Internet Archive); CMS NPPES; CMS Medicare Part D Prescribers by Provider, 2024; Overture Maps places, release 2026-09-23.1 | File 2026-09; built 2026-09-29 | https://nodilist.com/dentists/how-many-dentists/ |
| dentists-register-2026-10.csv | Registered practice addresses | 217,576 | CMS NPPES Data Dissemination V.2; NUCC provider taxonomy; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/dentists/ |
| dentists-stats-2026-09.csv | Estimated practicing dentists (people) | 199,887 | CMS NPPES; CMS Medicare Part D Prescribers by Provider, 2024; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-09; built 2026-09-29 | https://nodilist.com/dentists/how-many-dentists/ |
| dso-groups-2026-09.csv | National candidate-group metric per signal | Not applicable (no US row) | CMS NPPES Data Dissemination V.2 | File 2026-09 | https://nodilist.com/guides/what-is-a-dso/ |
| hedge-funds-register-2026-10.csv | Advisers reporting hedge funds | 2,748 | SEC Form ADV registered and exempt reporting adviser files; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/hedge-funds/ |
| hospitals-register-2026-10.csv | Medicare-enrolled hospitals (CCNs) | 5,354 | CMS Hospital General Information; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/hospitals/how-many-hospitals/ |
| optometrists-register-2026-10.csv | Registered practice addresses | 56,070 | CMS NPPES Data Dissemination V.2; NUCC provider taxonomy; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/optometrists/how-many-optometrists/ |
| pharmacies-register-2026-10.csv | Registered pharmacy addresses | 95,345 | CMS NPPES Data Dissemination V.2; NUCC provider taxonomy; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/pharmacies/how-many-pharmacies/ |
| physical-therapists-register-2026-10.csv | Registered practice addresses | 163,990 | CMS NPPES Data Dissemination V.2; NUCC provider taxonomy; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/physical-therapists/how-many-physical-therapists/ |
| physicians-register-2026-10.csv | Registered practice addresses | 482,659 | CMS NPPES Data Dissemination V.2; NUCC provider taxonomy; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/physicians/how-many-doctors/ |
| private-equity-firms-register-2026-10.csv | Advisers reporting private equity funds | 3,114 | SEC Form ADV registered and exempt reporting adviser files; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/private-equity-firms/ |
| ria-firms-register-2026-10.csv | SEC-registered advisers | 14,857 | SEC Form ADV registered adviser file; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/ria-firms/how-many-rias/ |
| trucking-companies-register-2026-10.csv | Active FMCSA carriers with recent MCS-150 filings | 914,701 | FMCSA Company Census File; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/trucking-companies/how-many-trucking-companies/ |
| venture-capital-firms-register-2026-10.csv | Advisers reporting venture capital funds | 2,181 | SEC Form ADV registered and exempt reporting adviser files; US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-04 | https://nodilist.com/venture-capital-firms/ |
| veterinarians-register-2026-10.csv | Veterinary clinic map listings | 41,151 | Overture Maps Foundation, places theme; BLS QCEW 2025 Q4, private veterinary-service establishments (NAICS 541940); US Census Bureau Vintage 2025 state population estimates (July 1, 2025) | File 2026-10; built 2026-10-03 | https://nodilist.com/veterinarians/how-many-veterinarians/ |

Each state file includes the 50 states, DC and a US row. The DSO file contains national summaries. Blank cells are left as published. Files have different schemas and should not be concatenated.

## chiropractors-register-2026-10.csv

Each state row counts distinct registered addresses (address line 1 + ZIP5) of active NPIs in this niche, deduplicated across NPIs. Suite numbers are kept. An active NPI has no deactivation date or was reactivated after it. These are registrations, not open practices; stale, home, billing and duplicate addresses can remain. The US row is the national distinct count. State counts may sum to more because an address + ZIP pair can be recorded in more than one state.

Niche: any of the provider's 15 taxonomy codes matches `(^|\|)111N`; entity types 1, 2 (1 = individual, 2 = organization).

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of registered practice addresses under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.

### Sources

- [CMS NPPES Data Dissemination V.2](https://download.cms.gov/nppes/NPI_Files.html)
- [NUCC provider taxonomy](https://www.nucc.org/index.php/code-sets-mainmenu-41/provider-taxonomy-mainmenu-40/csv-mainmenu-57)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- NPPES counts registrations, not open practices. Records are rarely updated, so closed and moved practices remain; the full register count is an upper bound, and even the 5-year count includes some closed sites.
- Address strings are normalized only by case and spacing; the same site written two ways counts twice.
- Specialty is the taxonomy the provider chose; it is not checked against board certification. A bare parent code (for example "Dentist" or "Pharmacy") is shown as "no specialty given" or "type not given"; in the individual tables, individuals whose primary code is an organization taxonomy (clinic/center) are counted in that row.

Nodilist source page: https://nodilist.com/chiropractors/

## churches-register-2026-10.csv

The headline count is **441,834 church locations**: open places of worship in Overture Maps places (release 2026-09-23.1) whose own category is a Christian place of worship (any tradition under `christian_place_of_worship`), plus places in the generic categories `place_of_worship` and `religious_organization` whose name reads as a church (church, chapel, cathedral, parish, ministry, fellowship, tabernacle, kingdom hall, basilica, mission and similar), deduplicated on normalized name + ZIP5. It is a count of map listings, not of congregations: one congregation can have several listed buildings or listings, and several congregations can share one building.

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of church map listings under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.

### Sources

- [Overture Maps Foundation, places theme](https://docs.overturemaps.org/guides/places/)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-03. See the source page for source-file dates and reproduction details.

Contains data from Overture Maps Foundation, licensed under CDLA Permissive 2.0 (https://cdla.dev/permissive-2-0/).

### Key limits

- Map listings are not a census: the count includes stale and duplicate listings and misses congregations without a listing, so it is neither a congregation count nor a building count.
- Categories come from the map sources and are sometimes wrong; the name rules are simple word matches.
- Overture's confidence score is the source's own estimate that the place exists; it is not a check we ran.

Nodilist source page: https://nodilist.com/churches/how-many-churches/

## dental-offices-2026-09.csv

Each state row estimates dental practice locations where patients are seen. The estimate is the median of four location counts: BLS QCEW, Census CBP, activity-filtered and deduplicated NPPES addresses, and Overture dental listings. The national estimate sums state medians. The national range uses the smallest and largest national source totals. This is a triangulated estimate, not a census. Nonemployer firms are context only and are excluded from the estimate.

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `est_offices`: Median of the four location counts per state; US sums the state medians.
- `est_low`: Smallest of the four source counts; the US row uses national source totals.
- `est_high`: Largest of the four source counts; the US row uses national source totals.
- `qcew_2025q4`: BLS QCEW 2025 Q4 private employer establishments, NAICS 621210.
- `cbp_2023`: Census County Business Patterns 2023 establishments, NAICS 621210.
- `nonemployer_2024`: Census 2024 nonemployer firms, NAICS 6212; context only, excluded from estimate.
- `nppes_candidate`: Candidate NPPES locations grouped by normalized street address + ZIP5.
- `nppes_active`: Candidate locations with at least one activity signal, before exclusions and merging.
- `nppes_active_dedup`: Active locations after institutional-name exclusions and same-phone/ZIP5 merging.
- `overture`: Dental map locations merged by address + ZIP5 (fallback phone or ID), not marked closed, confidence at least 0.5.

### Sources

- [BLS QCEW 2025 Q4, private offices of dentists](https://data.bls.gov/cew/data/api/2025/4/industry/621210.csv)
- [Census County Business Patterns 2023 (retrieved via Internet Archive)](https://www2.census.gov/programs-surveys/cbp/datasets/2023/cbp23st.zip)
- [Census Nonemployer Statistics 2024 (context only; retrieved via Internet Archive)](https://www2.census.gov/programs-surveys/nonemployer-statistics/datasets/2024/historical-datasets/nonemp24st.zip)
- [CMS NPPES](https://download.cms.gov/nppes/NPI_Files.html)
- [CMS Medicare Part D Prescribers by Provider, 2024](https://data.cms.gov/data-api/v1/dataset/14d8e8a9-7e9b-4370-a044-bf97c46b4b44/data)
- [Overture Maps places, release 2026-09-23.1](https://docs.overturemaps.org/guides/places/)

File 2026-09; built 2026-09-29. See the source page for source-file dates and reproduction details.

Contains data from Overture Maps Foundation, licensed under CDLA Permissive 2.0 (https://cdla.dev/permissive-2-0/).

### Key limits

- CBP is 2023 and QCEW is 2025 Q4, while NPPES and Overture are September 2026. Office counts grow slowly (QCEW rose from 136,952 in Q4 2024 to 138,795 in Q4 2025), so the vintage gap is small.
- Census inputs came from Internet Archive captures of the official census.gov files, not directly from census.gov. The file names and paths are the official ones. Verify them directly when census.gov is reachable.
- The institutional exclusion and the phone-based merge are heuristics. They are documented in the script and can be tuned.

Nodilist source page: https://nodilist.com/dentists/how-many-dentists/

## dentists-register-2026-10.csv

Each state row counts distinct registered addresses (address line 1 + ZIP5) of active NPIs in this niche, deduplicated across NPIs. Suite numbers are kept. An active NPI has no deactivation date or was reactivated after it. These are registrations, not open practices; stale, home, billing and duplicate addresses can remain. The US row is the national distinct count. State counts may sum to more because an address + ZIP pair can be recorded in more than one state.

Niche: any of the provider's 15 taxonomy codes matches `(^|\|)(1223|261QD0000X)`; entity types 1, 2 (1 = individual, 2 = organization).

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of registered practice addresses under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.

### Sources

- [CMS NPPES Data Dissemination V.2](https://download.cms.gov/nppes/NPI_Files.html)
- [NUCC provider taxonomy](https://www.nucc.org/index.php/code-sets-mainmenu-41/provider-taxonomy-mainmenu-40/csv-mainmenu-57)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- NPPES counts registrations, not open practices. Records are rarely updated, so closed and moved practices remain; the full register count is an upper bound, and even the 5-year count includes some closed sites.
- Address strings are normalized only by case and spacing; the same site written two ways counts twice.
- Specialty is the taxonomy the provider chose; it is not checked against board certification. A bare parent code (for example "Dentist" or "Pharmacy") is shown as "no specialty given" or "type not given"; in the individual tables, individuals whose primary code is an organization taxonomy (clinic/center) are counted in that row.

Nodilist source page: https://nodilist.com/dentists/

## dentists-stats-2026-09.csv

Each state row estimates practicing dentists among active Type 1 dentist NPIs, using at least one of four activity signals: a record update within five years, enumeration in 2016 or later, an address shared with a recently updated dental organization, or a 2024 Medicare Part D prescriber record. Counts use the primary practice-location state. These are modeled people counts, not organization or office counts. An activity signal does not prove current practice.

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `est_practicing`: Dentist NPIs with at least one activity signal (5-year update, recent enumeration, active organization address or Part D).
- `est_low`: Dentist NPIs updated within three years, enumerated in 2016 or later, or present in Part D 2024.
- `est_high`: Practicing estimate plus no-signal dentist NPIs enumerated in 2008 or later.
- `est_practicing_per_100k`: Practicing estimate divided by population, times 100,000.
- `dentist_npis`: All active Type 1 dentist NPIs; an upper bound.
- `dentist_npis_per_100k`: Active Type 1 dentist NPIs divided by population, times 100,000.
- `dental_org_npis`: Active Type 2 dental organization NPIs.
- `candidate_locations`: Candidate practice addresses grouped by normalized address + ZIP5; an upper bound on practices.
- `sig_updated_5y`: Dentist NPIs updated within the five years before the NPPES file date.
- `sig_updated_3y`: Dentist NPIs updated within the three years before the NPPES file date.
- `sig_enumerated_2016plus`: Dentist NPIs enumerated in 2016 or later.
- `sig_active_org_address`: Dentist NPIs at a candidate address with a dental Type 2 NPI updated within five years before the file date.
- `sig_partd_2024`: Dentist NPIs present in Medicare Part D Prescribers by Provider, 2024.
- `population`: Resident population on July 1, 2025, Census Vintage 2025.
- `population_vintage`: Label for the Census population vintage and reference date.

### Sources

- [CMS NPPES](https://download.cms.gov/nppes/NPI_Files.html)
- [CMS Medicare Part D Prescribers by Provider, 2024](https://data.cms.gov/data-api/v1/dataset/14d8e8a9-7e9b-4370-a044-bf97c46b4b44/data)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-09; built 2026-09-29. See the source page for source-file dates and reproduction details.

License of the published CSV: CC BY 4.0 (attribution: nodilist.com, from CMS and US Census Bureau data).

### Key limits

- Part D suppression (<11 claims) and low prescribing by some specialties undercount activity. A 2024 prescription or a record update doesn't prove practice in September 2026.
- Retired dentists who updated their NPI within 5 years, or who share an address with an active organization, are counted as practicing.
- Per-state counts of NPIs enumerated in the last 12 months looked uneven (New York: 38), so they are not published.

Nodilist source page: https://nodilist.com/dentists/how-many-dentists/

## dso-groups-2026-09.csv

Each row is a national metric for candidate dental groups, not a state row. There is no US row. Active dental NPIs in the 50 states or DC are clustered by normalized practice address (both lines) + ZIP5. Organization NPIs are linked by normalized legal name or by authorized-official name and telephone at two or more locations. These are candidate groupings, not confirmed ownership or DSO affiliation. Group-location links can exceed distinct locations; summary rows count distinct locations. The either signal is the union of both signals.

### Columns

- `table`: Metric table: base, size_distribution or summary.
- `signal`: Linking signal: org_name, auth_official or their union (either); blank for base rows.
- `metric`: Metric identifier: groups per size band, group-location links or distinct locations meeting a group-size threshold.
- `value`: Count for the metric and signal named in the row.
- `share_of_all_locations_pct`: Distinct locations in the summary as a percentage of all candidate locations.

### Sources

- [CMS NPPES Data Dissemination V.2](https://download.cms.gov/nppes/NPI_Files.html)

File 2026-09. See the source page for source-file dates and reproduction details.

### Key limits

- These are **candidate groupings, not confirmed ownership or DSO affiliation**. A DSO's practices usually sit under many dentist-owned legal entities, so this method undercounts DSOs. It also counts groups that are not DSOs, such as dentist-owned group practices, dental schools, community health centers and credentialing back offices.
- The parent-organization field is sparse. Heartland Dental is the parent of only 57 dental NPIs in the file, while its homepage reports 1,900+ supported practices.
- Candidate locations are registrations, not confirmed open practices. In a hand check of 50 random clusters, about 10% were clearly wrong, and about 34% were wrong or unverifiable.
- 69.7% of dental NPI records had not been updated in 5 or more years at the file date.

Nodilist source page: https://nodilist.com/guides/what-is-a-dso/

## hedge-funds-register-2026-10.csv

Each state row counts SEC-registered and exempt reporting advisers reporting hedge funds in Form ADV Item 7.B, with a US main office in the 50 states or DC. Registered advisers have Approved or 120-Day Approval status; exempt reporting advisers have ERA - Active status. Rows are deduplicated by CRD number, keeping the registered row when both files contain it. Exempt reporting advisers are not SEC-registered. Counts are advisers, not distinct funds or parent groups. Filings removed by the documented suspect-filing rules are excluded; withheld main-office states are missing.

The suspect-filing filter removes ERA rows whose exact gross private-fund asset value is not a whole multiple of $1 million and is shared by at least three CRDs, or whose business name contains EXCHANGE or TOKEN, or the word CRYPTO or RWA. The rules can remove legitimate filers and retain doubtful ones.

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of advisers reporting hedge funds under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.

### Sources

- [SEC Form ADV registered and exempt reporting adviser files](https://www.sec.gov/data-research/sec-markets-data/information-about-registered-investment-advisers-exempt-reporting-advisers)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- Form ADV data is self-reported and updated at least once a year; fund counts and gross assets can be up to a year old.
- Private fund advisers registered only with a state securities regulator are not in the SEC files and not in this register.
- A group can file under several advisers (and a fund can be reported by more than one adviser), so groups appear more than once.
- An adviser is counted once, at its main office; branch offices are not counted.

Nodilist source page: https://nodilist.com/hedge-funds/

## hospitals-register-2026-10.csv

Each state row counts distinct CMS Certification Numbers in Hospital General Information, in the 50 states or DC. Repeated Facility IDs are counted once. A CCN can cover several campuses, so this counts certified providers, not buildings. Territories and hospitals not enrolled with Medicare are excluded.

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of medicare-enrolled hospitals (ccns) under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.
- `critical_access`: Hospitals classified by CMS as Critical Access Hospitals.

### Sources

- [CMS Hospital General Information](https://data.cms.gov/provider-data/dataset/xubh-q36u)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- Medicare-enrolled hospitals only. Hospitals that are not enrolled are missing, as are hospitals enrolled after the file date. Federally owned hospitals in the file (205) are close to the American Hospital Association's 210 federal hospitals.
- Hospitals that closed or merged after the file date stay in until CMS removes them.
- One CCN can cover several campuses or a main hospital with satellite locations, so the count is of certified providers, not buildings.
- The file has no inpatient rehabilitation hospital type and lists only 5 long-term rows, so it is not the same count as the American Hospital Association's total of US hospitals.

Nodilist source page: https://nodilist.com/hospitals/how-many-hospitals/

## optometrists-register-2026-10.csv

Each state row counts distinct registered addresses (address line 1 + ZIP5) of active NPIs in this niche, deduplicated across NPIs. Suite numbers are kept. An active NPI has no deactivation date or was reactivated after it. These are registrations, not open practices; stale, home, billing and duplicate addresses can remain. The US row is the national distinct count. State counts may sum to more because an address + ZIP pair can be recorded in more than one state.

Niche: any of the provider's 15 taxonomy codes matches `(^|\|)152W`; entity types 1, 2 (1 = individual, 2 = organization).

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of registered practice addresses under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.

### Sources

- [CMS NPPES Data Dissemination V.2](https://download.cms.gov/nppes/NPI_Files.html)
- [NUCC provider taxonomy](https://www.nucc.org/index.php/code-sets-mainmenu-41/provider-taxonomy-mainmenu-40/csv-mainmenu-57)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- NPPES counts registrations, not open practices. Records are rarely updated, so closed and moved practices remain; the full register count is an upper bound, and even the 5-year count includes some closed sites.
- Address strings are normalized only by case and spacing; the same site written two ways counts twice.
- Specialty is the taxonomy the provider chose; it is not checked against board certification. A bare parent code (for example "Dentist" or "Pharmacy") is shown as "no specialty given" or "type not given"; in the individual tables, individuals whose primary code is an organization taxonomy (clinic/center) are counted in that row.

Nodilist source page: https://nodilist.com/optometrists/how-many-optometrists/

## pharmacies-register-2026-10.csv

Each state row counts distinct registered addresses (address line 1 + ZIP5) of active NPIs in this niche, deduplicated across NPIs. Suite numbers are kept. An active NPI has no deactivation date or was reactivated after it. These are registrations, not open practices; stale, home, billing and duplicate addresses can remain. The US row is the national distinct count. State counts may sum to more because an address + ZIP pair can be recorded in more than one state.

Niche: any of the provider's 15 taxonomy codes matches `(^|\|)3336`; entity types 2 (1 = individual, 2 = organization).

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of registered pharmacy addresses under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.

### Sources

- [CMS NPPES Data Dissemination V.2](https://download.cms.gov/nppes/NPI_Files.html)
- [NUCC provider taxonomy](https://www.nucc.org/index.php/code-sets-mainmenu-41/provider-taxonomy-mainmenu-40/csv-mainmenu-57)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- NPPES counts registrations, not open practices. Records are rarely updated, so closed and moved practices remain; the full register count is an upper bound, and even the 5-year count includes some closed sites.
- Address strings are normalized only by case and spacing; the same site written two ways counts twice.
- Specialty is the taxonomy the provider chose; it is not checked against board certification. A bare parent code (for example "Dentist" or "Pharmacy") is shown as "no specialty given" or "type not given"; in the individual tables, individuals whose primary code is an organization taxonomy (clinic/center) are counted in that row.

Nodilist source page: https://nodilist.com/pharmacies/how-many-pharmacies/

## physical-therapists-register-2026-10.csv

Each state row counts distinct registered addresses (address line 1 + ZIP5) of active NPIs in this niche, deduplicated across NPIs. Suite numbers are kept. An active NPI has no deactivation date or was reactivated after it. These are registrations, not open practices; stale, home, billing and duplicate addresses can remain. The US row is the national distinct count. State counts may sum to more because an address + ZIP pair can be recorded in more than one state.

Niche: any of the provider's 15 taxonomy codes matches `(^|\|)(2251|261QP2000X)`; entity types 1, 2 (1 = individual, 2 = organization).

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of registered practice addresses under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.

### Sources

- [CMS NPPES Data Dissemination V.2](https://download.cms.gov/nppes/NPI_Files.html)
- [NUCC provider taxonomy](https://www.nucc.org/index.php/code-sets-mainmenu-41/provider-taxonomy-mainmenu-40/csv-mainmenu-57)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- NPPES counts registrations, not open practices. Records are rarely updated, so closed and moved practices remain; the full register count is an upper bound, and even the 5-year count includes some closed sites.
- Address strings are normalized only by case and spacing; the same site written two ways counts twice.
- Specialty is the taxonomy the provider chose; it is not checked against board certification. A bare parent code (for example "Dentist" or "Pharmacy") is shown as "no specialty given" or "type not given"; in the individual tables, individuals whose primary code is an organization taxonomy (clinic/center) are counted in that row.

Nodilist source page: https://nodilist.com/physical-therapists/how-many-physical-therapists/

## physicians-register-2026-10.csv

Each state row counts distinct registered addresses (address line 1 + ZIP5) of active NPIs in this niche, deduplicated across NPIs. Suite numbers are kept. An active NPI has no deactivation date or was reactivated after it. These are registrations, not open practices; stale, home, billing and duplicate addresses can remain. The US row is the national distinct count. State counts may sum to more because an address + ZIP pair can be recorded in more than one state.

Niche: any of the provider's 15 taxonomy codes matches `(^|\|)(207|208)`; entity types 1, 2 (1 = individual, 2 = organization).

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of registered practice addresses under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.

### Sources

- [CMS NPPES Data Dissemination V.2](https://download.cms.gov/nppes/NPI_Files.html)
- [NUCC provider taxonomy](https://www.nucc.org/index.php/code-sets-mainmenu-41/provider-taxonomy-mainmenu-40/csv-mainmenu-57)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- NPPES counts registrations, not open practices. Records are rarely updated, so closed and moved practices remain; the full register count is an upper bound, and even the 5-year count includes some closed sites.
- Address strings are normalized only by case and spacing; the same site written two ways counts twice.
- Specialty is the taxonomy the provider chose; it is not checked against board certification. A bare parent code (for example "Dentist" or "Pharmacy") is shown as "no specialty given" or "type not given"; in the individual tables, individuals whose primary code is an organization taxonomy (clinic/center) are counted in that row.

Nodilist source page: https://nodilist.com/physicians/how-many-doctors/

## private-equity-firms-register-2026-10.csv

Each state row counts SEC-registered and exempt reporting advisers reporting private equity funds in Form ADV Item 7.B, with a US main office in the 50 states or DC. Registered advisers have Approved or 120-Day Approval status; exempt reporting advisers have ERA - Active status. Rows are deduplicated by CRD number, keeping the registered row when both files contain it. Exempt reporting advisers are not SEC-registered. Counts are advisers, not distinct funds or parent groups. Filings removed by the documented suspect-filing rules are excluded; withheld main-office states are missing.

The suspect-filing filter removes ERA rows whose exact gross private-fund asset value is not a whole multiple of $1 million and is shared by at least three CRDs, or whose business name contains EXCHANGE or TOKEN, or the word CRYPTO or RWA. The rules can remove legitimate filers and retain doubtful ones.

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of advisers reporting private equity funds under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.

### Sources

- [SEC Form ADV registered and exempt reporting adviser files](https://www.sec.gov/data-research/sec-markets-data/information-about-registered-investment-advisers-exempt-reporting-advisers)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- Form ADV data is self-reported and updated at least once a year; fund counts and gross assets can be up to a year old.
- Private fund advisers registered only with a state securities regulator are not in the SEC files and not in this register.
- A group can file under several advisers (and a fund can be reported by more than one adviser), so groups appear more than once.
- An adviser is counted once, at its main office; branch offices are not counted.

Nodilist source page: https://nodilist.com/private-equity-firms/

## ria-firms-register-2026-10.csv

Each state row counts SEC-registered investment advisers with Approved or 120-Day Approval status and a main office in the 50 states or DC. This is not every US RIA: state-registered advisers, exempt reporting advisers and firms whose main office is withheld are excluded. A firm is counted at its main office, not at its branches.

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of sec-registered advisers under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.

### Sources

- [SEC Form ADV registered adviser file](https://www.sec.gov/data-research/sec-markets-data/information-about-registered-investment-advisers-exempt-reporting-advisers)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- Form ADV data is self-reported and updated at least once a year; assets and employee counts can be up to a year old.
- A firm is counted once, at its main office; branch offices are not counted.
- Summed regulatory assets under management double-count assets that more than one adviser reports (for example a sub-adviser and the adviser that hired it); the total is a sum of filings, not the size of the market.
- Firms with a withheld main office address are missing from the state counts (see above).

Nodilist source page: https://nodilist.com/ria-firms/how-many-rias/

## trucking-companies-register-2026-10.csv

Each state row counts active FMCSA-registered carriers with an MCS-150 update in the 24 months before the file date, at their US physical address in the 50 states or DC. This includes passenger carriers, intrastate-only USDOT carriers and private fleets, as well as for-hire trucking. An active USDOT number does not establish operating authority or that trucks are on the road. This is not a count of every US trucking company.

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of active fmcsa carriers with recent mcs-150 filings under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.
- `new_12m`: Register carriers whose USDOT number was added in the 12 months before the file date.
- `one_truck_pct`: Percentage of register carriers reporting one power unit on the latest MCS-150.
- `intrastate_pct`: Percentage of register carriers classified as intrastate-only.

### Sources

- [FMCSA Company Census File](https://data.transportation.gov/Trucking-and-Motorcoaches/Company-Census-File/az4n-8mr2)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- The census covers USDOT-registered entities, not every truck operator; intrastate-only carriers in states that do not require a USDOT number are missing.
- MCS-150 figures are self-reported and can be up to two years old; fleet size can lag.
- Status A means the USDOT number is active, not that trucks are on the road or that the carrier holds operating authority.
- A carrier is counted once, at its physical address; terminals and depots are not counted. A broker authority is counted once per docket; a company with two dockets counts twice.

Nodilist source page: https://nodilist.com/trucking-companies/how-many-trucking-companies/

## venture-capital-firms-register-2026-10.csv

Each state row counts SEC-registered and exempt reporting advisers reporting venture capital funds in Form ADV Item 7.B, with a US main office in the 50 states or DC. Registered advisers have Approved or 120-Day Approval status; exempt reporting advisers have ERA - Active status. Rows are deduplicated by CRD number, keeping the registered row when both files contain it. Exempt reporting advisers are not SEC-registered. Counts are advisers, not distinct funds or parent groups. Filings removed by the documented suspect-filing rules are excluded; withheld main-office states are missing.

The suspect-filing filter removes ERA rows whose exact gross private-fund asset value is not a whole multiple of $1 million and is shared by at least three CRDs, or whose business name contains EXCHANGE or TOKEN, or the word CRYPTO or RWA. The rules can remove legitimate filers and retain doubtful ones.

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of advisers reporting venture capital funds under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.

### Sources

- [SEC Form ADV registered and exempt reporting adviser files](https://www.sec.gov/data-research/sec-markets-data/information-about-registered-investment-advisers-exempt-reporting-advisers)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-04. See the source page for source-file dates and reproduction details.

### Key limits

- Form ADV data is self-reported and updated at least once a year; fund counts and gross assets can be up to a year old.
- Private fund advisers registered only with a state securities regulator are not in the SEC files and not in this register.
- A group can file under several advisers (and a fund can be reported by more than one adviser), so groups appear more than once.
- An adviser is counted once, at its main office; branch offices are not counted.

Nodilist source page: https://nodilist.com/venture-capital-firms/

## veterinarians-register-2026-10.csv

The register count is **41,151 veterinary clinic locations listed on public maps (Overture, 2026-09-23.1)**: places whose own category is veterinary care, plus generic animal-service places whose name reads as a veterinary practice, deduplicated on normalized name + ZIP5. It counts map listings, not practices or veterinarians: a practice with two listings counts twice until deduplication catches it, and a practice with no listing is missing. The official count of veterinary businesses is the BLS QCEW figure below; pages headline that and show this map count second.

### Columns

- `state`: Two-letter state code, DC, or US for the national row.
- `state_name`: State or national area name.
- `orgs`: Count of veterinary clinic map listings under the definition above.
- `per_100k`: Count per 100,000 residents, using Census Vintage 2025 population.
- `share_pct`: State count as a percentage of the sum of the 51 state counts; US is 100.
- `rank`: State's rank by count among the 50 states and DC (1 = most; ties broken by state code); blank for US.
- `qcew_estabs`: BLS QCEW 2025 Q4 private establishments in NAICS 541940 Veterinary services.

### Sources

- [Overture Maps Foundation, places theme](https://docs.overturemaps.org/guides/places/)
- [BLS QCEW 2025 Q4, private veterinary-service establishments (NAICS 541940)](https://data.bls.gov/cew/data/api/2025/4/industry/541940.csv)
- [US Census Bureau Vintage 2025 state population estimates (July 1, 2025)](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/state/totals/NST-EST2025-ALLDATA.csv)

File 2026-10; built 2026-10-03. See the source page for source-file dates and reproduction details.

Contains data from Overture Maps Foundation, licensed under CDLA Permissive 2.0 (https://cdla.dev/permissive-2-0/).

### Key limits

- Map listings are not a census: the count includes stale and duplicate listings and misses practices without a listing.
- Categories come from the map sources and are sometimes wrong; the name rules are simple whole-word matches.
- Overture's confidence score is the source's own estimate that the place exists; it is not a check we ran.
- Neither source counts veterinarians by state; the AVMA figure is national and counts people.

Nodilist source page: https://nodilist.com/veterinarians/how-many-veterinarians/

## License

Nodilist counts are licensed under Creative Commons Attribution 4.0 International (CC BY 4.0): https://creativecommons.org/licenses/by/4.0/. Credit Nodilist and keep the third-party data credits given in each file section and in LICENSE. The 2020 U.S. Religion Census congregation figures cited on nodilist.com's church pages are not included (ASARB, all rights reserved). This package contains aggregate statistics, not upstream contact records.

## How to cite

Nodilist (2026). US Business Counts by State (17 CSVs) (Version 2026-10) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.23325480

```bibtex
@misc{nodilist_us_business_counts_2026,
  author = {Nodilist},
  title = {US Business Counts by State (17 CSVs)},
  year = {2026},
  version = {2026-10},
  doi = {10.5281/zenodo.23325480},
  url = {https://nodilist.com/}
}
```

## Updates

Updated about once a month, as sources are re-read and reviewed. A package release does not imply that every source was refreshed. Follow the source-page links above for definitions, source dates and reproduction instructions.

## Contact

info@nodilist.com
