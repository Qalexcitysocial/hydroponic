# Hydroponic

In this implementation Ebb and Flow system is used. This system works by temporarily flooding the grow tray with nutrient solution and then draining the solution back into the reservoir. When the scheduler turns the pump on nutrient solution is pumped into the grow tray. When the timer shuts the pump off the nutrient solution flows back into the reservoir. The water pump is set to come on several times a day, depending on the size and type of plants, temperature and humidity and the type of growing medium used.

![alt tag](http://gardenious.com/wp-content/uploads/2014/08/how-to-build-an-ebb-and-flow-hydroponic-system.png)

# How it works

Rasbperry Pi works as a server that collects sensor data from Arduino over USB serial communication and keeps it in SQLite database. It is equipped with Pi camera, used for visual inspection of plants progress, also it has the functionality of capturing timelapse photos.

Web app is used for displaying the sensor data in form of the charts and working time for devices (light and water pump), providing user with configuration page where he can set on/off intervals of the devices and desired values of the sensors, also it displays notifications. From here user can take pictures manually or open the timelapse view for specified date range.

Telegram bot can retrieve the data about sensor values in the last 24h, send notifications about values out of range for sensors (specified in the config part of web app) and capture pictures.

# Setting up

git clone https://github.com/djolez/hydroponic.git

Web app: Run bower install in web-app folder

For the Client, the Bot, Part: Simply Search Hydrobot on telegram


# Pictures of the system development

Project pictures: http://imgur.com/a/kVj2a
