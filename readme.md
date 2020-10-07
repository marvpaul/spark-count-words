# How to run
Use this command to run the jupyter notebook docker image: 
Install requirements: docker build --rm -t jupyter/all-spark-notebook .
docker run -p 8888:8888  -v "$PWD":/home/jovyan/work jupyter/all-spark-notebook
