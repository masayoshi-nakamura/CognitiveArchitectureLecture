# Quickstart

Assuming you have docker installed, run this to start brica-gazebo experiment environment.

```
$ docker run -it -p 8888:8888 -p 8080:8080 -p 7681:7681 brica-gazebo
```

Docker will build container and after building, to start gazebo server and gazebo web server,

```
/root/gzweb/start_gzweb.sh && gzserver /root/CognitiveArchitectureLecture/worlds/maze_turtlbot.xml &
```

You'll now be able to access http://localhost:8080/ 


Running a BriCA sample agent

```
cd /root/CognitiveArchitectureLecture/examples/brica_agent 
python brica_agent.py
```



If you use iPython and want to create your code

```
jupyter notebook --no-browser --port 8888 --ip=*
```

You'll now be able to access http://localhost:8888/ 


