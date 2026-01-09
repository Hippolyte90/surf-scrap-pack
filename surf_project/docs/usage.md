# surf-scrap – User Guide

## Description
This package allows you to scrape surf conditions from surf-report.com.

## Function
`scrape_surf_report(url, output_csv)`

- `url`: URL of the surf report page
- `output_csv`: path where the CSV file will be saved

## Example

```python
from surf_scrap import scrape_surf_report

df = scrape_surf_report(
    "https://www.surf-report.com/meteo-surf/moliets-plage-centrale-s102799.html",
    "moliets.csv"
)

print(df.head())