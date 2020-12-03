FROM jupyter/datascience-notebook

# install jupyter lab
RUN pip install --upgrade pip && pip install jupyterlab
RUN jupyter serverextension enable --py jupyterlab

# jupyterlab setting
# make directory
RUN mkdir -p .jupyter/lab/user-settings/@jupyterlab/notebook-extension/ \
    && mkdir -p .jupyter/lab/user-settings/@jupyterlab/apputils-extension/
# copy setting files
COPY jupyterlab_setting/tracker.jupyterlab-settings .jupyter/lab/user-settings/@jupyterlab/notebook-extension/
COPY jupyterlab_setting/themes.jupyterlab-settings .jupyter/lab/user-settings/@jupyterlab/apputils-extension/



# Install "plotly"
RUN pip install --upgrade pip && pip install ipywidgets>=7.5 \
	plotly \
	holoviews
# JupyterLab renderer support
RUN jupyter labextension install jupyterlab-plotly@4.13.0
