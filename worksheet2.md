# Displaying data from the Sense HAT in Minecraft

SpaceCRAFT displays data from the SenseHAT in Minecraft, converting the data into 3D structures and blocks.

![SpaceCRAFT Display](images/spacecraft3.png)

This can be run at any time and will use live data from the SenseHAT, allowing you to see the results instantly in Minecraft.

## Run the real-time SpaceCRAFT display program

Run Minecraft by clicking `Menu > Games > Minecraft Pi`.

Click `Start Game` and enter a world by either double-clicking a world you have already created or selecting `Create new`.

Leave Minecraft running, press `Escape` to go to the menu and release your mouse pointer.

Open a terminal by clicking the icon on the taskbar, or by clicking `Menu > Accessories > Terminal`, and enter the following commands one by one, pressing `Enter` after each command:

```
cd ~/SpaceCRAFT/spacecraft
python3 mcastrorealtime.py
```

The SpaceCRAFT display will be created in front of the player's position. If you go back to Minecraft and look up, you will see the ISS.

## Explore the SpaceCRAFT data

### The four pillars

The four pillars running up the centre of the display show data from the temperature, humidity and pressure sensors on the Sense HAT and its CPU temperature.

![SpaceCRAFT Display Pillars](images/spacecraft5.png)

Along the centre of each pillar is a different type of block representing the different sensors:

* Lava - temperature
* Water - humidity
* Obsidian - pressure
* Red wool - CPU temperature 

Try holding your finger over the temperature sensor or breathing on the humidity sensor, and seeing what effect it has on the level of lava or water in the pillars.

### The ISS

The ISS at the top of the stairs which circle the pillars changes position based on the orientation of the Sense HAT. This is calculated using the Sense HAT's accelerometer, gyroscope, and magnetometer.

![SpaceCRAFT Display ISS](images/spacecraft7.png)

![SpaceCRAFT Display ISS](images/spacecraft2.png)

![SpaceCRAFT Display ISS](images/spacecraft8.png)

Tilt the Sense HAT and see the effect it has on the ISS.

### The date and time

The date and time is displayed by a large clock on the left of the display. When run live, it will show the current time set on the computer; when playing back data capture from the ISS, it will show the date and time the information was captured.

![SpaceCRAFT Display Date and Time](images/spacecraft10.png)

The date and time is displayed in the format DD.MM.YY HH:MM:SS (day . month . year  hours : minutes : seconds).

### Rocket

The rocket will be launched when the joystick is used.

![SpaceCRAFT Display Date and Time](images/spacecraft4.png)

![SpaceCRAFT Display Date and Time](images/spacecraft11.png)

## What next?

Now move on to [worksheet 3](worksheet3.md) to learn how to capture data from the Sense HAT.
