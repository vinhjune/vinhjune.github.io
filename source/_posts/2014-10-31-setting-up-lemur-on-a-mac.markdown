---
layout: post
title: "Setting up Lemur on a Mac"
date: 2014-10-31 15:18:31 +0100
comments: true
categories: Music
tags: [Lemur, dj]
---
[!(http://img.youtube.com/vi/r2aURZbVR38/0.jpg)](http://www.youtube.com/watch?v=r2aURZbVR38)

{% youtube https://www.youtube.com/watch?v=r2aURZbVR38 %}
Lemur is one of the most powerful and flexible MIDI controllers out there. When it comes to setting up Lemur though, things are a bit more involved than the usual USB MIDI controller. The following article will take you step-by-step on setting up Lemur and how to configure Traktor for use with a custom MIDI map. The video above shows all of the steps from start to finish. Though the focus is on Mac, many of the general principles will also apply to PC.
<!--more-->

# Getting the Software:

The Lemur app is available from the Apple App Store. Once purchased, head over to Liine.net and download the additional software that’s needed. The software includes two applications: the Lemur Editor which loads and edits templates, and the Lemur Daemon which works as a bridge between the audio software and the Lemur app.  You will need to register with Liine before downloading these. It’s also worth taking a look at the premium templates while at the site. There are hundreds of user templates created by the Lemur community and the premium ones are some of the best.

# Tech Overview:

It’s helpful to have a bit of an understanding of how the different parts of Lemur work together. A Lemur setup includes four main components.  The first is the Lemur iPad app.  The next two are the Lemur Editor and Lemur Daemon that you downloaded from the site. Last is the ad hoc network or hardwired MIDI connection.  An ad hoc network is a computer to computer wireless network that’s created on the host computer.  In a Lemur setup, this ad hoc network consists of two devices: the iPad with the Lemur app on it and the computer running the Lemur Editor and audio software to be controlled.

# Steps for setting up Lemur on a Mac:

1. First, make sure the Lemur Daemon is running. When on, the Daemon shows up as a small iconin the upper right of the desktop. You can set the Daemon to always launch at startup by clicking on the icon and clicking “Setup Daemon Preferences” from the dropdown menu.
2. Next it’s time to create the Ad Hoc network:
  * Click on the WiFi symbol  in the upper right of the desktop and select “create network” from the dropdown menu.
  * After giving the network a new name or leaving it at default, hit the create button.
  * Now on your iPad go into the “WiFi” area in the settings. You should see the name of theÂ network you just created. Click on it and verify that the iPad connects to it.

   Your iPad and host computer are now connected to eachother on their own ad hoc network.
3. Now you will connect the Lemur Editor on the host computer to the Lemur app on the iPad.
  * Run the Lemur App on your iPad.
  * Now start the Lemur Editor on the computer.
  * Once the Editor opens, press the small box with an arrow  in the upper right corner. Your iPad and its IP address should show up in the “connection” box that pops up. It may take a minute or two for your iPad to appear.
  * Double click on your iPad name in the “connection” box. The arrow button in the upper right of the Lemur Editor  should turn into a green square indicating a connection with the iPad.
4. Finally it’s time to load a Lemur template into the iPad app. To do this, first open a template in the editor by double clicking on the .jzml file. Then click the arrow button   in the Editor and then double click your iPad in the “connection” box.

Your Lemur template should now be loaded onto the iPad and ready to control.

## Extra Tips:

1. It’s possible to upload a template from your iPad to the Lemur Editor on the computer.  To upload a template, first click the arrow button  in the Editor.  Now, instead of double clicking on your iPad name in the “connection” box, highlight your iPad and press the download button at the bottom of the box.  Your template will now upload to the Editor.

2. The Lemur Editor can also mirror the slider movements and button presses you make on your iPad. This feature helps when modifying or creating templates from scratch. To turn on mirroring, click the small box with two arrows  in the upper right corner of the Editor. Once activated, the arrows in the box will turn green.

# Using Lemur with Audio Software:

Now that you can load templates between the Lemur Editor and Lemur iPad app, let’s take a look at how to setup an audio program like Traktor to use Lemurs MIDI ports.

## Traktor Preference Settings:

1. With Traktor running, open up the “Preferences” from the dropdown menu and click on “Controller Manager” located at the bottom of the lefthand side.

2. In the “Device Setup” area at the top, click on the “Load” button. Then from the dropdown menu select “Import TSI” and from the next menu click on “Import Other”.

3. Now locate the .TSI file you want to load into Traktor.

4. Finally, make sure that the “In Port” and “Out Port” in the “Device Setup” area are set to the correct Lemur MIDI ports. These port may be different depending on the Lemur template, but a good place to start is with “Daemon In 0″ and “Daemon Out 0″.

Your Lemur template should now be MIDI mapped to Traktor.

Traktor is just one of the many examples of music software that that Lemur can control. In fact, most other programs are even easier to set up as they won’t need any sort of .tsi file loaded in.  For these, setting up Lemur is pretty much the same as setting up a standard USB MIDI controller.