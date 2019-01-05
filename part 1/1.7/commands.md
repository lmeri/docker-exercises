Place Dockerfile from /front to /frontend-example-docker and from /back to /backend-example-docker

```
docker build -t backend ./backend-example-docker
```
```
docker build -t frontend ./frontend-example-docker
```
```
docker run -it -d -p 8000:8000 -v "/$(pwd)"/backend-example-docker/logs.txt:/mydir/logs.txt backend
```
```
docker run -d -p 5000:5000 frontend
```