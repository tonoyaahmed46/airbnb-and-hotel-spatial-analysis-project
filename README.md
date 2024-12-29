# Spatial Analysis Project - Airbnb and Hotels in Popular Tourist Destinations in CA

## This project answers the following questions: 
- Is there a higher concentration of Airbnb and hotels in California surrounding popular tourist destinations?
- Are there areas with higher tourist attractions and a lack of Airbnbs?

## Significance of project: 

This project is important because it can help us understand tourist behavior and their hospitality preferences. The primary business case this project can solve is whether or not certain parts of California are more profitable than others for hospitality. There are two possible expected audiences. One expected audience group is hotel/Airbnb owners. They can use this information to decide which part of California would be most profitable when considering where to buy land or a house for their business. The other expected audience group is tourists. They can use this information to see which tourist destinations have the most convenient and nearby lodging. From the distribution of hotels and Airbnb’s, they can also deduce the popularity of a particular tourist area, and approximate how many other tourists are usually in the area.

## Data sources 

Airbnb dataset: This dataset is a compilation of datasets from Airbnb containing spatial and temporal data about the location and other describing factors of the Airbnb. 

Tourist Dataset: This source provides OpenStreetMap data specific to Tourist Attractions in California, offering various GIS/CAD formats and thematic layers.

Hotel Dataset: This dataset is a compilation of all addresses of hotels in the State of California.


Airbnb dataset:    

https://www.kaggle.com/datasets/kritikseth/us-airbnb-open-data?resource=download 

Tourist Attractions:

https://mygeodata.cloud/data/download/osm/tourist-attractions/united-states-of-america--california

Hotel Data:

https://ucsdonline.maps.arcgis.com/home/item.html?id=87a655a8d6b8439290e899cb24061f86


When we first obtained all this data, our expectation was that we would have data for the entire state of California. Such is the case for the Hotel and Tourist Attraction data. However, for the Airbnb data, we are limited to Airbnbs in more densely populated areas within California, such as more metropolitan cities and counties (i.e Santa Clara County, Los Angeles etc.). If we were able to obtain all Airbnb locations within California, this would help our project, since we would have better analyses on locations where there are Airbnbs and hotels near tourist destinations. Since we may try to identify areas where there is a shortage of Airbnbs, the results might be biased due to lack of data.

## Background and Literature

- Dubetz, Alissa, et al. “Staying Power: The Effects of Short-Term Rentals on California’s Tourism Economy and Housing Affordability.” Milken Institute. https://milkeninstitute.org/sites/default/files/2022-05/Short_Term_Rentals_California.pdf
This paper explains that short term rentals (like Airbnbs) frequent popular tourist destinations, have a very strong impact on the local economies of those areas, which in turn, expands the number of tourists that area can accommodate.

- Lehr, Dean D., "An Analysis of the Changing Competitive Landscape in the Hotel Industry Regarding Airbnb" (2015). Graduate Master's Theses, Capstones, and Culminating Projects. 188. https://doi.org/10.33015/dominican.edu/2015.bus.01
This paper explains that Airbnb and hotels have to split the same target market and have to focus on the same competitive landscape. This could be confirmed by analyzing the geospatial proximity of Airbnb hubs and hotel hubs.

- La, L., Xu, F., Hu, M. and Xiao, C., 2022. Location of Airbnb and hotels: The spatial distribution irbbs al and relationships. Tourism Review, 77(1), pp.209-224. https://www.emerald.com/insight/content/doi/10.1108/TR-10-2020-0476/full/html
The paper investigates the spatial distribution of Airbnb and hotels in London, analyzing their relationship with demographic, socioeconomic, and environmental factors. Utilizing data from Insideairbnb.com, the study employs geo-spatial auto-correlation analysis and spatial econometric models to reveal distinct patterns. It finds that Airbnb dominates peripheral and tourist attraction areas, while hotels coexist with Airbnb in downtown regions. The study extends traditional hotel location models to Airbnb, shedding light on the differing factors influencing their locations. While limited to London and secondary data, the research offers practical implications for regulating accommodations and guiding Airbnb location choices.

- Leick, B., Kivedal, B. K., Eklund, M. A., & Vinogradov, E. (2022). Exploring the relationship between Airbnb and traditional accommodation for regional variations of tourism markets. Tourism Economics, 28(5), 1258-1279. https://doi.org/10.1177/1354816621990173
This article examines the relationship between Airbnb and traditional accommodations in various tourist destinations across Norway, focusing on both primary and secondary locales. Through exploratory cluster analysis and a panel vector autoregressive (PVAR) model, the study finds significant spillover effects from Airbnb to traditional lodging in secondary destinations. Interestingly, while Airbnb demand positively impacts traditional accommodation demand in the long term, its influence on the supply side of regional tourism markets is relatively small. This suggests that Airbnb growth may stimulate overall tourism sector growth in less-visited areas.

Overall, these references have helped specify our research problem more narrowly by providing insights into the spatial distribution of Airbnb and hotels, their relationship, and their impacts on local economies and tourism sectors. They have also influenced the formulation of hypotheses regarding the concentration of accommodations around tourist destinations in California and the potential implications for hospitality businesses and tourists.

## Packages Needed to Install 

- pandas/geopandas - this will help us organize and manipulate the data

- sklearn - this will help us develop a predictive model to analyze how certain behaviors affect the hospitality/tourism industry

- ArcGIS features, gis, geocoding, geoenrichment, geometry - these modules will help us visualize our data, supplement our data with additional information, and organize the data spatially do be able to draw geographic conclusions
