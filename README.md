# Determine a Good Observatory Location

>_Abstract : A good observatory to observe the night sky depends on many factors. Under ideal conditions, the best place to see sky objects lies in "a good seeing", that is, a steady, transparent atmosphere (In general, seeing could be known via telescope guiding systems by computing the full width at half maximum (FWHM) and half flux diameter (HFD) of a selected star)[1]. However, in most places crowded and developed, which can cause a strong atmospheric disturbance, to have a nice seeing is almost as far as possible. Apart from anthropogenic factors, we can still rely on "weather conditions" to define the sky quality. The project will show a basic weather analyze of night sky observation at one of the observatories in Taiwan from Jan 2016 to Dec 2020, by analyzing some common features._

## Table of Contents
 <ul>
<li><a href="#intro">Introduction</a></li>
<li><a href="#steps">Steps</a></li>
<li><a href="#slide">SLide Deck</a></li>
<li><a href="#GE">Geographical Environment</a></li>
<li><a href="#PD">Parameters Definition</a></li>
<li><a href="#UR">Useful Resources</a></li>
 </ul>

<a id='intro'></a>
## Introduction

Things to consider when deciding where an astronamy observatory should be located : clear, dry, and dark. In addition to latitude and season, a clear night sky should be able to see the maximum stellar objects. Lunar and human activities may cause heavy light pollution, but an observatory for the general public to know the beauty of the night sky is not that impracticable. Since buildings cannot be destroyed, which is one of the atmospheric disturbance contributing factor, the last thing to consider is humidity, a place where is often rainy and cloudy could impact both the seeing and the apparatus. Notice that the dataset only contains a five-year data, since we all know the climate in an area "should" be about the same in all time (we will not consider the El Niño and La Niña cases which are unpredictable and shouldn't be a reason not to build observatories).  
According to Isaac Newton Group of Telescopes, one of the observing conditions at the observatory is : 75% of nights are clear.
Other conditions like extinction and brightness[2] depends alot on the sky background of a certain area, which are not what we will put in consideration now. Also, we will not introduce any type of telescope, that should base on the individual decisions, its not in our discussion.  

###### [1] Full Width at Half Maximum (FWHM) : The width of a spectrum curve measured between those points on the y-axis which are half the maximum amplitude, quality of an astronomical image based on how much the telescope and atmosphere have smeared a point source in an image over several pixels in the CCD, measured in arcseconds(″).
###### Half Flux Diameter (HFD) : The star size in an astronomical image, measured in pixels. Both FWHM and HFD should be as small as possible for a good seeing, it can also tell if the telescope is out of focus.

###### [2] Atmospheric extinction : The reduction in brightness of stellar objects as their photons pass through our atmosphere.

<a id='steps'></a>
## Steps
Investigation of the site should start with the geographical environment, giving the first information of where the observatory stand. In the overall dataset, cloud coverage(<25%), wind speed(<15m/s) and visibility are the critical parameters of defining a clear sky. The percentage of the relative humidity(<90%) could tell the environmental condition of setting up a telescope. Next, we should observe whether this place have a stable climate by looking at its temperature variation in different seasons. Finally, we will take a look at the photometric and spectroscopic nights[3]  The last of last, we will take a look at the world dark scale map via Wikipedia and the [Light Pollution Map](https://www.lightpollutionmap.info/) to see how bright or how dark Zhongli is.
###### [3] Photometric and spectroscopic night : A photometric night is a night where the sky is clear and transparent at least six hours or the whole summer night. A spectroscopic night can be a bit lighter and partial cloudy (extinction < 0.5 magnitudes and obscuration < 50% above 30 degree elevation).  

<a id='slide'></a>
## Slide Deck
To view the html slide for the `observe_slide_deck` file, input the following comment in your prompt.  
```
jupyter nbconvert FILE_NAME.ipynb --to slides --post serve --template output_toggle
```

<a id='GE'></a>
## Geographical Environment
Location : Taiwan, Zhongli district  
Coordinates : 24°57′25″N 121°13′25″E
Area : 76.52 km^2  
Climate (Taiwan) : Marine tropical. The northern and central regions are subtropical, whereas the south is tropical and the mountainous regions are temperate. The rainy season is concurrent with the onset of the summer East Asian Monsoon in May and June. The entire island experiences hot, humid weather from June through September. Typhoons are most common in July, August and September. During the winter (November to March), the northeast experiences steady rain, while the central and southern parts of the island are mostly sunny.  
Geology (Taiwan) : Convergent boundary between the Yangtze Subplate of the Eurasian Plate to the west and north, the Okinawa Plate on the north-east, the Philippine Plate on the east and south, and the Sunda Plate to the southwest.  
Topography : Plateau  

Located at the north west of Taiwan, Zhongli has an estimated population 397,083 in January 2017, and it's one of the most multicultural cities due to its convenience and proximity to Taipei (easy to commute). With the eight biggest but least populated villages on the western side of the district while the eastern side is occupied by industrial factories (belonging to electronic, metal, chemical, mechanical, food, textile and plastic manufacturers) and the heart of the metropolitan area. Surrounded by shoping districts and night markets (daily, usually from 6 p.m. to 1 a.m.).(Wikipedia)  

<a id='PD'></a>
## Parameters Definition
* Cloud Ccover : Percentage of the cloud coverage, it `can't represent the layer of the cloud`.
* Visibility (miles) : Measure of distance at which an object or light can be clearly discerned, varies from the direction and angle of view, and the height of the observatory, affected by the presence of fog, cloud, haze and precipitation (Scales from 0 (poor) to 11 (pure)).

<a id='UR'></a>
## Useful Resources
[1][Observing conditions: definitions](https://www.eso.org/sci/observing/phase2/ObsConditions.html)  
[2][Observing conditions](http://www.ing.iac.es/astronomy/observing/manuals/html_manuals/general/obs_guide/node9.html)  
[3][Basic numerical range and its conditions](https://www.weather.gov/bgm/forecast_terms)  
[4][Site Quality](http://www.ing.iac.es/astronomy/observing/conditions/#ext)  
[5][Analysis of the atmospheric visibility Restoration and fog attenuation](https://www.semanticscholar.org/paper/Analysis-of-the-atmospheric-visibility-Restoration-Deshpande/662237bb893d2b50a728751880f20cf1f8225aef)  
