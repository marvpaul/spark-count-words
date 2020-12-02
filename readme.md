# Word count using pySpark 
We use pySpark to count words in several languages. This includes some preprocessing (removing stop words) and some analysis for performance when using pySpark with different hardware settings. 

## How to run
This project is using a Dockerfile which creates a jupyter notebook enivorment for us with Spark preconfigured and the package stop-words which we use for removing stop-words. 
Install requirements: 
`docker build --rm -t jupyter/all-spark-notebook .`

Use this command to run the jupyter notebook docker image: 
`docker run -p 8888:8888  -v "$PWD":/home/jovyan/work jupyter/all-spark-notebook`
