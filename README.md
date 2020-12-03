# Interactive Maps with Folium!

This tutorial explored a very straightforward library (Folium) that can be used to create visually pleasing and interactive maps in Python.

The first part of this lab imported geojson files of LA county and LA county zipcodes, as well as a csv file of the location of every Starbucks in LA county. The first output map was a map choropleth map of the number of Starbucks locations in each zipcode. Since zipcode is an arbitrary spatial divide, the second map is a point map of all Starbucks locations that were plotted based on the lat/long of each store. 

The second part of the lab created a choropleth map of unemployment rates in US states. This map accessed data directly from a github repository using a url to the repository. It used a json file of US states and a csv file of state unemployment rates. I ran into a problem while trying to import the files for this part of the lab because the url I was using was not correct, and was directing to `raw.githubusercontent` which is in a format that can be accessed directly by python code.

### Takeaways from Lab 6 
- I am glad to know that you can import data that is in a github repository without having to download the data, and then import the data. This is helpful in cases where 1) the repository includes multiple datasets and you are interested in only one or a few and 2) when you are working colaboratively in a Colab document, and file names or pathnames are creating inconsistencies between users' code. 
- It is great to know that it is possible to create itneractive maps using python, in which you can zoom in and out, and add or remove data layers. 
- Exploring some of the suggested code for the folium library, it is clear that the folium library allows users to create many differnt kinds of maps beyong choropleth and point maps. Maps are created not all in one line of code, but by adding muliple layers or map features to an initial base map layer by using `.add_to(BaseMapName)`. To display the map you then just call the initial base map that all layers and features have been added to.  
