# Instructions on ThirdReality Vibration Sensor Private Cluster in Home Assistant ZHA

## ZHA Configuration

1）Create a Folder for Local Code Files: a. Navigate to the /config directory. b. Create a new folder with a name(e.g., thirdreality_quirks). This folder will store the local code files.

2）Place the vibrate.py File: a. Use the Samba share tool to transfer the vibrate.py file into the newly created folder.

3）Edit the configuration.yaml File(as shown in the boxed area):

<img title="" src="assets/vibrate/1.png" alt="">

4）Restart Home Assistant: a. Restart Home Assistant to apply the configuration changes.

Operating Devices

Note: These instructions describe the operation for a Vibration Sensor. Similar methods can be applied to customize other ThirdReaity devices with private clusters.

1.Add a Vibration Sensor

2.Access Vibration Sensor Settings, navigate to the details page of the added Vibration Sensor click the "Options" button, as shown in the screenshot

<img title="" src="assets/vibrate/2.png" alt="">

3.In the pop-up menu, choose the "Manage Zigbee Device" option.

<img title="" src="assets/vibrate/3.png" alt="">
<img title="" src="assets/vibrate/4.png" alt="">

4.In the new window, select "ThirdRealityAccelCluster" from the "Clusters" drop-down list.

<img title="" src="assets/vibrate/5.png" alt="">

5.Under "ATTRIBUTES," locate "cooldown_perioc.", set the "value" to 10, click the "WRITE ATTRIBUTE" button.

<img title="" src="assets/vibrate/6.png" alt="">

6.Compare the "Logbook" display before and after sending the command. The following two screenshots show the difference.

<img title="" src="assets/vibrate/7.png" alt="">

<img title="" src="assets/vibrate/8.png" alt="">

3.Access Smart Plug scripts on GitHub
URL：https://github.com/thirdreality

<img title="" src="assets/vibrate/9.png" alt="">

<img title="" src="assets/vibrate/10.png" alt="">

<img title="" src="assets/vibrate/11.png" alt="">

<img title="" src="assets/vibrate/12.png" alt="">
