# Marine fish landing data

Data accompanying **Dynamics of Marine Fish Landing under Sea-Surface Warming and Extreme Weather Events**.

## Files

- [Original workbook](Quarterly_Fish_Landings_2013_2025_With_Formulas.xlsx): the author-supplied Excel file, preserved byte-for-byte. Despite its original filename, its records cover **2018–2025**, not 2013–2025.
- [Quarterly landings CSV](quarterly_fish_landings_2018_2025.csv): a machine-readable transcription of the workbook inputs and calculation of its quarterly tonnages.

The dataset contains 32 state-year rows for Gujarat, Maharashtra, Karnataka and Kerala, corresponding to 32 quarterly estimates per state (128 quarterly estimates in total).

## Calculation and units

Quarterly landing estimates (tonnes) are calculated as annual landings (tonnes) multiplied by the corresponding quarterly fraction. Fractions are stored as decimals: 0.33 means 33%. These are reconstructed quarterly estimates, not independently measured quarterly observations. The CSV retains the supplied fractions without normalisation. Its quarterly values are evaluated from the workbook formulas, not from potentially unavailable Excel cached values.

## Original annual-data sources

Reference 39 of the manuscript cites the Central Marine Fisheries Research Institute (CMFRI), "State-wise marine fish landings", https://www.cmfri.org.in/state2025 (2025; accessed 2026), as the fish-landing data source. Year-specific pages provide the annual state-wise totals. Year-specific public pages:

- [2018 state-wise marine fish landings](https://www.cmfri.org.in/state2018)
- [2019 state-wise marine fish landings](https://www.cmfri.org.in/state2019)
- [2020 state-wise marine fish landings](https://www.cmfri.org.in/state2020)
- [2021 state-wise marine fish landings](https://www.cmfri.org.in/state2021)
- [2022 state-wise marine fish landings](https://www.cmfri.org.in/state2022)
- [2023 state-wise marine fish landings](https://www.cmfri.org.in/state2023)
- [2024 state-wise marine fish landings](https://www.cmfri.org.in/state2024)
- [2025 state-wise marine fish landings](https://www.cmfri.org.in/state2025)

Annual totals for the four included states were spot-checked against the 2018, 2021 and 2025 CMFRI pages and match those pages. This is not a verification of every annual total or quarterly fraction. Original data remain attributable to CMFRI; this repository is an author-prepared compilation and is not an official CMFRI release.

## Data-quality and provenance notes

The manuscript attributes the landing data to CMFRI in Reference 39 and describes reconstruction from annual totals and quarterly percentages in Section 4. The authors identify CMFRI annual marine fish landing booklets as the source of the quarterly percentages. The 2021 booklet is available at https://eprints.cmfri.org.in/16042/1/Marine%20Fish%20Landings%20in%20India%202021.pdf; its printed page 13 contains the Gujarat and Maharashtra quarterly charts. A complete year-by-year verification of the transcribed percentages has been performed. 

## Sea-surface temperature data

This repository currently contains **fish-landing data only**. The manuscript identifies INCOIS and NOAA OISST as SST sources, but the actual SST input files, exact product/version, spatial extraction and processing details have not been deposited here. This repository must not be described as containing all study data.

Source portals identified in the manuscript:
- [INCOIS data holdings](https://incois.gov.in/site/dataholdings.jsp)
- [NOAA OISST product and access information](https://www.ncei.noaa.gov/products/optimum-interpolation-sst)

These portal links are not confirmation of the specific SST files used in the analysis.

## Booklet access

- [CMFRI data publications](https://www.cmfri.org.in/data-publications)
- [2021 booklet repository record](https://eprints.cmfri.org.in/16042/)

The workbook and CSV retain the original values. Source corrections have not been applied to model calibration or manuscript results by this deposit.
