# A prototype of simple BriCA agent with simulation environment

## Requirements
Minimum requirements:

 - Python 2.7

 - Gazebo 2.2+

 - pygazebo
 
 - BriCA V1

 - [BriCA Language](https://github.com/rondelion/brical.git)

 - Nengo 2.0


## Installation (Mac, Ubuntu)

 - Gazebo
 
[Mac](http://gazebosim.org/tutorials?tut=install_on_mac&),
[Ubuntu](http://gazebosim.org/tutorials?tut=install_ubuntu&)

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

## License

Apache License 2.0 (see `LICENSE` file).
