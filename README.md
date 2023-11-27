![](img/logo1.png)


# **TIMCON_ua**
LLC "Telemetric intelligent control modules"
_____
 *intelligent agents for telemetric monitoring and management*

![TREND](https://connectedworld.com/wp-content/uploads/2023/02/FOD-2.22.23.gif)
![AGRO](https://www.edimax.com/campaigns/mw/cufiles/images/ediexpo2022/reliable_dongle/smart_argriculture_660x440.gif)

# We write codes for smart devices

 ``` c++
void sensors_read() {
 
incubator_1.t1 = readSi7021Temperature(SI7021_ADDRESS);
incubator_1.h1 = readSi7021Humidity(SI7021_ADDRESS);
incubator_1.tegg1=getTemperatureBySensorName("tegg1");

incubator_1.tegg1=constrain(incubator_1.tegg1,35,39);

incubator_1.tw1=getTemperatureBySensorName("tw1");
//incubator_1.tw1=dsRead(0),2; 
incubator_1.tw1=constrain(incubator_1.tw1,5,70); 

incubator_1.t2=getTemperatureBySensorName("t2");
//incubator_1.t2=dsRead(1),2; 
incubator_1.t2=constrain(incubator_1.t2,5,70); 

int sensorValue = analogRead(SENSORGAZ_PIN);
float ppm = convertToPPM(sensorValue);
 incubator_1.CO2 = round(ppm);
  
}
 ```
- [X] create prototypes of control modules
- [x] design an electrical board
- [X] debug the module



![Monitoring agro](https://s3.amazonaws.com/s3-biz4intellia/images/applications-of-iot-in-agriculture.jpg)

# We get an intellectual assistant

-[PyLounge my TelegramBot(https://t.me/organic_farm_Timco_Bot)]
  
<!--
**TIMCON23/TIMCON23** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
