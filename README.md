# Tree-Coverage-in-Urban-Environments-for-Community-Health-and-Energy-Saving
Sarah Brown
University of Calgary - Department of Geography
sarahkbrown02gmail.com

The purpose of this project was to analyze tree coverage density impacts on surface temperature around calgary and how the presence of trees may be unequal across the city due to income disparities between communities.

Folder Structure:
Land_Surface_Temperature_Calculations contains all ArcGIS layers used to calculate land surface temperature in the city of Calgary from landsat raster data collected from 2020/07/26 and 2022/07/24.
Tables_Created contains attribute table of Calgary_Communities_Data used to create map of income and map of tree are coverage by community, and excel file, Income_TreeCoverage of correlation between tree coverage and income.
Tree Canopy files contain geo_export files of tree coverage in calgary for 2020 and 2022
Community_District_Boundaries is the shapefile of Calgary community boundaries
Landsat images used in the land surface temperatre calculations metadata tables 

Coordinate Reference System: WGS84(DD)

Data Sources: 
Raster data collected via Landsat 8-9 from USGS(.gov) <accessed 2025/10/06>
Calgary community district boundaries collected via data.calgary.ca <accessed 2025/10/07>
Calgary tree canopy coverage 2020 and 2022 collected via data.calgary.ca <accessed 2025/10/07>
Calgary community profiles for median income collected via calgary.ca/communities <accessed 2025/10/23>

Methods:
Landsat raster raw images were used to calculate land surface temperature through a series of python expressions in ArcGIS pro "raster calculator" tool. All layers created found in Land_Surface_Temperature_Calculations file. The final land surface temperature raster layer was overlayed with the Tree Canopy geo_export for the respective year to compare surface temperature in the presence of tree coverage. Calgary community boundaries were used, and median income (2021) was manually added to the attribute table via community profile data, to analyze median income by community. Tree canopy coverage from 2022 and median income from 2021 were compared. Tree canopy coverage and individual community area was calculated by ArcGIS "calculate geometry". In the attribute table for Calgary_Communities_Data percent of area of community polygon covered by each indivual tree canopy coverage polygon was created as a field and summed to find the total percent of tree canopy area coverage by community. These percentages were pulled into the Income_TreeCoverage_Graph to make a corrrelation scatterplot of median income and percent of tree canopy coverage. 



