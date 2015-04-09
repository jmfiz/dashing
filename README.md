# dashing

This docker starts dashing service 
 
It contains the following components:
- Ubuntu 14.04
- Dashing
- Supervisor

##Quickstart

Build the image:

```
docker build -t dashing .
```

then run:

```
docker run -d -p 3030:3030 dashing

```

Or run the image without building:

```
docker run -d -p 3030:3030 jmfiz/dashing
```

A volume is created at /dashboard to host the components of your dashboard. If you want to mount to modify or save its content you could run:

```
docker run -v {your/local/path}:/dashboard -d -p 3030:3030 jmfiz/dashing
```
