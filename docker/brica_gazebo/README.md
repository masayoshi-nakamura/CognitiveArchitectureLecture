# Quickstart

Assuming you have docker installed, run this to start brica-gazebo experiment environment. Docker will build container and run.

```
docker run -it -p 8888:8888 -p 8080:8080 -p 7681:7681 brica-gazebo
```

start gazebo server and gazebo web server,

```
/root/gzweb/start_gzweb.sh && gzserver /root/CognitiveArchitectureLecture/worlds/maze_turtlbot.xml &
```

You'll now be able to access http://localhost:8080/ 

<img src="https://github.com/masayoshi-nakamura/CognitiveArchitectureLecture/screenshots/gzweb_brica_maze.png" width=400/>


Running a BriCA sample agent

```
cd /root/CognitiveArchitectureLecture/examples/brica_agent 
python brica_agent.py
```



If you use iPython notebook and want to create your code

```
cd ~/CognitiveArchitectureLecture/examples/brica_agent
jupyter notebook --no-browser --port 8888 --ip=*
```

You'll now be able to access http://localhost:8888/ 


<img src="https://github.com/masayoshi-nakamura/CognitiveArchitectureLecture/screenshots/gzweb_brica_maze_and_ipythonnotebook.png" width=400/>



