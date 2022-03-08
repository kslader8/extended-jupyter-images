- build image
```docker build -t kslader8/fastai-notebook:python-3.9.7 - < dockerfile```
- push to hub
```
docker login
docker push kslader8/fastai-notebook:python-3.9.7
```
- spin up a container using the image
```
docker run -it --rm -p 8888:8888 kslader8/fastai-notebook:python-3.9.7
```
