# *[UP42](https://up42.com/) Customer Support Challenge*

### Objective (why)
Our main role as customer support engineers is to make sure we understand the customer problem and we help in finding a solution to the problem.

This challenge aims to emphasize the following skills:
- [x] Problem solving and delivering an optimal solution in a limited timeframe.
- [x] Open communication with the customer.
- [x] Ability to persuade the customer.

### The challenge (what)
Our colleagues in Business Development have just closed a large deal with Bruno Brazil Associates, a well-established environmental consulting firm that consists of a multidisciplinary team (geotechnical engineers, geologists, biologists, agronomists, etc.).
Their current assignment is to evaluate the health of forests in [Bhutan](https://en.wikipedia.org/wiki/Forestry_in_Bhutan). Additionally, the local monarch has asked Bruno Brazil Associates to provide the results in [Cloud Optimized GeoTIFF](https://www.cogeo.org/) (COG) format, so that local communities can access the results without overloading the network infrastructure of the country. Usually, they would send a team to do the assessment on the ground. However, due to both the high costs of sending a team to such a remote country and also due to CoVID travel restrictions, the consulting firm needs to find a way to investigate the country!s overall forest health without ground measurements, so they decided to contact UP42 and adopt remote sensing as their method of investigating forest health.

### Main materials
To carry out this project we used:
- [x] [Up42 - SDK](https://sdk.up42.com/)
- [x] [Bhutan Forest GeoJson](https://mapcruzin.com/bhutan-shapefiles/bhutan_natural.zip)
- [x] [Python](https://www.python.org/)
- [x] [Jupyter Notebook](https://jupyter.org/)
- [x] [GitHub](https://github.com/)

### Here you can find
Catalog of the Spot, Pleiades and Sentinel-2 satellites to be able to observe the availability of images of our main products, for the most current dates.
- [Press Here](https://github.com/diegoalarc/Challenge_up42/blob/main/Catalog_Search_Bhutan.ipynb)

Example with [Modis](https://en.wikipedia.org/wiki/Moderate_Resolution_Imaging_Spectroradiometer) satellite to be able to observe an option that can give us a general view of the Bhutan forest.
- [Press Here](https://github.com/diegoalarc/Challenge_up42/blob/main/Up42_Challenge_Modis.ipynb)

Example with [Sentinel-2](https://en.wikipedia.org/wiki/Sentinel-2) satellite, which we used to analyze a sample of the Bhutan forest, and with which we will generate a simple Normalized difference vegetation index or [NDVI](https://en.wikipedia.org/wiki/Normalized_difference_vegetation_index) analysis.
- [Press Here](https://github.com/diegoalarc/Challenge_up42/blob/main/Up42_Challenge_Sentinel_2.ipynb)

### Possible customer solution

To solve the problem we are facing, one of the best possible and quick solutions through the use of satellite images is the use of NDVI. That is why as the first option, within our options is to obtain the values for the Bhutan forest with [Modis](https://en.wikipedia.org/wiki/Moderate_Resolution_Imaging_Spectroradiometer) images. In our case, since we are requested to be current information and when checking that there are no good current images of this satellite, we have resorted to the use of [Sentinel-2](https://en.wikipedia.org/wiki/Sentinel-2), which can provide us with quite detailed information and with a good temporal frequency.

To better understand what the NDVI values mean, we invite you to click on the following link:
- [Press here](https://eos.com/blog/ndvi-faq-all-you-need-to-know-about-ndvi/)

Here it is possible to observe the sample located at the coordinates Latitude: 27.25 & Longitude: 90.4 approximately.
![NDVI - Sample of the forests in Bhutan](https://github.com/diegoalarc/Challenge_up42/blob/main/ndvi-image.png)

A Histogram could be useful for quick analysis by giving a visual insight into the distribution of "healthy" vs "unhealthy" vegetation values in your study area.
Healthy, dense vegetation canopy should be above 0.5, and sparse vegetation will most likely fall within 0.2 to 0.5. However, it’s only a rule of thumb and you should always take into account the season, type of plant and regional peculiarities to know exactly what NDVI values mean.
In most cases, NDVI values between 0.2 and 0.4 correspond to areas with sparse vegetation; moderate vegetation tends to vary between 0.4 and 0.6; anything above 0.6 indicates the highest possible density of green leaves.
Traditionally, NDVI results are presented as a color map, where each color corresponds to a certain range of values. There’s no standard color palette, but most software uses the “red-green” one, meaning that red-orange-yellow tints indicate bare soil or dead/sparse vegetation, and all shades of green are a sign of normal to dense vegetation cover.

![Bhutan NDVI histogram](https://github.com/diegoalarc/Challenge_up42/blob/main/Bhutan_ndvi_histogram.png)

### Sample on the web
Here you can find a quick view version of the Bhutan forest sample area.

- [NDVI Bhutan forest sample](https://diegoalarc.github.io/Challenge_up42/)

### Why all the bands?
When we download the images from Up42-SDK, for this example, we also download the other bands at 10 meters that Sentinel-2 incorporates (a total of 12 bands). It is important not to eliminate them, since it is possible to generate different analyzes to more accurately determine the health of the forest by applying a spectral analysis when generating other indices. For this, we would like to invite you to investigate further or, in your case, analyze the data with your team of professionals familiar with remote sensing.

Check the following link to learn combinations of different indexes.
- [Press here](https://www.indexdatabase.de/)

note: NDVI is an index.

### Presentation
Here you can download a small presentation to show the capabilities and great advantages of using the Up42 API.
- [Presentation Here](https://github.com/diegoalarc/Challenge_up42/raw/main/Presentation_CS_Up42.pptx)

### SDK Up42
Here you can find the necessary documentation to be able to work with the Python SKD created by Up42.
- [SDK Here](https://sdk.up42.com/)

### More
If you wish, you can also visit the UP42-GitHub to find more examples.
- [UP42-GitHub ](https://github.com/up42)