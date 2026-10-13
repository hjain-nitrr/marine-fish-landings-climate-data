# Marine fish landing and sea-surface temperature data

Data accompanying **Dynamics of Marine Fish Landing under Sea-Surface Warming and Extreme Weather Events**.

## Files

- [Original workbook](Quarterly_Fish_Landings_2018_2025_With_Formulas.xlsx): the author-supplied Excel file, preserved byte-for-byte. The repository filename reflects the actual **2018–2025** coverage; the supplied workbook was originally named with 2013–2025.
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

The manuscript attributes the landing data to CMFRI in Reference 39 and describes reconstruction from annual totals and quarterly percentages in Section 4. The authors identify CMFRI annual marine fish landing booklets as the source of the quarterly percentages. The 2021 booklet is available at https://eprints.cmfri.org.in/16042/1/Marine%20Fish%20Landings%20in%20India%202021.pdf; its printed page 13 contains the Gujarat and Maharashtra quarterly charts. A complete year-by-year verification of the transcribed percentages has not been performed. Two rows do not reconcile with their annual totals:

| State and year | Supplied Q1–Q4 fractions | Sum | Sum of derived quarters (tonnes) | Annual total (tonnes) |
|---|---|---:|---:|---:|
| Gujarat, 2021 | 0.14, 0.12, 0.06, 0.38 | 0.70 | 403491.2 | 576416 |
| Kerala, 2018 | 0.20, 0.22, 0.33, 0.26 | 1.01 | 649005.8 | 642580 |

All other rows sum to 1.00 within floating-point tolerance. The Kerala difference may reflect rounding, but its cause has not been established. The official 2021 booklet (printed page 13) lists Gujarat quarterly shares as 44%, 12%, 6% and 38%; the supplied workbook instead contains 14% for Q1. This is a source-to-workbook discrepancy, preserved here to document the supplied analytical input. Neither row has been changed. This deposit documents the supplied analytical input; it does not certify that the dataset is error-free. Any later correction should be versioned and its effect on the analysis assessed.

## Sea-surface temperature data

- [Original SST workbook](WESTERN_COAST_SST_MONTHLY.xlsx): the workbook explicitly identified by the author as the SST input used in this study; preserved byte-for-byte.
- [Monthly SST CSV](western_coast_sst_monthly.csv): a machine-readable copy with dates formatted as YYYY-MM-DD. All temperatures and column labels are unchanged.

The workbook contains 113 consecutive monthly records from June 2002 to October 2011 for Kerala, Karnataka, Goa, Maharashtra and Gujarat. Units are degrees Celsius, as indicated in the original headers. There are 565 numeric SST entries with no missing temperatures. The manuscript analyses Kerala, Karnataka, Maharashtra and Gujarat; the original Goa column is retained in the deposited file.

The manuscript identifies INCOIS and NOAA OISST as original SST sources:
- [INCOIS data holdings](https://incois.gov.in/site/dataholdings.jsp)
- [NOAA OISST product and access information](https://www.ncei.noaa.gov/products/optimum-interpolation-sst)

The deposited workbook provides direct access to the regional SST series identified by the author as used in the study. It contains no source product/version identifiers, extraction coordinates or processing notes. Attribution to INCOIS and NOAA follows the manuscript; those upstream details cannot be independently established from the workbook alone. The earlier supplied file named `Indian Costal SST.xlsx` is not the author-designated study input and is not included in this repository.

## Booklet access

- [CMFRI data publications](https://www.cmfri.org.in/data-publications)
- [2021 booklet repository record](https://eprints.cmfri.org.in/16042/)

The workbook and CSV retain the original values. Source corrections have not been applied to model calibration or manuscript results by this deposit.
