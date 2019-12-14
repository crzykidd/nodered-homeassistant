HomeAssistantFlows
==================

Flows for my home assistant environment

### About

I am in the process of moving from Smarthings over to Home Assistant, during the process I have decided to jump into Node-Red head first.   My intent to share my project with you is to maybe give someone starting out some insight and ideas.   

This is a good guide on how to import flows:  http://www.steves-internet-guide.com/copy-nodes-flows-node-red/

You should be able to import the RAW txt from flows.json into Node-Red and see the logic and the flows.     I will also try to keep some of the pictures of the flows up to date, but that will happen from time to time.

## ZWave Scene Management
The first flow is designed around using the zwave scene from HA and exeucting a set of commands based on that value.  This is utilizing the multi button tap functions from the Homeseer WD200+ Z-Wave switches.   In order to use these functions you will need to follow the directions here as well:  https://www.home-assistant.io/docs/z-wave/device-specific/#homeseer-switches

SceneManagement01.PNG is the main flow for this and it has links to the different lights involved in the scene:
![Image description](https://github.com/crzykidd/nodered-homeassistant/raw/nodered-homeassistant/SceneManagement01.PNG)

SceneManagement02.PNG is where the links land to turn on or off different lights
![Image description](https://github.com/crzykidd/nodered-homeassistant/raw/nodered-homeassistant/SceneManagement02.PNG)

## Washer and Dryer Announcement 
For Washer and Dryer complete announcements I am using Google Home devices with TTS.   
I have also found this power monitor node that makes it really simple.   You will need to play with your power to determine when each appliance is complete, but it doesn't take long to get it perfect.   
https://flows.nodered.org/node/node-red-contrib-power-monitor
Here is a picture of the flow. The flow itself can be found in the main flows.json.
![Image description](https://github.com/crzykidd/nodered-homeassistant/raw/nodered-homeassistant/WasherDryerAnnounce.PNG)

## Added a schedule builder for house modes  
Here is the flow for this:
https://github.com/crzykidd/nodered-homeassistant/raw/nodered-homeassistant/HouseStateChangeSchedule.PNG

Hope you find this usefull.
 
