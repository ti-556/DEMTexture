# DEM-Image Pair Extraction

This repo is aimed to process and export paired satellite imagery and DEM data using Google Earth Engine.

## Prerequisites

- Python 3.x
- Google Earth Engine API
- geemap library (for visualization)

## Installation

```bash
pip install earthengine-api geemap
```
## Execution

```bash
python script.py [options]
```
### Options

--aoi lon_min lat_min lon_max lat_max: Area of interest boundary coordinates (default to -122.5 37.0 -121.5 38.0) \
--start-date YYYY-MM-DD: Start date for satellite image data range\
--end-date YYYY-MM-DD: End date for satellite image range\
--cloud-percentage: Maximum cloud coverage percentage\
--export-folder: Google Drive folder for exports\
--export-scale: Scale in meters for exports.\
--project: Google Cloud project ID (if required).\
