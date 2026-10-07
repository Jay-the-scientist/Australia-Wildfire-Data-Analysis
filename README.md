# Australia Wildfires Analysis

**Exploring historical wildfire activity across Australia through data analysis and visualization.**

## Overview

How has wildfire activity changed across Australia over time? Do different regions experience different patterns in fire activity and intensity?

This project explores these questions using historical Australian wildfire data, examining changes in estimated fire area, regional differences, and fire-related measurements.

Using Python, I analyzed wildfire observations and created visualizations to better understand how fire activity varies over time and across different parts of Australia.

## Dataset

The project uses the **Historical Wildfires** dataset provided through IBM Skills Network, containing fire activity observations across seven Australian regions beginning in 2005.

The dataset is based on satellite-derived fire measurements and includes:

- **Estimated fire area:** Estimated area associated with detected vegetation fires, measured in square kilometers
- **Fire brightness:** Temperature-related measurements from detected fire pixels, measured in Kelvin
- **Radiative power:** Estimated energy emitted by detected fires, measured in megawatts
- **Detection confidence:** Confidence associated with the fire observations
- **Region and date:** Geographic region and observation date
- **Fire pixel count:** Number of pixels flagged as presumed vegetation fires

The analysis focuses on understanding how these measurements change across time and geographic regions.

**Data source:** [IBM Skills Network — Historical Wildfires Dataset](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0101EN-SkillsNetwork/Data%20Files/Historical_Wildfires.csv)

## Exploring Wildfire Activity Over Time

To understand how wildfire activity changed over the years, I grouped the observations by year and month and calculated the average estimated fire area.

The analysis revealed noticeable changes in estimated fire area over time, including a period of elevated activity around 2011–2012.

Examining the data at a monthly level provided a closer look at when these changes occurred.

![Average Estimated Fire Area by Month and Year](images/5-estimated-fire-over-time-by-month-and-year.png)

**Key takeaway:** Wildfire measurements fluctuate over time, and examining monthly patterns can reveal changes that are less apparent in annual summaries.

## Comparing Australia's Regions

Wildfire characteristics can vary significantly across different geographic regions.

This analysis covers seven Australian regions:

- New South Wales (NSW)
- Northern Territory (NT)
- Queensland (QL)
- South Australia (SA)
- Tasmania (TA)
- Victoria (VI)
- Western Australia (WA)

To compare these regions, I examined the distribution of estimated fire brightness using histograms and regional comparisons.

![Distribution of Estimated Fire Brightness Across Australian Regions](images/11-stacked-distribution-of-estimated-fire-brightess-across-regions.png)

The stacked histogram illustrates how recorded fire brightness measurements are distributed across the seven regions.

**Key takeaway:** Comparing regional distributions provides a more detailed view of wildfire measurements than looking only at national averages.

## Mapping Australia's Regions

To provide geographic context for the analysis, I created an interactive map using **Folium**.

The map identifies the seven Australian regions included in the dataset using geographic markers.

![Australian Regions Visualized with Folium](images/14-regions-marked-in-folium.png)

The map provides a geographic reference for understanding the regions represented in the analysis. The markers identify regions rather than individual wildfire locations.

## Technologies Used

- **Python** — Data analysis and visualization
- **Pandas & NumPy** — Data preparation, grouping, and aggregation
- **Matplotlib & Seaborn** — Statistical charts and visualizations
- **Folium** — Interactive geographic mapping
- **Jupyter Notebook** — Interactive data exploration

## Skills Demonstrated

- Exploratory data analysis
- Working with historical and time-based data
- Data grouping and aggregation
- Time-series visualization
- Regional comparisons
- Statistical data visualization
- Geographic data visualization
- Communicating findings through charts

## Project Context

This project was completed as part of the **IBM Data Visualization coursework**, providing hands-on experience analyzing and presenting historical environmental data.

The analysis demonstrates how different visualization techniques can be used to explore temporal, regional, and measurement-related patterns in a dataset.

The project focuses on understanding and communicating historical wildfire observations rather than predicting future wildfire events.
