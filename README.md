# qgis-vice
Docker build for running QGIS in CyVerse VICE

To run locally:

```
docker run -it -p 5901:5901 -p 6901:6901 tswetnam/ubuntu-xfce-vnc:latest
```

To run locally with NVIDIA drivers:
```
docker run -it --runtime=nvidia -v /tmp/.X11-unix:/tmp/.X11-unix -v /tmp/.docker.xauth:/tmp/.docker.xauth -p 5901:5901 -p 6901:6901 tswetnam/ubuntu-xfce-vnc:opengl

```
