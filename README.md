# COVID-19 Statistics, Forecasts and Demographics

This project began as my final project in the UC Berkeley Data Bootcamp, that ran from January through June of 2020.  I have continued to update, expand, and refine this analysis since the course ended last summer.

I sourced data from a number of sources, including Tableau's Coronavirus (COVID-19) Datahub (https://data.world/covid-19-data-resource-hub), the New York Times COVID-19 Github repository (https://github.com/nytimes/covid-19-data), the LA Times COVID-19 Github repository (https://github.com/datadesk/california-coronavirus-data), the CDC COVID Data Tracker (https://covid.cdc.gov/covid-data-tracker/#datatracker-home), the Our World in Data Coronavirus Data Tracker (https://ourworldindata.org/coronavirus), the U.S. COVID Community Vulnerability Index (CCVI) (https://precisionforcovid.org/ccvi), UCLA Law's COVID Behind Bars Data Project (https://uclacovidbehindbars.org/), and the COVID Tracking Project (https://covidtracking.com/).  Three different mobility indices have been followed, including Google (https://www.google.com/covid19/mobility/), Apple (https://covid19.apple.com/mobility), and Descartes Labs (https://www.descarteslabs.com/mobility/) help understand changes in U.S. mobility from Coronavirus-related physical distancing.

I decided to look into COVID in Scotland, as that is my parents' homeland.  I sourced data from the Public Health Scotland website (https://www.opendata.nhs.scot/dataset/covid-19-in-scotland).  In order to plot the data geographically, I obtained the local authority boundary maps from The Information Lab (https://www.theinformationlab.co.uk/) and added them to Tableau.  I constructed a Tableau story and posted it to Tableau Public, which can be found here - https://public.tableau.com/profile/doug.smith8181#!/vizhome/COVIDinScotland/Story1.  These dashboards are also included in my main Tableau story - https://public.tableau.com/profile/doug.smith8181#!/vizhome/COVIDCrunching/COVIDCrunching.  Both of these stories are available for download in my Github repository - https://github.com/menlodoug/covid_crunching/tree/main/tableau



<img src=".\images\covid-19-datahub2.jpg" alt="covid-19-datahub2" /><img src=".\images\latimes2.png" alt="latimes" /><img src=".\images\nyt2.png" alt="nyt" /><img src=".\images\CDC2.jpg" alt="CDC" /><img src=".\images\our_world_in_data2.jpg" alt="our_world_in_data" /><img src=".\images\apple2.jpg" alt="apple2" /> )<img src=".\images\google-corona-960x540-2.png" alt="google-corona-960x540" /><img src=".\images\DL_Logo_Color_Black_With_Wordmark2.png" alt="DL_Logo_Color_Black_With_Wordmark" /><img src=".\images\precision-logo.4dd54723-2.png" alt="precision-logo.4dd54723" /><img src=".\images\ucla2.jpg" alt="ucla2" /><img src=".\images\PHS2.png" alt="phs2" /><img src=".\images\InfoLab2.png" alt="InfoLabe2" />



From Tableau's Coronavirus (COVID-19) Datahub, I downloaded the hyper extract file (https://data.world/covid-19-data-resource-hub/covid-19-case-counts/workspace/file?filename=COVID-19+Activity.hyper) and have put together a number of slides based on that data.  I update the slides regularly as Tableau updates this data daily.   Here are screenshots of several.

 <img src=".\images\tableau1-2.jpg"  alt="tableau1-2" /><img src=".\images\tableau2-2.jpg"  alt="tableau2-2" /><img src=".\images\tableau4-2.jpg"  alt="tableau4-2" /><img src=".\images\tableau3-2.jpg"  alt="tableau3-2" />

These dashboards all make an extensive use of filters, providing the viewer with a high degree of interactivity.

