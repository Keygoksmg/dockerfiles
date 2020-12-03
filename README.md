# dockerfiles

# How to use
move to directory you want and run:
```
docker-compose up
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
