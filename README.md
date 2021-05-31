# Determine a Good Observatory Location

>_Abstract : A good observatory to observe the night sky depends on many factors. Under ideal conditions, the best place to see sky objects lies in "a good seeing", that is, a steady, transparent atmosphere (In general, seeing could be known via telescope guiding systems by computing the full width at half maximum (FWHM) and half flux diameter (HFD) of a selected star)[1]. However, in most places crowded and developed, which can cause a strong atmospheric disturbance, to have a nice seeing is almost as far as possible. Apart from anthropogenic factors, we can still rely on "weather conditions" to define the sky quality. The project will show a basic weather analyze of night sky observation in Taiwan from Jan 2016 to Dec 2020, by analyzing some common features. Since the accuracy of the analyze depend on a certain place, which could be a city or a district, this project would not give a precise result, it would only demonstrate the considerations when deciding the location of the observatory._

## Table of Contents
 <ul>
<li><a href="#intro">Introduction</a></li>
<li><a href="#steps">Steps</a></li>
<li><a href="#insta">Install</a></li>
<li><a href="#GE">Geographical Environment</a></li>
<li><a href="#PD">Parameters Definition</a></li>
<li><a href="#UR">Useful Resources</a></li>
 </ul>

<a id='intro'></a>
## Introduction

Things to consider when deciding where an astronamy observatory should be located : clear, dry, and dark. In addition to latitude and season, a clear night sky should be able to see the maximum stellar objects. Lunar and human activities may cause heavy light pollution, but an observatory for the general public to know the beauty of the night sky is not that impracticable. Since buildings cannot be destroyed, which is one of the atmospheric disturbance contributing factor, the last thing to consider is humidity, a place where is often rainy and cloudy could impact both the seeing and the apparatus. The dataset of this project will start from collecting historical weather data from [World Weather Online](https://www.worldweatheronline.com/developer/). Notice that the dataset only contains a five-year data, since we all know the climate in an area "should" be about the same in all time (we will not consider the El Niño and La Niña cases which are unpredictable and shouldn't be a reason not to build observatories).  
According to Isaac Newton Group of Telescopes, one of the observing conditions at the observatory is : 75% of nights are clear.
Other conditions like extinction and brightness[2] depends alot on the sky background of a certain area, which are not what we will put in consideration now. Also, we will not introduce any type of telescope, that should base on the individual decisions, its not in our discussion.  

###### [1] Full Width at Half Maximum (FWHM) : The width of a spectrum curve measured between those points on the y-axis which are half the maximum amplitude, quality of an astronomical image based on how much the telescope and atmosphere have smeared a point source in an image over several pixels in the CCD, measured in arcseconds(″).
###### Half Flux Diameter (HFD) : The star size in an astronomical image, measured in pixels. Both FWHM and HFD should be as small as possible for a good seeing, it can also tell if the telescope is out of focus.

###### [2] Atmospheric extinction : The reduction in brightness of stellar objects as their photons pass through our atmosphere.

<a id='steps'></a>
## Steps
Investigation of the site should start with the geographical environment, giving the first information of where the observatory stand. In the overall dataset, cloud coverage(<25%), relative humidity(<90%), wind speed(<15m/s) and visibility per year are the critical parameters of defining a clear sky. Since the dataset won't exactly tell us the weather of that day, we will first plot them as univariate exploration respectively. Next, we should observe whether this place have a stable climate by looking at its average temperature in all years. And finally, we will take a look at the photometric and spectroscopic nights[3]  
###### [3] Photometric and spectroscopic night : A photometric night is a night where the sky is clear and transparent at least six hours or the whole summer night. A spectroscopic night can be a bit lighter and partial cloudy (extinction < 0.5 magnitudes and obscuration < 50% above 30 degree elevation).

<a id='insta'></a>
## Install

Install the package (see : [WorldWeatherOnline historical weather data API wrapper](https://github.com/ekapope/WorldWeatherOnline#install-the-package))
```
pip install wwo-hist
```

<a id='GE'></a>
## Geographical Environment
Location : Taiwan  
Coordinate : 25°04′N 121°31′E  
Area : 36,197 km^2  
Climate : Marine tropical. The northern and central regions are subtropical, whereas the south is tropical and the mountainous regions are temperate. The rainy season is concurrent with the onset of the summer East Asian Monsoon in May and June. The entire island experiences hot, humid weather from June through September. Typhoons are most common in July, August and September. During the winter (November to March), the northeast experiences steady rain, while the central and southern parts of the island are mostly sunny.  
Geology : Convergent boundary between the Yangtze Subplate of the Eurasian Plate to the west and north, the Okinawa Plate on the north-east, the Philippine Plate on the east and south, and the Sunda Plate to the southwest. (Wikipedia)  

<a id='PD'></a>
## Parameters Definition
* moon illumination : Moon phase, percentage of the illuminated disc. (New Moon : 0%; First and Third Quarters : 50%; Full Moon : 100%.) Although there might be some moonlight in some cases, the observation can still go on by looking at the other directions. In this project, we will filter out the data of illumination 50% ~ 100% at night time (gibbous phase).
* precipMM (mm) : Precipitation, a product of the condensation of atmospheric water vapour that falls under gravity.
* cloudcover : Percentage of the cloud coverage, but it `can't represent the layer of the cloud`.
* visibility (miles) : Measure of distance at which an object or light can be clearly discerned, varies from the direction and angle of view, and the height of the observer, affected by the presence of fog, cloud, haze and precipitation. (Scales from 0 (poor) to 10 (excellent).)

<a id='UR'></a>
## Useful Resources
[1][Observing conditions: definitions](https://www.eso.org/sci/observing/phase2/ObsConditions.html)  
[2][Observing conditions](http://www.ing.iac.es/astronomy/observing/manuals/html_manuals/general/obs_guide/node9.html)  
[3][Site Quality](http://www.ing.iac.es/astronomy/observing/conditions/#ext)
