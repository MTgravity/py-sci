FROM jupyter/datascience-notebook

RUN python --version

RUN conda install --quiet --yes -c \
    conda-forge osmnx dask

COPY requirements.txt ./
RUN conda install --file requirements.txt

WORKDIR /notebooks