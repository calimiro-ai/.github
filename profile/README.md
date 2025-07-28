# Calimiro AI

<h2>A powerful smart mirror to film and track your workout session with AI.</h2>
Built in Munich, Germany, by Lennard Gross, Philip Synowiec und Younes Bendimerad at <a href="https://www.github.com/check24">@CHECK24</a>  
<br><br>


<img src="thumbnails/thumbnail_mirror_real.jpg"/>

<br>

<h2>Calimiro</h2>

<h3>Our goal</h3>

Calimiro AI develops a smart mirror, which is able to track your workout session and to recognize the workout exercise you're doing. It can also count repetitions, and so establish reliable statistics about your global performance.

We want to make fitness and calisthenics easier for people who are starting in this discipline, without forcing them to be in the gym or to have a coach.

<h3>Project overview</h3>

A Calimiro consists of several components. A Raspberry Pi 4+, a transparent mirror with integrated display, and an ESP Camera. A webserver permits a WiFi connection between the Raspberry Pi and the Camera to establish an HTTP (or on newer versions RTSP) live video stream. The core of Calimiro, Calitracker, runs on the Raspberry Pi and analyzes your position with several pre-trained AI models. Another server runs on the Raspberry Pi to permit communication with the User Interface, built with <a href="www.magicmirror.builders">MagicMirror</a>.

<h3>Future updates</h3>

&bull;	Websockets for a better architecture  
&bull;  Built-in computation of calories  
&bull;  Pose & gesture correction  
&bull;  Workout Session Program generation with AI  
&bull;  3D pose & gesture models on the mirror  
&bull;  Interactive plots of workout data  

<br>

<h2>Getting started</h2>

Calimiro AI does not provide the required hardware to run any Calimiro device.


<h3>Installing</h3>

You can start by cloning the tracker repository and the mirror repository.

```
git clone https://github.com/calimiro-ai/calitracker
git clone https://github.com/calimiro-ai/calimirror
```

<h3>Start Calitracker</h3>

Run the calitracker server on your OS

```
cd calitracker
python src/backend_interface/server.py
```


<h3>Start Calimirror</h3>

You can update the required dependencies for your MagicMirror server for the frontend with:

```
cd calimirror
npm install
```

Run it with:
```
npm run server
```

You will see your mirror in action by pointing your browser to <a href="http://localhost:8080">your mirror</a>. 

<h3>Configuring your mirror</h3>

You can change the port or the IP address by editing the config/config.js file of calimirror. Please see the <a href="https://www.docs.magicmirror.builders">MagicMirror documentation</a> for details.

<br>
<br>

Copyright &copy; Lennard Gross, Philip Synowiec and Younes Bendimerad, 2025. All rights reserved.