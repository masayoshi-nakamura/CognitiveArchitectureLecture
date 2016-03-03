
# Brain Simulator controls TurtleBot in Gazebo Environment Demo

GoodAI's Brain Simulator V0.4 controls TurtleBot on Gazebo Environment.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=TRSP8eudr8s
" target="_blank"><img src="http://img.youtube.com/vi/TRSP8eudr8s/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

Tcp connection nodes in Brain Simulator communicate with python server and this server controls TurtleBot via PyGazebo.

## Run
Prepare two machines and connect same network.

 - Wiwndows (NVIDIA CUDA-enabled graphics card and 64-bit Windows) for Brain Simulator
 - Ubuntu for Gazebo (we use Ubuntu 14.04)
  
### Ubuntu 
Install Gazebo.

Install pygazebo

```
# Do not use version 3.0.0-2014.1 
git clone https://github.com/jpieper/pygazebo.git
cd pygazebo
git checkout 3eaac84
python setup.py install
```

 Install BriCA V1
https://github.com/wbap/BriCA1.git

Launch maze world

```
 gazebo worlds/maze_turtlbot.xml
```

Open new ternminal

```
cd examples/brica_brainsimulator_agent/
python brica_brainsimulator_agent.py
```


### Windows 
Install Brain Simulator and load brica_sample_agent.brain. Click simulation start button.
 
