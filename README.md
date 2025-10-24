# Overview
This project is an interactive dashboard created using Vega-Lite and HTML, visualizing birth rates in Malaysia from 2000 to 2023 across different attributes such as state, gender, and ethnicity.

# Website Link:
https://ritz21-raina.github.io/DataVisualisation2/


# Munaver Visualisation Framework
### Domain:
This visualisation explores the birth trends in Malaysia from 2000 to 2023, analysing how birth counts vary across different dimensions of society such as state, gender, and ethnicity. The main goal is to understand Malaysia’s population dynamics over time — revealing regional patterns, gender balance, and ethnic diversity in birth rates. This domain is significant as it connects demographic data with socio-cultural and geographic contexts, helping viewers observe long-term changes that reflect broader social and economic developments.


### What:
The primary data on live birth counts was sourced from the Department of Statistics Malaysia (DOSM) Open Data Portal, ensuring official and credible information. The total population of Malaysia was obtained from Our World in Data, providing broader national context for comparison.
Latitude and longitude details were later added to the merged dataset to enable spatial visualisation. To map the geographic component, a GeoJSON file of Malaysia was downloaded from SimpleMaps, and then converted into TopoJSON format using Mapshaper for efficient rendering in Vega-Lite.

#### Data Sources:

Malaysia population: https://ourworldindata.org/explorers/population-and-demography?time=2000..2023&hideControls=false&indicator=Population&Sex=Both+sexes&Age=Total&Projection+scenario=None&country=~MYS

Birth Counts: https://open.dosm.gov.my/data-catalogue/births_annual_sex_ethnic_state?state=johor&sex=male&ethnicity=overall&visual=table

Map GeoJSON: https://simplemaps.com/gis/country/my


### How:
Several visual idioms were designed to present different aspects of the data clearly and interactively:

1. Three Choropleth Maps (2000, 2010, 2020):
Display birth counts by state across three time periods. Keeping them separate allows easier comparison and highlights how regional birth patterns shift over decades.

2. Line Chart (Births by Ethnicity):
Shows the trend of birth counts across all years and ethnic groups. This helps users identify how demographic diversity evolves and which ethnicities drive population changes.

3. Lollipop Chart (Births by State):
Plots absolute birth counts with a year slider, allowing comparison of quantitative values across states and over time in an intuitive, minimal way.

4. Gender Pyramid:
Breaks down births by state and gender, visualising Malaysia’s gender ratio. It highlights that the distribution remains generally balanced, with no strong bias toward either gender.

5. Heatmap (State vs Ethnicity):
Combines all three variables — state, ethnicity, and gender — into one compact view. The x-axis represents ethnicity, the y-axis represents states, and users can toggle a gender filter to explore detailed insights interactively.

All these charts and maps were made using vegalite. Made into a webpage using html, styling in css.
