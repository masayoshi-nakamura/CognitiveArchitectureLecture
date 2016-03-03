# Quickstart

Assuming you have docker installed, run this to start nengo-gazebo experiment environment. Docker will build container and run.

```
git clone https://github.com/masayoshi-nakamura/CognitiveArchitectureLecture.git
cd CognitiveArchitectureLecture/docker/nengo_gazebo
docker build --tag=nengo-gazebo .
docker run -it -p 8888:8888 -p 8080:8080 -p 7681:7681 nengo-gazebo
```

start gazebo server and gazebo web server,

```
/root/gzweb/start_gzweb.sh && gzserver /root/CognitiveArchitectureLecture/worlds/maze_turtlbot.xml &
```

You'll now be able to access http://localhost:8080/ 

<img src="https://cloud.githubusercontent.com/assets/1708549/13484633/fd0aa402-e142-11e5-8b4a-cd4be83954e4.png" width=400/>


Running a nengo sample agent

```
cd ~/CognitiveArchitectureLecture/examples/nengo_agent 
python nengo_agent.py
```



If you use iPython notebook and want to create your code

```
cd ~/CognitiveArchitectureLecture/examples/nengo_agent
jupyter notebook --no-browser --port 8888 --ip=*
```

You'll now be able to access http://localhost:8888/ 


<img src="https://cloud.githubusercontent.com/assets/1708549/13484604/d72e9cf2-e142-11e5-8ac9-e4eb9e8978c1.png" width=400/>



