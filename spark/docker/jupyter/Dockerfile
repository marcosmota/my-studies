FROM jupyter/pyspark-notebook

USER root

# Install java 8
RUN apt-get update \
    && echo "Updated apt-get" \
    && apt-get install -y openjdk-8-jre \
    && echo "Installed openjdk 8"

# install jupyterthemes
RUN pip install jupyterthemes
# upgrade to latest version
RUN pip install --upgrade jupyterthemes

USER $NB_UID

COPY ./requirements.txt .
RUN pip install -r requirements.txt
