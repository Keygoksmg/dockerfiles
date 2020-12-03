# dockerfiles

# How to use
1. clone this repository to the dir in which you want to volume files
(if you want, you can change directory for volume in docker-compsoe.yml)
```
$ cd <your working dir>
$ git clone https://github.com/Keygoksmg/dockerfiles
```

2. 
move to one of the directory of <b>dockerfiles</b>
```
e.g. $ cd  jupyterlab
```

3.
run the following and open localhost:<defined port> on browser
```
$ docker-compose up
```

# Type of docker files
each directory are composed of "Dockerfile" and "docker-compose.yml".
The explanation of directory are the following:

### jupyterlab
Using "jupyter/datascience-notebook", you can add needed packages with "pip install xxx".

### jupyterlab_with_graphtool
Using "ubuntu:18.04", you can use "graphtool" which enables you to network analysis.
It is optimazed for Network analysis, however, you cannot use plotly and other extensions working with nodejs.
I'm not sure what worng with graphtool, but installation of graph_tool is complicated and out of my hand.
Other network analysis tool(networkx) as well installed and make you easier for starting network analysis.
