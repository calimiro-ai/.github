# Calimiro AI

<h2>A powerful smart mirror to film and track your workout session with AI.</h2>
Built in Munich, Germany, by Lennard Gross, Philip Synowiec und Younes Bendimerad at <a href="https://www.github.com/check24">@CHECK24</a>  
<br><br>


<img src="thumbnails/thumbnail_mirror_real.jpg"/>




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

You will see your mirror run by pointing your browser to: localhost:8080


<h3>Configure your mirror</h3>

You can change the port or the IP address by editing the config/config.js file of calimirror. Please see the <a href="https://www.docs.magicmirror.builders">MagicMirror documentation</a> for details.



Copyright &copy; Lennard Gross, Philip Synowiec and Younes Bendimerad, 2025. All rights reserved.