```
docker build -t backend-reader .
```
```
docker run -it -p 8000:8000 -v "/$(pwd)"/logs.txt:/mydir/logs.txt backend-reader
```
(Without quotes $(pwd) might give invalid reference format error.)


