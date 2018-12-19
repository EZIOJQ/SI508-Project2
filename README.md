# Data visualization - NationalSites
(To run this project, you must have a google APIkey, to get a google APIkey, you can check this website for instructions: https://developers.google.com/places/web-service/get-api-key)

## How to run this project?
* Run "proj2_nps.py", you will see in your terminal as follow:
```
--list <stateabbr>
--exit
--help
Please choose a function:
```
* Input LIST and an abbreviation of one state to see all the national sites in this state.
```
list mi
1) Isle Royale
2) Keweenaw
3) Motor Cities
4) North Country
5) Pictured Rocks
6) River Raisin
7) Sleeping Bear Dunes
Please choose a site to get nearby places or map
```
* Input the index of one national site to see the nearby places
```
nearby 1
1) South Lake Desor Campground
2) Malone Bay Campground
3) Hatchet Lake Campground
4) Todd Harbor Campground
5) Crystal Cove
6) Ishpeming Point
7) Isle Royale Wilderness
8) Little Todd Campground
9) North Lake Desor Campground
10) Hay Bay Campground
11) Hay Bay Boat Launch
12) Malone Bay Ranger Station
13) Malone Bay Boat Launch
enter map to show the plot
```
* Or input MAP to see the plot of these national sites
![Michigan](https://github.com/EZIOJQ/SI508-Project2/raw/master/Sample_Michigan_Nationalsite.png)

### caching files are "sample_cache_national_site.json" and "google_cache.json"
### caching files are named but you can change them by themselves.
### you may need to install BeautifulSoup4 and Plotly packages. You can use "pip3 install bs4" or "pip3 install plotly" to achieve that.
### make sure you have the google api key and add it into "secrets.py".

#### Each files have different functions:
1. alternate_advanced_caching.py is a .py script that contains all caching funcitons and the time of each cache. 
2. secrets.py is a file that needs you to input your google api key. To get a google api key, you can check this website   

#### An example to run:
1. run the proj2_nps.py, then choose which state you want to see. You should input like "list mi" or "list ca" for example.
2. It will give you a list of all national sites in this state, and you can simply use "map" command to get the plot of these sites on the map. A new popup website will show up.
3. If you want to get more information about the nearby places of this national site, you can input "nearby < index >". (The index number of which site you want to know more). 
4. it will give you a map contains all nearby places of this site.
5. Anytime you want to quit, input "exit". And anytime you need help, just input "help".















references:
1. https://www.nps.gov/state/al/index.htm
2. https://developers.google.com/places/web-service/search
3. https://plot.ly/python/scatter-plots-on-maps/
