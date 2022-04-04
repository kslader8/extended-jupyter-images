- build image
```cmd
docker build -t kslader8/sql-notebook:python-3.9.10 - < dockerfile
```
or
```powershell
Get-Content dockerfile | docker build -t kslader8/sql-notebook:python-3.9.10 -
```

- push to hub
```cmd
docker login
docker push kslader8/sql-notebook:python-3.9.10
```
- spin up a container using the image
```cmd
docker run -it --rm -p 8888:8888 kslader8/sql-notebook:python-3.9.10
```
- find the hosted [sql-notebook](https://hub.docker.com/repository/docker/kslader8/sql-notebook) image
