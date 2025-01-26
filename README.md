# Dataeng-zoomcamp Cohort 2025
This notebook is dedidicated for collecing notes on learning Data Engineering concepts via dataeng-zoomcamp cohort 2025. My official start date is January 25, 2025.



## Module 1 Docker + Postgress

### Docker Basics

Docker is a _containerization software_ that allows us to isolate software in a similar way to virtual machines but in a much leaner way.

A Docker image is a snapshot of a container that we can define to run our software, or in this case our data pipelines. By exporting our Docker images to Cloud providers such as Amazon Web Services or Google Cloud Platform we can run our containers there.

Docker provides the following advantages:

- Reproducibility
- Local experimentation
- Integration tests (CI/CD)
- Running pipelines on the cloud (AWS Batch, Kubernetes jobs)
- Spark (analytics engine for large-scale data processing)
- Serverless (AWS Lambda, Google functions)

Docker containers are stateless: any changes done inside a container will NOT be saved when the container is killed and started again. This is an advantage because it allows us to restore any container to its initial state in a reproducible manner, but you will have to store data elsewhere if you need to do so; a common way to do so is with volumes.


> Note: you can learn more about Docker and how to set it up on a [Mac](https://github.com/ziritrion/ml-zoomcamp/blob/11_kserve/notes/05b_virtenvs.md#docker) in this link. You may also be interested in a Docker reference [cheatsheet](https://gist.github.com/ziritrion/1842c8a4c4851602a8733bba19ab6050#docker).


### Docker to Postgress

**Mounting** is the action of hosting your data in a local machine which docker will be mapped to. 
