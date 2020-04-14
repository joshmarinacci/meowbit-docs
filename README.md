# meowbit-docs

Bonus docs for using MakeCode Arcade with the MeowBit

The [MeowBit](https://www.kittenbot.cc/products/meowbit-codable-console-for-microsoft-makecode-arcade) is a little 
gameboy like device that you can program using MakeCode Arcade, Python, or KittenBot's version of Scratch. It has
buttons, several sensors, can run on a battery, and you can make your own games for it through the web. This repo
will cover everything I've learned about using it with MakeCode Arcade. I don't plan to cover Python or Scratch. (yet)  

![image](./img/meowbit.jpg)

You can buy the MeowBit from KittenBot's website or one of several resellers. I got ours from Adafruit.

# Getting Started

First you should learn [MakeCode Arcade](https://arcade.makecode.com/), which does not require any hardware at 
all to use, and can work with several different devices. Once you've created a program you can 
click the download button in your projects to compile 
it into a .uf2 file.  This is the actual binary that goes on your device.  Plug your MeowBit into your computer using USB. It should
automatically mount as a flash drive. Drag the downloaded .uf2 file to the drive. The MeowBit will automatically disconnect
and load the game. It's that easy.

## Learning MakeCode Arcade

The MakeCode Arcade lessons are great for learning how to code and build games.  I went through the
[CS Intro 1 course](https://arcade.makecode.com/courses/csintro1) with my 8yr old kid and he loved it.
He's now making fun little games all by himself.   The courses cover using events, logic, loops,
animating sprites, creating a tilemap, and simple audio.

# Advanced Usage

I found very little specific to using MeowBit with MakeCode arcade, in particular the sensors. So that's 
what I'm covering here.


## Sensors

The MeowBit has built in sensors for light, temperature, and a gyroscope/accelerometer.  You can use them
with the Controller Extras extension. This extension will give you extra blocks in the 'Controller' category.

### Light

The built in light sensor is just below the switch in the top center of the MeowBit screen. The light value
is a number between 0 and 255. There are blocks to: 

* get the current light level with the `light level` block.
* detect light level changes with the `on light [dark]` block.

This example creates a lightbulb sprite. Every second it makes
the sprite *say* the current light level.  If the light becomes
*dark* then it says 'It got dark'. 

![light level](img/light_sensor.png) 

[live example](https://makecode.com/_3XbUYE2VdH8e)

 

* Document light sensor, gyro, temp



* Palette shift and color fade
* Doc controller combos 
* Test two player
* SD Card
* Seven segment
* Storyboard only JS

