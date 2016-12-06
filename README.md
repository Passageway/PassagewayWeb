#### 
<img src="https://dl2.pushbulletusercontent.com/KbQ1LfBQ4PvfBj4LmbcYmXDPBHlTsnHR/Passageway.png" width="500px">

### Project Description
Passageway is an attempt to provide a cost-effective, scalable, and automated method of aggregating foot traffic data within a facility. Such data aggregation offers meaningful statistics about the foot traffic of individuals within a defined space. With Passageway, users are able to see heat maps and view graphs that represent the foot traffic in a building, and analyze it on a website with various building floor-plans layered onto a Google Map. Users may also specify a certain time frame to see specific temporal data. All of the data is collected within the facilities through a system including CHIP computers connected to a pair of Infrared break beams. Ultimately, the data may be used to determine the frequency of activity for specific rooms, hallways, or entryways. Foot traffic data may be useful for understanding activity within a facility, seeing popularity of certain areas during specific times, or identifying times where room capacity is exceeded and thus presents a fire code violation.

### Architecture Overview
<center><img src="http://i.imgur.com/LuledZu.png" width="700px"></center>

### Repositories

 - [Android](https://github.com/Passageway/PassagewayAndroid) 
 - [Field Unit](https://github.com/Passageway/PassagewayFieldUnit) 
 - [Web](https://github.com/Passageway/PassagewayWeb) *You are here*

### Repo Overview
This is the webapp part of the Passageway project. This is where users can see data associated with each Passageway unit in heatmap form on a Google Map as well as in a chart of room count over time. The data is filterable by date and time as well. The webapp uses the Polymer project as a framework to provide a rich user experience.

### What it Looks Like
Here are some pictures to give a better understanding of what this webapp looks like when set up. 
<center><img src="http://i.imgur.com/6MKPeqZ.png" width="900px"></center>

Above is the view when a whole building is selected. In this view, a heatmap is displayed over top a blueprint of the building selected. Blueprints are not necessarily required in this project, but make it easier to see rooms on the map. If there were multiple units with data within the time period specified in the filters at the top, you would see heat points weighted according to activity. 
<center><img src="http://i.imgur.com/OqPrEmX.png" width="900px"></center>

In the image above, a single unit is selected. In this view, a line graph is displayed instead of a map. This graph shows the exits, entries and total count for the room at any given time. This is very useful to recognize trends and peak hours. You may notice that the count goes negative at some points. Given this project is still in its earlier stages, this is to be expected. To counteract any innaccuracies, the room count is reset back to 0 at 4am.
### Detailed Set-up Instructions
The wiki section will have more details on how to exactly set the system up in your own environment for testing. it is worth noting that this system is very much still in early stages and is not perfect by any means.

#### Getting started

1. Copy the project to your local machine:  
`git clone https://github.com/Passageway/PassagewayWeb.git passageway-web`
2. `cd passageway-web`
3. Allow access to the following scripts: `chmod u+x init/deploy init/ubuntu_prepare init/deploy`
4. Run `init/ubuntu_prepare`
5. Once completed, run `firebase login` and `firebase add --project <passageway-project-id>`
6. From there, run `firebase open` to run locally, or run `init/deploy` to deploy to the Firebase hosting instance


#### Futher Reference
* [Firebase hosting quickstart][firebase_qs]
* [Polymer CLI][polymer_cli]


[firebase_qs]: https://firebase.google.com/docs/hosting/quickstart
[polymer_cli]: https://www.polymer-project.org/1.0/docs/tools/polymer-cli
