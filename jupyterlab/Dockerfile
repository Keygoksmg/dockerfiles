FROM jupyter/datascience-notebook

# install jupyter lab
RUN pip install --upgrade pip && pip install jupyterlab
RUN jupyter serverextension enable --py jupyterlab


# Install "plotly"
RUN pip install --upgrade pip && pip install ipywidgets>=7.5 \
	plotly \
	holoviews
# JupyterLab renderer support
RUN jupyter labextension install jupyterlab-plotly@4.13.0