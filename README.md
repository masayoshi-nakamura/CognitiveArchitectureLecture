# A prototype of simple agent with simulation environment using BriCA, Nengo and Brain Simulator

<img src="https://cloud.githubusercontent.com/assets/1708549/13484633/fd0aa402-e142-11e5-8b4a-cd4be83954e4.png" width=400/>

## Quickstart with docker

 - using BriCA: [BriCA-Gazebo docker](/docker/brica_gazebo)
 - using Nengo: [Nengo-Gazebo docker](/docker/nengo_gazebo)
 - using Brain Simulator: [Brain Simulator and BriCA](examples/brica_brainsimulator_agent)

-------------
## Installation (Mac, Ubuntu)
### Requirements
Minimum requirements:

 - Python 2.7

 - Gazebo 2.2+

 - pygazebo
 
 - BriCA V1

 - [BriCA Language](https://github.com/rondelion/brical.git)

 - Nengo 2.0


### Installation (Mac, Ubuntu)

 - pygazebo
```bash
 # Do not use version 3.0.0-2014.1 
 git clone https://github.com/jpieper/pygazebo.git
 cd pygazebo
 git checkout 3eaac84
 python setup.py install
```

 - BriCA V1
https://github.com/wbap/BriCA1.git

 - Nengo 2.0
```bash
 pip install nengo
 pip install nengo_gui
```

## Simple Usage

Launch maze world
```bash
 gazebo worlds/maze_turtlbot.xml
```
Open new ternminal, 

```bash
 cd examples/brica_agent/
 python brica_agent.py
```

