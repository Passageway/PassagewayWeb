# 
![passageway logo](https://dl2.pushbulletusercontent.com/KbQ1LfBQ4PvfBj4LmbcYmXDPBHlTsnHR/Passageway.png)

### Project Description
Passageway is an attempt to provide a cost-effective, scalable, and automated method of aggregating foot traffic data within a facility. Such data aggregation offers meaningful statistics about the foot traffic of individuals within a defined space. With Passageway, users are able to see heat maps and view graphs that represent the foot traffic in a building, and analyze it on a website with various building floor-plans layered onto a Google Map. Users may also specify a certain time frame to see specific temporal data. All of the data is collected within the facilities through a system including CHIP computers connected to a pair of Infrared break beams. Ultimately, the data may be used to determine the frequency of activity for specific rooms, hallways, or entryways. Foot traffic data may be useful for understanding activity within a facility, seeing popularity of certain areas during specific times, or identifying times where room capacity is exceeded and thus presents a fire code violation.

### Repositories

 - [Android](https://github.com/Passageway/PassagewayAndroid)
 - [Field Unit](https://github.com/Passageway/PassagewayFieldUnit)
 - [Web](https://github.com/Passageway/PassagewayWeb) *you are here*

### Repo Overview
This is the webapp part of the Passageway project. This is where users can see data associated with each Passageway unit. This data is filterable by date and time as well.

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