The New York Times COVID-19 Github site provides daily COVID-19 data.  I combined this data with U.S. county population figures and have performed a number of  manipulations (well commented out) in this pandas notebook (https://github.com/menlodoug/covid_crunching/blob/main/pandas/COVID_USA.ipynb).  Case and death rates per county were calculated and, once again, using extensive filtering, I have provided some great interactive visualizations.

<img src=".\images\state-map2.jpg"  alt="state-map2" /><img src=".\images\state-ranking2.jpg"  alt="state-ranking2" /><img src=".\images\state-map-table2.jpg"  alt="state-map-table2" /><img src=".\images\case-ranking2.jpg"  alt="case-ranking2" />

I also took some of the ranking information and plotted it using Plotly, to show how Plotly and Tableau can work together.  Plotly has more robust capability with its hover marks.

<img src=".\images\plotly1-2.jpg"  alt="plotly1-2" /><img src=".\images\plotly2-2.jpg"  alt="plotly2-2" />



The L.A. Times Github repository provides daily insight into California-related COVID data, including information on infections and deaths by race and age, nursing home/senior care data and running 7-day average test positivity.  Here are a couple of pandas notebooks I've constructed to extract data - http://localhost:8888/notebooks/Documents/UC%20Berkeley/Final_Project/Data%20Processing/Race-Ethnicity.ipynb, https://github.com/menlodoug/covid_crunching/blob/main/pandas/Nursing.ipynb) and screen shots from the Tableau dashboards.

<img src=".\images\race-ethnicity.jpg"  alt="race-ethnicity" /><img src=".\images\nursing2.jpg"  alt="nursing2" />

The COVID Tracking Project keeps track of testing throughout the country, by state.  I adjusted their pandas notebook to give me a look at national and California-specific testing data on a daily basis (https://github.com/menlodoug/covid_crunching/blob/main/pandas/Covid_Tests.ipynb).

<img src=".\images\testing-data2.jpg"  alt="testing-data2" /><img src=".\images\testing-data-ca2.jpg"  alt="testing-data-ca2" />

Here are a couple of demographic resources I have tapped.  The Surgo Foundation has developed the CCVI or COVID-19 Community Vulnerability Index.  In the U.S., people living in vulnerable communities are significantly more likely to have died from COVID-19 as low vulnerability communities are burdened because people do not have equitable access to **health care, affordable housing, transportation, childcare**, **or safe and secure employment**.  The Index originally had six elements to it, but as the understanding of the virus has increased, they tweaked their model in December adding an additional element.  I have constructed a detailed, interactive dashboard incorporating their data at the state and county level.

The APM Research Lab has compiled data on the state death rates of  various racial groups.  Here is an interactive chart I have put together showing that data by state.

<img src=".\images\CCVI2.jpg"  alt="CCVI2" /><img src=".\images\color2.jpg"  alt="color2" />

The CDC provides extensive data on COVID, including 7-day rolling averages on cases and deaths and positivity rates for 7-day, 30-day, and the entire duration of the pandemic.  I have utilized the parameter feature in Tableau to offer different views.  They also recently started providing vaccination data, offering an opportunity for another dashboard.

<img src=".\images\7day-case2.jpg"  alt="7day-case2" /><img src=".\images\7day-death2.jpg"  alt="7day-death2" /><img src=".\images\positivity2.jpg"  alt="positivity2" /><img src=".\images\vaccines2.jpg"  alt="vaccines2" />

The CDC also gathers forecast data for both cases and deaths from a number of different research organization.  Using filtering, I have put together interactive dashboards for each category, offering looks at projections from the different outfits by state.  Here are screenshots.

<img src=".\images\death-forecast2.jpg"  alt="death-forecast2" /><img src=".\images\case-forecast2.jpg"  alt="case-forecast2" />

A population that has been severely impacted by the pandemic are those imprisoned.  UCLA Law has conducted a study tracking infections and deaths in the country.  Here's a screenshot of an interactive dashboard that shows the data by facility, by state, and by magnitude of impact

Public mobility has been significantly affected by the pandemic as social distancing has kept people from their normal routines and at home.  Three companies tracking mobility are Google, Apple, and Descartes Labs.  Here are screenshots from the dashboards I constructed for each.

<img src=".\images\prison2.jpg"  alt="prison2" /><img src=".\images\google2.jpg"  alt="google2" /><img src=".\images\apple-mobility2.jpg"  alt="apple-mobility" /><img src=".\images\descartes2.jpg"  alt="descartes2" />

I conclude the Tableau story by including a cute, short animation from Stanford Medicine.

<img src=".\images\prevent2.jpg"  alt="prevent2" />