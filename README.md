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

Things to consider when deciding where an astronamy observatory should be located : clear, dry, and dark. In addition to latitude and season, a clear night sky should be able to see the maximum stellar objects. Lunar and human activities may cause heavy light pollution, but an observatory for the general public to know the beauty of the night skay is not that impracticable. Since buildings cannot be destroyed, which is one of the atmospheric disturbance contributing factor, the last thing to consider is humidity, a place where is often rainy and cloudy could impact both the seeing and the apparatus. The dataset of this project will start from collecting historical weather data from [World Weather Online](https://www.worldweatheronline.com/developer/). Notice that the dataset only contains a five-year data, since we all know the climate in an area "should" be about the same in all time (we will not consider the El Niño and La Niña cases which are unpredictable and shouldn't be a reason not to build observatories).  
According to Isaac Newton Group of Telescopes, one of the observing conditions at the observatory is : 75% of nights are clear.
Other conditions like extinction and brightness[2] depends alot on the sky background of a certain area, which are not what we will put in consideration now. Also, we will not introduce any type of telescope that should base on the individual decisions, its not in our discussion.  

###### [1] Full Width at Half Maximum (FWHM) : The width of a spectrum curve measured between those points on the y-axis which are half the maximum amplitude, quality of an astronomical image based on how much the telescope and atmosphere have smeared a point source in an image over several pixels in the CCD, measured in arcseconds(″).
###### Half Flux Diameter (HFD) : The star size in an astronomical image, measured in pixels. Both FWHM and HFD should be as small as possible for a good seeing, it can also tell if the telescope is out of focus.

###### [2] Atmospheric extinction : The reduction in brightness of stellar objects as their photons pass through our atmosphere.

<a id='steps'></a>
## Steps
Investigation of the final location should start with the geographical environment, giving the first information of where the observatory stand. In the overall dataset, cloud coverage(<25%), relative humidity(<90%), wind speed(<15m/s) and visibility per year are the critical parameters of defining a clear sky. Since the dataset won't exactly tell us the weather of that day, we will first plot them as univariate exploration respectively. Next, we should observe whether this place have a stable climate by looking at its average temperature in all years. And finally, we will take a look at the photometric and spectroscopic nights[3]  
###### [3]

<a id='insta'></a>
## Install

<a id='GE'></a>
## Geographical Environment

<a id='PD'></a>
## Parameters Definition

<a id='UR'></a>
## Useful Resources
[1][Observing conditions: definitions](https://www.eso.org/sci/observing/phase2/ObsConditions.html)  
[2][Site Quality](http://www.ing.iac.es/astronomy/observing/conditions/#ext)
