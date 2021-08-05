# Project: IPO density map 

This is a project for Lede week 9.  
Using an IPO company list I obtained, analyzed IPO density based on geographics, visualized with mapbox.
---
## Background
In late 2020, tech nerds have argued whether the "San Francisco exodus" is real or not.  Some people who moved to places like Texas said, "We live in  Zoom era, location doesn't matter.", but others did not agree to this idea.
For example, an investor Sam Altman [tweeted](https://twitter.com/sama/status/1341799820843831296?s=20) : "a large fraction of the most important US companies started in the next decade will continue to be within 50 miles of SF."

Before talking about the future, we should know the current situation. Can we say the SF is still an epicenter of innovation? Are there no other tech hubs in the US? 

As an indicator of the growth of new companies, I obtained a company list that went public between January 2109 to August 2, 2021. I analyzed the density of companies with QGIS, then visualized it with Mapbox. The link to my GitHub Pages is [here](https://hiromisa.github.io/IPO-density/).

---
## Data
I did data cleaning with Python/pandas with Jupyter notebook.

1. Finding IPO company list as a base dataset. The data range is January 2019 to August 2, 2021.

2. data cleaning
(a) Picking up Nasdaq or NYSE listed companies. (b) Removing non-US-based companies for this purpose. (c) Removing SPACs. I think these companies do not fit this purpose.

3. Geocoding based on company address

---
## Analysis
I did a geobased analysis with QGIS based on the data I gathered.

1. plotting the Data on the map.

2. Calculating the density of companies with Hexbins analysis on QGIS. I set the short diagonal length of a hexagon at 100km.

3. the SF area has more than 100 companies that went public past two and a half years, followed by the Boston area. There are some other small IPO hubs around the US. 

---
## Visualization
I used Mapbox for visualization and GitHub Pages to publish on the web. 





