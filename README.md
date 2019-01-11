# TF-Ranking docker image #


## Base Image ##
This is the docker image for TF-Ranking, its baseImage is from tensorflow/tensorflow:latest-gpu-py3

The Dockerfile content is from two sources:
-  [tensorflow dockerfile](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/tools/dockerfiles/dockerfiles/devel-gpu-jupyter.Dockerfile)
-  [tf_ranking dockerfile](https://github.com/gitathrun/tf_ranking_docker/blob/gpu-support/Dockerfile)


## Additional installed packages ##

## Docker Registry Repo ##


## Usage ##
on dsvm-gpu virtual machines
```
sudo docker login
```

```
sudo docker pull 
```

remember the target port is __8889__
```
sudo nvidia-docker run -it -p 8889:8888 -v <project-dir-path>:/app <image>
```

In local browser, remember the target port is __8889__
```
http://xxx.com:8889/?token=xxxx
```