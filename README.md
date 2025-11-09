# Coins-Roman-Britain_Tableau
This dashboard shows Roman coin finds from England and Wales, based on the “Coin corpus divided by ABCDEF Phase by parish” dataset. It focuses on coins dated between c. AD 260–402, organized into five historical phases (A–E).

Spatial Coverage: England and Wales (United Kingdom)
Temporal Coverage: c. AD 260–402, divided into Periods A, B, C, D, and E
Data Source: Archaeology Data Service (ADS)
Original Author: Richard Henry
Dataset DOI/ID: Henry, R. (2023). Coin corpus divided by ABCDEF Phase by parish [digital object]. York: Archaeology Data Service. Object ID: 2362226
Link to Source: https://archaeologydataservice.ac.uk/archives/collections/view/1005487/index.cfm 

Data Acquisition & Extraction:
Data downloaded from the Archaeology Data Service (ADS) as provided by Richard Henry (2023).


Source dataset includes parish-level quantification of Roman coin finds categorized by Periods A–F.


For this dashboard, only coins dated to Periods A–E (c. AD 260–402) were included.


Data Cleaning & Preparation:
Standardization of column names to maintain consistency.


Removal of period F as per research scope.


Recalculation of the column “Total quantity”, considering only Periods A through E. 


Validated and retained ADS-provided geographic coordinates (lat/long) for geospatial plotting.


No additional data manipulation or inference beyond the supplied dataset.


Data Modelling & Visualization Methodology:
TOP 10 Counties (Total Quantity of Coins)
The “County” field was placed on the Rows shelf to list each county, and the “Total Quantity (ABCDE)” field was placed on the Columns shelf to measure coin counts.


The “Total Quantity (ABCDE)” value was aggregated using SUM, ensuring that the chart reflects the combined coin quantities from all five periods (A–E), dating c. AD 260–402.


A filter was applied to the County field to display only the Top 10 counties with the highest total number of coins, allowing users to quickly identify the areas with the greatest coin concentrations.


This visual highlights regional disparities in coin circulation and helps users compare which counties had the strongest representation of Roman coinage within the dataset.


Coins by Historical Period
This visual displays the total number of coins recorded for each historical period (A–E), covering c. AD 260–402.


The chart was built using the Measure Names field on the Columns shelf and Measure Values on the Rows shelf.


A Measure Names filter was applied to include only the five relevant fields:
 Quantity_Period_A, Quantity_Period_B, Quantity_Period_C, Quantity_Period_D, and Quantity_Period_E.


Each measure was aggregated using SUM, allowing the chart to show the total number of coins found across all parishes for each period.

A chronological order was applied to the Measure Names filter to ensure periods A–E appear in sequence.


The Marks card was set to Line, with each period assigned a different colour to visually distinguish the temporal changes in coin quantities.


The final visual provides a clear overview of how coin circulation fluctuated through late Roman historical periods across England and Wales.

Social category Proportion
This visual represents the proportion of Major Social Categories identified in the dataset, based on the classifications provided by the original author.


The field “Major social category” was used to group the sites, and CNT (Count) was applied to measure how many parishes belong to each category.


A donut chart format was selected to clearly show the relative distribution of social categories across all recorded sites.


To maintain clarity and focus on the most relevant categories, two categories (“Other” and “Non-identified”) were removed from the visual.


The result highlights the dominant types of settlements represented in the dataset, allowing users to quickly understand the social context of the coin-find locations.

TOP 20 Parishes (Total Quantity of Coins)
The field “Parish” was placed on the Rows shelf to list each parish, and “Total quantity (ABCDE)” was placed on the Columns shelf, aggregated using SUM to show the total number of coins found per parish.


A Top N filter was applied to the Parish field, set to display only the Top 20 parishes ranked by total coin count.


This ranking uses the combined total across Periods A–E (c. AD 260–402), ensuring comparability between parishes.


The resulting bar chart allows users to quickly identify the parishes with the strongest representation of Roman coins and explore variations in coin deposition intensity across locations.

Parish Locations (England and Wales)
Assigned Latitude and Longitude fields with the correct Geographic Role (Latitude / Longitude).


Dragged Longitude to the Columns shelf and Latitude to the Rows shelf to generate the base map.


Used the Parish field in the Marks → Detail card to label and uniquely identify each mapped location.


Added the field “Total quantity (ABCDE)” to the Size card to scale the map markers based on the total number of coins found per parish.


Adjusted marker size and formatting for clarity and visual hierarchy.


Resulting map visualisation displays parish-based coin distribution across England and Wales, enabling users to identify spatial patterns and locations with higher or lower coin concentrations.


