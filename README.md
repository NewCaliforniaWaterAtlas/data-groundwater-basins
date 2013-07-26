# California Groundwater Basins Dataset - Version 0.0.5
--------------------------------------------------------------------------------

THIS IS A WORK IN PROGRESS. We will note when this document is final. 7/26/2013 -- laci videmsky

--------------------------------------------------------------------------------

The Department of Water Resources (DWR) maintains a dataset of groundwater elevation data, and makes it available through their data and mapping portal "California Statewide Groundwater Elevation Monitoring (CASGEM)"

We are working to create a dataset that is developer-friendly, accurate, up-to-date and well-documented. We believe this will help to speed communication and promote clarity and innovation about water usage in the State. We began in December 2012, and are doing more improvements in Summer 2013. Please watch this Github repository for updates. We would like to have a great & re-usable dataset worked out by January 2014.


data-groundwater-basins
==============================

Groundwater Basin Descriptions


From the California Department of Water Resources's description of this data:

"Out of 431 delineated groundwater basins, 24 basins are subdivided to create an additional 108 subbasins. These 515 distinct groundwater systems underlie about 40 percent of the surface area of the State."

"Many of the subbasin boundaries were developed or modified with public input, but little physical data. Because they should not be considered precise boundaries, a detailed local study should determine whether any specific area lies within a groundwater basin boundary."

PDFs of each groundwater basin and sub-basin can be found on DWR's site here:
http://www.water.ca.gov/groundwater/bulletin118/gwbasin_maps_descriptions.cfm


--------------------------------------------------------------------------------
** FIELDS **
--------------------------------------------------------------------------------

## Fields - Unique Identifiers

### Below needs to be formatted:


DWR_

DWR Number - includes hydrologic region number in first position.

SUBBSN_

DWR subbasin number only.

BAS_SBBSN

Combined field of basin and subbasin number.

GWBASIN

Name of groundwater basin.

BUDGET_TYP

A, B, or C type basin budget, as described in Bulletin 118 (2003)
SUBNAME

Subbasin name, where applicable

REGIONAL_O

DWR Region Office responsible for individual basin delineation and description
1 = Northern
2 = North Central
3 = South Central
4 = Southern

ACRES

Area of basin or subbasin in acres

--------------------------------------------------------------------------------

Additional Information
The basin boundaries for the revised groundwater basin map were primarily defined using geologic contacts and hydrogeologic divides. Specifically the identification of the groundwater basins was initially based on the presence and areal extent of unconsolidated alluvial soils identified on 1:250,000 scale geologic maps provided by the California Department of Conservation, Division of Mines and Geology. The identified groundwater basin areas were then further evaluated through review of relevant geologic and hydrogeologic reports, well completion reports, court-determined adjudicated basin boundaries, and contact with local agencies to refine the basin boundaries.

Metadata Update - December 09, 2010
B118_v3_BasinBoundaries_NAD83_unprojected file was developed from B118v3NAD27UTM10 (dated 15-September-2006) which had a UTM 10 NAD 27 projection. The new file projection is defined as Latitude/Longitude NAD 83 and was converted using ESRI's Project tool in a two step process. Set one changed the Datum from NAD27 to NAD 83. The second step was to re-project the file from Universal Transverse Mercator 10 to Lat/Long Geographic projection for the use of CASGEM.

Metadata Update – June 20, 2012
The shapefile B118_BasinBoundaries_v4_1.shp  replaces B118_v3_BasinBoundaries_NAD83_unprojected.shp.   Changes in the update include restoration of the northern portion of the North Yuba subbasin which was inadvertently removed during the 2003 B-118 Update.  Also, the DWR District field (DWR_DIST) in the feature attribute table has been replaced by Regional Office Field (Regional_O).  Basin boundary features in previous versions that were comprised of multiple polygons are now represented by single multi-part polygons.