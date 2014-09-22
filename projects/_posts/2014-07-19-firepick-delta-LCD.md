---
layout: post
title:  "Delta Robot LCD Console"
projectname: "firepickConsole"
date:   2014-07-19
comments: true
tags: projects
type: project
summary: An LCD screen used on the FirePICK delta robot for the hackaday.com competition
source: https://github.com/firepick-delta/firepick-delta-console
---
<div class="leaders">
<h2><li>Quick Information</li></h2>
The firepick-delta-console is a display which is used to give the user useful information about their FirePICK delta machine.

<h2>Features</h2>
*	IP Address Status
*	Time/date information

<h2>To-Do</h2>
*	Interface with FireREST software to display job completeness status bar
*	Display other useful system info
*	Add buttons to allow the user to scroll through informational the different screens.


<h2><li>Instillation</li></h2>
<h2>Requirements</h2>
* python-pip (for python 2.7)
* python 2.7
* python-setuptools
* pip package rpi.gpio


<h2>Automatic/Scripted Instillation</h2>
The install.sh script was written for a debian-based system, specifically the Raspberry Pi Rev. B running Raspberrian/FireREST. If you are using different software, please fork the repo and revise the script :).

* run the bash installer script install.sh.

<h2>Manual Instillation</h2>
1. Install the following dependancies manually:
  * Python 2.7
  * Python Setup Tools
  * rpi.gpio python package

2. Optional Dependancies:
  * Pip for Python 2.7 (for installing the rpi.gpio package)
 </div>