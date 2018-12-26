```
docker build -t backend-reader .
```
```
docker run -it -p 8000:8000 -v "/$(pwd)"/logs.txt:/mydir/logs.txt backend-reader
```
(Without quotes $(pwd) gives invalid reference format error.)

Or, if you want to use the logs.txt file in the backend-example-docker folder, use:
```
docker run -it -p 8000:8000 -v "/$(pwd)"/backend-example-docker/logs.txt:/mydir/logs.txt backend-reader
```


