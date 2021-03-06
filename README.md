# ESP32_Skripsi
Arduino code for ESP32 configuration as Wi-Fi Access Point (AP) and Station (STA). Also, STA is configured as web server that can handle Ajax request to refresh the measured RSSI data in the webpage. 

These programs are adapted and modified from [circuit4you](https://circuits4you.com/) and [randormnerdtutorials](https://randomnerdtutorials.com/esp32-access-point-ap-web-server/) projects. The modification in Arduino code is mostly done by me whereas the html header code is modified entirely by my friend and was uploaded first on his [gist repo](https://gist.github.com/mwafa/c3a70e72e3064bcd1f3a6744e1128229#file-realtime-grafik-ajax-polling-html). See code for full description. 

This code is created for my final undergraduate thesis with the topic of indoor localization using Wi-Fi RSSI data. The `ESP32_AP` repo contain an Arduino code for configuring ESP32 as an AP with the custom SSID and password. The `ESP32_RSSI_Graph_webServer` repo contain the code for configuring ESP32 as STA and webserver. 

The webpage for displaying measurement values can be accessed by first configuring ESP32 as STA, then copying the printed IP Adress on the Arduino serial monitor. While doing this, be sure to connect the STA with a working Wi-Fi hotspot for internet connection. For further data processing, measurement values can be downloaded as a csv file. Also, the displayed value will be updated based on the latest measurement data using Ajax.

Example of visualized real-time data on the local web and downloaded csv file is shown below. Missing data was due to a temporary connection lost. 

![alt Visualized data](https://github.com/effendev/ESP32_Skripsi/blob/master/data1.jpeg "Visualized data in graph and table")
<p align="center">
	<b>Visualized data in graph and table</b><br>
	<br>
</p>

![alt CSV data](https://github.com/effendev/ESP32_Skripsi/blob/master/data2.jpeg "Downloaded CSV data")

<p align="center">
	<b>Downloaded CSV Data</b><br>
</p>

