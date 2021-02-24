The goal of this project is to detect changes in land cover in Arctic cities and settlements, 
using publicly available satellite data.

*** Why the Arctic?


Thinning sea ice in the Arctic has the potential to transform global shipping.  Sending cargo 
along the Northern Sea Route, through the Barents Sea and over Sibera, already can reduce
transit time from the Mediterranean to East Asia by 2 to 3 weeks.  A Transpolar Sea Route, which 
some climate researchers estimate will be open during the summer by 2035, would save another 
few days.

China has made its ambitions for the region known publicly (2018 Arctic Policy), and  
is actively producing icebreaker ships to lead cargo vessels through the Bering Strait.  Norway's 
northern cities are growing steadily.  Russia is balancing population decline on its Siberian 
coast with an increased effort to harvest Arctic fossil fuels, and will take over as chair of 
the Arctic Council in May of this year. 12 other nations sit on the Council, with Estonia and Ireland 
potentially joining in the coming years.  

The stakes in the region are rising and it does not seem the world is paying much attention.

*** Why satellite data?

We seek to discover which nations are preparing for the opportunity of
a rapid escalation in economic activity in the Arctic in the coming few decades.

There are satellites in orbit that collect electromagnetic data for the entire surface of the earth
every 2 weeks.  NASA's Landsat satellites, along with Sentinel 1 and 2 from the European 
Space Agency, are the main ones that make their data publicly available.

The satellite collects not only visible light, but near-infrared and other "bands" located
slightly further out on the electromagnetic spectrum.  This is an incredible resource for data
scientists seeking to draw inference on what is happening on the earth's surface.  These additional
bands provide additional features for running machine learning algorithms.  For example, water and 
heavy vegatation may be hard for a computer to discern on the spectrum of visible light,
but their reflectance measurements are quite different on bands with slightly longer wavelengths.  The
Landsat satellite data has 12 variables, as opposed to only 3 for a red, blue, green pixel image format.

*** Machine Learning Project Plan:

1. Obtain satellite data for various Arctic locations in 2000, 2010, and 2020
(note that Google Earth Engine has functionality to create nice composite data sets 
with the best satellite capture data throughout the time window)

2. Run a supervised machine learning algorithm to detect land cover in each location
Step A: Train the data by selectioning specific points and areas within the region
of known land cover (water, buildings, trees, rocks).
Step B: Run the algorithm to classify each pixel into the same categories.
Step C: Assess accuracy metrics of the model.

3. Compare vegetation loss and building increases across the three time spans to discover economic activity.
