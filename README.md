# NARRDownload

This repo contains a python script to download and extract NARR data.

The script will:
    * Download desired [monolevel](https://psl.noaa.gov/data/gridded/data.narr.monolevel.html) & [subusurface](https://psl.noaa.gov/data/gridded/data.narr.subsurface.html) records for specified time intervals.
    * Parse the data to query values for gridpoints near a specific location and use inverse distantce weighting to interpolate to a specified point.
    * Be careful requesting subsurface variables near coastlines, the interpolation will be based on only the inland gridpoints
