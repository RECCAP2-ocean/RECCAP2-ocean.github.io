---
title: Regional masks
---

## Open ocean regions 
A netCDF file with regional masks is available at [https://github.com/RECCAP2-ocean/R2-shared-resources/blob/master/data/regions/RECCAP2_region_masks_all_v20221025.nc](https://github.com/RECCAP2-ocean/R2-shared-resources/blob/master/data/regions/RECCAP2_region_masks_all_v20221025.nc). This file contains the `open_ocean` mask and the sub-regions for each basin: `atlantic, pacific, indian, arctic, southern`. Further, a `coast` mask is included. All land, or non-valid regions of the masks are set to zero. An additional mask, `seamask`, is a mask for all ocean pixels (based on SST).

We have used the biomes of Fay and McKinley to divide the basins into subregions. 
The areas where FM14 does not have data have been ingested by the neighboring biome or a new distinct biome has been added, as noted in the figure below. Two exceptions are in the Indian and Arctic. In both regions, we have created new biomes based on input from the respective chapter leads. 

![https://raw.githubusercontent.com/RECCAP2-ocean/R2-shared-resources/master/figures/regions/RECCAP2_region_masks_all_v20221025.png](https://raw.githubusercontent.com/RECCAP2-ocean/R2-shared-resources/master/figures/regions/RECCAP2_region_masks_all_v20221025.png)

## Coastal regions
The coastal regions will be the updated MARCATS product used in [Laruelle et al. 2017](https://doi.org/10.5194/bg-14-4545-2017). The extent is defined by the following:

>The outer limit used here is given by whichever point is the furthest from the coast: either 300 km distance from the coastline (which roughly corresponds to the outer edge of territorial waters; Crossland et al., 2005) or the 1000m isobaths (Laruelle et al., 2013). The resulting domain covers 77 million km$^2$. 

## How the global map was created 
Below is a map of the proposed regions for RECCAP v2. Note that the coastal boundaries have not been added to this map. 

The map is annotated to show how boundaries were decided. WOA09 uses the [World Ocean Atlas 09 basins map](https://iridl.ldeo.columbia.edu/SOURCES/.NOAA/.NODC/.WOA09/.Masks/.basin/data.nc). FM14 indicates Fay and McKinley (2014) boundaries were used. Note that the exception is in the Indian Ocean, where boundaries were drawn based on advice from the Indian Ocean Chapter leads. These changes are not shown in the figure below. 

![bas_all](img/ocean_regions/basin_all_wBiomes.png)

Comment on the boundary definition from Luke Gregor:  

>The boundaries are defined in one of three ways: CO2 biomes by Fay and McKinley (2014) (FM14); the WOA (2009) ocean basin map (WOA09); manual decisions. The WOA mask might not be well known, but this doesn’t matter as it serves purely as a convenient way to define the borders.*
>
>Starting from the simplest, the Southern Ocean is defined by FM14. The eastern boundary of the Indian is defined by the WOA09 boundary between the Pacific and Indian. The Red Sea and the Persian Gulf have been masked. Further, the indian ocean has been divided into < 18°S, <0°S and north of this, along the 78° E line. In the North Pacific, the Bearring Strait limit is also defined by WOA09. The Atlantic includes the Mediterranean Sea and Gulf of Mexico. We have chosen to exclude the Baltic Sea as carbon cycling and fluxes are notoriously difficult to predict in the region. The boundary between the Arctic and the Atlantic is defined by FM14 with some modifications. The northern boundary has manually been set to 56°N that limits the extent of FM14's biome in the Labrador Sea. In the far North Atlantic, the eastern extent has been set to 25°E as the most northern extent of Scandinavia.*
