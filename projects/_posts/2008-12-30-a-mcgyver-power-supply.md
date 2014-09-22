---
layout: post
title:  "McGyver Power Supply"
projectname: "mcVoltage"
date:   2008-12-30
comments: true
tags: projects
type: project
summary: This is probably one of the worst power supplies I have made. I was in middle school when I made this.
---

For all of your electronics projects, a power supply comes in handy in almost every situation. From making a simple LED circuit to designing High-Frequency RF circuitry Power-Supplies are a key to debugging and testing your circuitry.<br />
<br />
This article will help you make your own variable power supply from stuff you can find around your house.<br />
<br />
<span style="font-size: 180%; font-weight: bold;">Materials:</span><br />
<ol>
<li>An old TV, or a regular step-down transformer.</li>
<li>* A rectifier IC, or 4 diodes.</li>
<li>A light dimmer.</li>
<li>Alligator clips are nice, but not necessary.</li>
<li>Soldering Iron.</li>
<li>Solder.</li>
<li>An old power cable.</li>
<li>A surge protector with a breaker.</li>
<li>2.5A fuse.</li>
<li>Multimeter.</li>
</ol>
<span style="font-size: 180%;"><span style="font-weight: bold;">Difficult to find materials:</span></span><br />
<br />
<span style="font-size: 130%;">A rectifier IC or 4 diodes:</span><a href="http://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Bridge_rectifiers.jpg/590px-Bridge_rectifiers.jpg" onblur="try {parent.deselectBloggerImageGracefully();} catch(e) {}"><img alt="" border="0" src="http://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Bridge_rectifiers.jpg/590px-Bridge_rectifiers.jpg" style="cursor: pointer; float: left; height: 187px; margin: 0pt 10px 10px 0pt; width: 184px;" /></a><br />
<ul>
<li>On a basic level, a rectifier changes AC to DC.</li>
<li>The outlets in your wall are 120VAC</li>
<li>Most appliances run DC.</li>
<li>You can find a rectifier in almost everything you plug into a wall power outlet.</li>
</ul>
<br />
<ul>
<li>If you cannot find one, or wish to make one yourself--make the rectifier using this <a href="http://upload.wikimedia.org/wikipedia/commons/thumb/f/f5/Diode_bridge_alt_2.svg/557px-Diode_bridge_alt_2.svg.png">diagram</a>.</li>
</ul>
<br />
<span style="font-size: 180%;">Procedure:<span style="font-size: 100%;"><br /></span></span><br />
<ol>
<li>Strip your old power cable on the female end, exposing the Black (hot) White (neutral) Green (ground) leads. Your cable may not have a ground, this is fine.<br /></li>
<li>Solder the Neutral, and hot leads to the two terminals on your light dimmer.<br /></li>
<li>Next take the other side of your light dimmer (the side that normally connects to the lights) and solder that into your step-down transformer.<br /></li>
<li>Next, you will need to do a little bit of debugging. The wires on your transformer may not be labeled or color-coded correctly, so it is up to you to find out which wires connect to which coils (i.e. high Voltage, low voltage, and input).<br /></li>
<li>Once you find out which output leads hook to the different coils on the transformer, plug each of them into your diode bridge or rectifier IC circuit.<br /></li>
<li>After you rectify the AC from the output of your transformer solder a couple of wires to the output.<br /></li>
<li>Next, put something on the end of the output (I used an alligator clip) to make it easier for you to power your projects.</li>
</ol>
<span style="font-size: 180%;"><span style="font-weight: bold;">Conclusion:</span></span><br />
<br />
This is not the best way to make a power supply, but it can be done with things from around your house, so you cannot complain. Using an old desktop ATX power supply as a lab power supply is a much better idea than making a power supply this way. You can easily find instructions on Google for to modify an ATX power supply into a lab bench power supply. However there is one advantage to this type of power supply, when you turn the light dimmer, you are actually varying the total output power and not just the voltage.