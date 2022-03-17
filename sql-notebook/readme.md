- build image
```cmd
docker build -t kslader8/sql-notebook:python-3.9.7 - < dockerfile
```
- push to hub
```cmd
docker login
docker push kslader8/sql-notebook:python-3.9.7
```
- spin up a container using the image
```cmd
docker run -it --rm -p 8888:8888 kslader8/sql-notebook:python-3.9.7
```