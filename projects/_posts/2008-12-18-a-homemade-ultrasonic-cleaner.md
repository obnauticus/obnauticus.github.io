---
layout: post
title:  "A homemade Ultrasonic cleaner"
projectname: "openClean"
date:   2008-12-18
comments: true
tags: projects
type: project
summary: Ultrasonics are the most popular method for cleaning metal with precision and care. Making a scientific-grade cleaner at home is a breeze.
---

From cleaning car parts to cleaning cleaning jewelry, ultrasonic cleaners are used in a wide variety of applications. Wither it's a sensitive diamond ring that needs a little polish, or an old spark plug covered in grease -- Ultrasonics are the most popular method of choice for cleaning parts in little time with precision.<br />
<br />
<span style="font-size: 180%; font-weight: bold;">How Ultrasonic Cleaning works:</span><br />
<br />
Ultrasonic cleaning works by tearing voids between particles in the cleaning solution, this is called cavitation. These little pockets of air explode when they come in contact with a solid surface. Some people report these explosions occurring at pressures up to 15,000PSI and temperatures up to 5,000K. Although these conditions are extreme, the pockets of air are so small that they only have enough power to tear off any surface dirt on the dirty object. You can even stick your hand in the ultrasonic cleaner while it is running.<br />
<br />
However, like all other things; machines with this amount of precision cost a large sum of money. This De-I-Why article is written to help you design your own Ultrasonic cleaner at a fraction of the price.<br />
<br />
This project is similar to all audio setups. Previous knowledge of audio hardware and setup is a real plus, and will help you lots with the design of this project.<span style="font-size: 180%;"><br /></span><span style="font-size: 180%; font-weight: bold;">Materials:</span><br />
<br />
* = Hard to find around the house.<br />
<ol>
<li>Oscilloscope (Nice if you have one, but not necessary).</li>
<li>* Two Ultrasonic Transducers</li>
<li>* A capable sound card (with a frequency response ≥the optimal resonating frequency for the transducers), or function generator (same restrictions apply).</li>
<li>* Linear Amplifier (with an RMS &gt; the n*the required power necessary to drive the transducers (e.g. 2 Transducers need to be driven at 55W (2x55Watts) -- therefore I need an amplifier with an RMS ≥110Watts) ). The amplifier's frequency response must be greater than or equal to the frequency necessary to drive your transducers.</li>
<li>A soldering iron</li>
<li>Solder</li>
<li>Old RCA Audio cables.</li>
<li>A stainless steel container capable of holding a cleaning solution (Jelly roll, or cookie tray will do as long as it is built with only one layer of steel).</li>
</ol>
Note: Items 3 and 4 can be replaced by buying an "Ultrasonic Generator," however, they are generally very expensive, and do not have enough output power to drive more than one transducer.<br />
<br />
<span style="font-size: 180%; font-weight: bold;">Gathering the hard-to-find Materials:</span><br />
<br />
<img alt="" border="0" src="assets/images/2inchtrans2.jpg"/>1. Ultrasonic Transducers:<br />
<ul style="text-align: left;">
<li>Ultrasonic Transducers are very easy to find online, I got mine from eBay, a couple of 55Watt ones. Make sure the ones you get are designed for cleaner applications.</li>
</ul>
<br />
<br />
2. A capable soundcard:<br />
<ul>
<li>My sound is the X-Fi Fatal1ty, I generated a high-frequency (44kHz) waveform within Adobe Audition and verified it was 44kHz on my oscilloscope to make sure it was able to drive the transducers. Check your manufacture's specifications for your sound card's frequency response or maximum sampling rate to find out what the maximum output frequency of your soundcard is.</li>
</ul>
3. A linear amplifier:<br />
<ul>
<li>Make sure the RMS of the power is equal to or greater than the total amount of power needed to drive your transducers (the sum of the power necessary to drive all of your transducers must be equal to or greater than the RMS of the power your amplifier provides).</li>
<li>You must also make sure the frequency response of the amplifier is greater than or equal to the frequency which you plan to run your transducers at (usually around 40-46kHz).</li>
</ul>
<div align="center">
<img alt="" border="0" src="{{ site.url }}/assets/images/PT2000.jpg"><br />
</div>
<br />
<br />
<ul>
<li>I chose to use the Pyle Pro PT-2000 because it provides 175W of RMS power over two channels with a frequency response of 10Hz to 50kHz. This amplifier both meets and exceeds the specs required to drive the transducers I picked. It is also relativly cheap. </li>
</ul>
<ul>
<li>Note: Do not buy an "Ultrasonic Amplifier," these are just regular audio amplifiers. There is a particular seller on ebay which has photoshopped a Pyramid Pro 150W amplifier and charges about 40% more just reselling it on eBay under a different name.</li>
</ul>
4. A soldering Iron:<br />
<ul>
<li>If you don't already have one you need to get one. A tempreature controlled one is nice, but not necessary.</li>
<li>I used my Weller WESD51, this soldering iron is nice for everything and is a popular choice among many hobbyists as well as professionals.</li>
</ul>
5. A Stainless Steel Container:<br />
<ul>
<li>Keep in mind that it will be filled with a cleaning solution, and therefore must be able to hold a cleaning solution.</li>
<li>The container must be made of a something capable of resonating sound waves. It's also a good idea to look for corrosion resistant material. Stainless steel is the most popular choice in the world of ultrasonic cleaning.</li>
<li>Make sure there is only one layer of metal between the stainless steel and the cleaning solution.</li>
<li>I chose to use a Jelly Roll pan, there are obviously more choices out there. Be creative!</li>
</ul>
<span style="font-size: 180%; font-weight: bold;">Procedure:</span><br />
<ol>
<li>Epoxy your ultrasonic transducers to the bottom of your stainless steel container. Make sure they are in locations which allows cavitation to occur evenly throughout the cleaning tank. I suggest spacing them diagonally from each other in a rectangular cleaning tank, so there is even cavitation throughout the entire volume of the cleaning tank. Make sure when epoxying them to the bottom that you try to keep the bond space between the transducers and the steel tank as small as possible. You can use vice grips or weights placed on top of the transducers to achieve this.</li>
<br />
<li>Now, cut off one end of an old RCA cable of your choice.Next, solder both of the wires (doesn't matter which one), to ONE of the pads in the picture, pointed out by red arrows. Do not solder both wires to one pad, solder one wire per pad, and solder both of them to a pad.</li>
<br /><br />
<div align="center">
<img alt="" border="0" src="{{ site.url }}/assets/images/transducer.PNG">
</div>
<br />
<li>  Repeat step 2 for the other transducer.<br /></li>
<li> Next, plug the other end of the component cables into the output of your amplifier (left or right channels do not matter).<br /></li>
<li> Next, plug your sound card (or HF sin wave generator) into the input of your amplifier.<br /></li>
<li> Now, fill the stainless steel container with a cleaning solution of your choice (I used Isopropyl Alcohol "iso alcohol," most people do not suggest using flammable materials because there is a chance it will explode, I didn't really care though).<br /></li>
<li> Make sure everything is hooked up correctly.<br /></li>
<li> Turn your amplifier on, and generate your HF sin wave (you can find some sound card wave generators on google, I used Adobe Audition).<br /></li>
<li> If that did not explode, then you should be seeing cavitation in the cleaning solution.</li>
</ol>
<span style="font-size: 180%; font-weight: bold;">Conclusion:</span><br />
<br />
This should work for most cleaning applications, I have seen many people use Ultrasonic cleaning for cleaning grease off of old PCB's, a well as a variety of different parts. Just make sure to change your cleaning solution out once you feel it has been tainted with whatever dirt you may have put into the cleaner.