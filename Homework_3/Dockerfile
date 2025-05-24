FROM jupyter/base-notebook

USER root
RUN apt-get update && apt-get install -y git

USER jovyan
WORKDIR /home/jovyan/work

COPY . /home/jovyan/work

EXPOSE 8888

CMD ["start-notebook.sh", "--NotebookApp.token=''", "--NotebookApp.password=''"]
