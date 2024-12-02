# DEM-Image Pair Extraction

This repo is aimed to process and export paired satellite imagery and DEM data using Google Earth Engine.

## Prerequisites

1. Install dependencies
- Python 3.x
- Google Earth Engine API
- geemap library (for visualization)

```bash
pip install earthengine-api geemap
```

2. Create a [Google Earth Project](https://earthengine.google.com/) with your google account. GEE is free for non-commercial uses. 

## Execution

```bash
python demtexture.py [options]
```
### Options

--aoi lon_min lat_min lon_max lat_max: Area of interest boundary coordinates (default to -122.5 37.0 -121.5 38.0) \
--start-date YYYY-MM-DD: Start date for satellite image data range\
--end-date YYYY-MM-DD: End date for satellite image range\
--cloud-percentage: Maximum cloud coverage percentage\
--export-folder: Google Drive folder for exports\
--export-scale: Scale in meters for exports.\
--project: Google Cloud project ID (if required).\

The script is only tested with USGS/SRTMGL1_003 (DEM) and COPERNICUS/S2_SR (Satellite Image). It is not yet confirmed to work with other datasets.
