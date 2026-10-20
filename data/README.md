# About the dataset(s)

Both files are snapshots of the [KOI Table (Cumulative list)](https://exoplanetarchive.ipac.caltech.edu/cgi-bin/TblView/nph-tblView?app=ExoTbls&config=cumulative) from the [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu/docs/data.html), listed under "Kepler".

For a comprehensive list of the column definitions, see [here](https://exoplanetarchive.ipac.caltech.edu/docs/API_kepcandidate_columns.html).

## Citation

This research has made use of the NASA Exoplanet Archive, which is operated by the California Institute of Technology, under contract with the National Aeronautics and Space Administration under the Exoplanet Exploration Program.

1. NASA Exoplanet Archive. 2025, *Kepler Objects of Interest Cumulative Table*,
   Version: 2025-08-27 14:27, NExScI-Caltech/IPAC. https://doi.org/10.26133/NEA4
   Accessed 2025-08-27, returning 9564 rows.

2. NASA Exoplanet Archive. 2026, *Kepler Objects of Interest Cumulative Table*,
   Version: 2026-10-19 14:13, NExScI-Caltech/IPAC. https://doi.org/10.26133/NEA4
   Accessed 2026-10-19, returning 9564 rows.

## `cumulative_2025.08.27_14.27.30.csv`

This is the raw dataset of shape `(9564, 49)` that is used in `v1_original.ipynb`, downloaded on 2025-08-27 at 14:27:30. When downloading, the following options were selected:
- CSV format
- Download Currently Checked Columns (default upon opening site)
- Download Currently Checked Rows (default upon opening site)

## `cumulative_2026.10.19_14.13.25.csv`

This is the raw dataset of shape `(9564, 141)` that is used in `v2_candidate_ranking.ipynb`, downloaded on 2026-10-19 at 14:13:25. When downloading, the following options were selected:
- CSV format
- Download all columns
- Download all rows

The archive table changes over time, so the exact files are committed to keep results reproducible. The newer dataset is used to check which Candidates were resolved after Aug 2025.

## Data Loading

Each file starts with metadata lines prefixed with `#`. Skip them with: 
```python
pd.read_csv('../data/cumulative_2026.10.19_14.13.25.csv', comment='#')
```
