# Brain Simulator controls TurtleBot in Gazebo
GoodAI's Brain Simulator V0.4 controls TurtleBot on Gazebo Environment.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=TRSP8eudr8s
" target="_blank"><img src="http://img.youtube.com/vi/TRSP8eudr8s/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

Tcp connection nodes in Brain Simulator communicate with python server and this server controls TurtleBot via PyGazebo.

This prototype module is red box. 
<img width="796" alt="2016-03-08 13 12 15" src="https://cloud.githubusercontent.com/assets/1708549/13591810/80346f62-e52f-11e5-8cf7-6b2b6760de76.png">

# Quickstart
## Run
Prepare two machines and connect same network.

 - Wiwndows (for Brain Simulator)
  - 64-bit Windows 7, 8, 8.1 or 10
  - NVIDIA CUDA-enabled graphics card
 - Ubuntu (for Gazebo)
  - we use Ubuntu 14.04
  
  
### Ubuntu 
[Install Gazebo](http://gazebosim.org/tutorials?tut=install_ubuntu).

Install pygazebo:

```
# Do not use version 3.0.0-2014.1 
git clone https://github.com/jpieper/pygazebo.git
cd pygazebo
git checkout 3eaac84
python setup.py install
cd ../
```

Install BriCA V1:

```
https://github.com/wbap/BriCA1.git
git clone https://github.com/wbap/BriCA1.git
cd BriCA1
git checkout 0261df0
python setup.py install
cd ../
```

Launch maze world:

```
git clone https://github.com/masayoshi-nakamura/CognitiveArchitectureLecture.git
gazebo CognitiveArchitectureLecture/worlds/maze_turtlbot.xml
```

Open new ternminal, start brainsimulator_agent.py

```
cd CognitiveArchitectureLecture/examples/brica_brainsimulator_agent/
python brainsimulator_agent.py
```


### Windows 
Install Brain Simulator and load brica_sample_agent.brain. Check Ubuntu PC's IP address and edit tcp connection nodes(sensor and action node). Then, click simulation start button.
 